---
description: >-
  To accurately track deployment events, DevDynamics needs to know when your
  application is deployed. Send deployment event by calling out API on Jenkins.
---

# Jenkins



#### CURL request&#x20;

```
curl --location \
 --request \
 POST 'https://api.devdynamics.ai/api/v1/deployment/yourorgId/notify' \
--header 'X-api-key: c70794a8-7184-43a1-a100-fddb85c2d4be' \
 \
--header 'X-delivery: c70794a8-7184-43a1-a100-fddb85c2d4bead' \
 \
--header 'X-event: cd' \
 \
--header 'Content-Type: application/json' \
 \
--data \
-raw '{
                    "id": "02537f6d-9196-4b59-a022-248e1ea7834a",
                    "timeStamp": "2023-06-27T11:38:17+00:00",
                    "htmlUrl": "https://api.github.com/repos/devdynamics-ai/devd-client/deployments/696863512",
                    "source": "git",
                    "issueId": "JIRA-123",
                    "assignee": "hello@devdynamics.ai",
                    "status": "success",
                    "repository": "devd-client",
                    "environment": "Production",
                    "commit": "a6264fbf55601a45890b98b55ce016c567a20dc9",
                    "prId": "2342346",
                    "branch": "main",
                    "artifact": "frontend-v1.0"
                  }'
```

#### Below is a sample Pipeline Script for same

```
pipeline {
    agent any


    environment {
        REPOSITORY = 'simple-maven-project-with-tests.git'
        ENVIRONMENT = 'Production'
        COMMIT_ID = null
        BRANCH = null
    }


    stages {
        stage('Build') {
            steps {
                script {
                    git 'https://github.com/jglick/simple-maven-project-with-tests.git'
                    sh 'mvn -Dmaven.test.failure.ignore=true clean package'
                
                
                // git url: REPOSITORY


                // sh 'mvn -Dmaven.test.failure.ignore=true clean package'
                }
            }


            post {
                success {
                    script {
                    def timeStamp = new Date().format('yyyy-MM-dd\'T\'HH:mm:ss\'Z\'')
                    def scmVars = checkout([$class: 'GitSCM', branches: [[name: 'master']], 
    userRemoteConfigs: [[url: 'https://github.com/jglick/simple-maven-project-with-tests.git']]])


                    
                    httpRequest contentType: 'APPLICATION_JSON', httpMode: 'POST', ignoreSslErrors: true, quiet: true, requestBody: """
                    {
                        "id": "${BUILD_NUMBER}",
                        "timeStamp": "${timeStamp}",
                        "commit": "${scmVars.GIT_COMMIT}",
                        "htmlUrl": "https://api.github.com/repos/devdynamics-ai/devd-client/deployments/696863512",
                        "source": "jenkins",
                        "issueId": "JIRA-123",
                        "assignee": "rishi@xyz.com",
                        "status": "completed",
                        "repository": "${REPOSITORY}",
                        "environment": "${ENVIRONMENT}",
                        "branch": "${scmVars.GIT_BRANCH}",
"artifact": ""
                    }
                    """, responseHandle: 'NONE', url: 'https://api.devdynamics.ai/api/v1/deployment/yourorgId/notify', wrapAsMultipart: false
                }
                    
                }
                failure {
                    script {
                    def timeStamp = new Date().format('yyyy-MM-dd\'T\'HH:mm:ss\'Z\'')
                    def COMMIT_ID = sh(returnStdout: true, script: 'git rev-parse HEAD').trim()
                    
                    def BRANCH = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
                    
                    httpRequest contentType: 'APPLICATION_JSON', httpMode: 'POST', ignoreSslErrors: true, quiet: true, requestBody: """
                    {
                        "id": "${BUILD_NUMBER}",
                        "timeStamp": "${timeStamp}",
                        "commit": "${scmVars.GIT_COMMIT}",
                        "htmlUrl": "https://api.github.com/repos/devdynamics-ai/devd-client/deployments/696863512",
                        "source": "jenkins",
                        "issueId": "JIRA-123",
                        "assignee": "rishi@xyz.com",
                        "status": "failed",
                        "repository": "${REPOSITORY}",
                        "environment": "${ENVIRONMENT}",
                        "branch": "${scmVars.GIT_BRANCH}",
"artifact": ""
                    }
                    """, responseHandle: 'NONE', url: 'https://api.github.com/repos/devdynamics-ai/devd-client/deployments/696863512', wrapAsMultipart: false
                }
                    
                }
            }
        }
    }
}
```
