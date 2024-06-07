# Cycle Time Metrics

Cycle time is one of the most important engineering metrics. Cycle time metrics in software engineering typically measure the time it takes for a work item to move through various stages of the software development process.

**Waiting Time:**

This is the duration from when an issue management ticket is created to the moment the first commit is made for that ticket. To calculate this duration, a link between the git pull request and the ticket ID is necessary. Therefore, we recommend that teams include the issue ID in the pull request title. Utilize a working agreement to enforce this practice.

**Coding Time:**

This duration represents the time from the moment the first commit is made in a pull request to the point when the pull request is raised.

**Pickup Time:**

The pickup time is the duration between the issuance of a pull request and the initiation of its review process. The start of a review is marked by someone beginning to review by adding comments or approving the pull request.

**Merge Time:**

Merge time refers to the duration required to successfully complete a code review and merge a pull request into the codebase. It is calculated as the period between the initial start of the review and the moment when the pull request is merged.

**Deploy Time:**

Deploy time refers to the duration it takes to release code to the production environment. It is calculated from the moment a pull request is merged until the code is successfully deployed in the production environment. For precise deployment time measurement, we recommend integrating your deployment tool with DevDynamics.

#### PR Cycle Time:

PR Cycle Time refers to the duration it takes to merge a pull request. It represents the time interval between the initiation of a pull request and its successful merging into the codeba

**Lead Time for Change:**

Lead Time for Change refers to the duration between the moment a code change is committed and when it is successfully deployed. This metric is calculated by determining the date of the first commit in a pull request and tracking it until the corresponding changes are deployed in the production environment. The Lead Time for Change encompasses the sum of deployment time, merge time, pickup time, and coding time.
