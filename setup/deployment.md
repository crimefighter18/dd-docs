# Deployment

In order to measure deployment (production deployments) DevDynamics needs to understand what counts as Deployment. To configure your Deployment navigate to [https://app.devdynamics.ai/settings/dora](https://app.devdynamics.ai/settings/dora) and click the Deployment tab

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 at 7.51.26 PM.png" alt=""><figcaption></figcaption></figure>

Devdynamics can detect deployment from multiple sources as  shown in the above image

* Issue Management - Many organizations manage their Deployments in Issue management systems like Jira or Linear. You can provide filter criteria like ticket type, ticket label, or any custom field name and value. All issues satisfying this filter criteria will be considered as deployment.
* Pull request merge to certain branches - If your pull request is merged to provided branches it will be considered as deployment. For example, if you provide value _**release\***_ pull request merge to any release branch, it will be counted as deployment.  **Please note this is the default option with the branch name as **_**main,master**_** (to support multiple branch comma separated values can be provided)**
* Git action, Jenkins, or API - This is the most accurate option as we know exactly at what time deployment was triggered and completed.  If you have integrated Github, deployment through GitHub actions will be automatically captured. Similarly, if you have integrated Jenkins all builds run with the provided job name pattern will be counted as deployment. In case you are using any other ci/cd tool you can send us a deployment event through our API.

### Team Tracking

&#x20;To ensure correct deployments are tagged to the team you also need to select which field to use for team tracking purposes. Once the option is selected its value has to be provided in the team config page. For example, if you select repository for team tracking then for all teams you need to provide a team repository as below.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 at 7.48.25 PM (1).png" alt=""><figcaption></figcaption></figure>
