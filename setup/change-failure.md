# Change Failure

In order to measure change failure (production failures like incidents) DevDynamics needs to understand what counts as change failure. To configure your change failure navigate to [https://app.devdynamics.ai/settings/dora](https://app.devdynamics.ai/settings/dora) and click the Change Failure Tab

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 at 7.02.26 PM.png" alt=""><figcaption></figcaption></figure>

Devdynamics can detect change failure from two sources as  shown in the above image

* Issue Management - Many organizations manage their change failure in Issue management systems like Jira or Linear. You can provide filter criteria like ticket type, ticket label, or any custom field name and value. All issues satisfying this filter criteria will be considered as change failures. **Please note this is a default option with filter criteria as **_**`Ticket type Prod Bug,incident,Incident,ProdBug`**_** (to support multiple ticket type comma separated values can be provided)**
* Incident Management - If your organization is using an incident management system like PagerDuty. You can choose this option. However, before that make sure you integrate your incident management system at [https://app.devdynamics.ai/settings/integrations](https://app.devdynamics.ai/settings/integrations). DevDynamics will count all PagerDuty incidents as change failures. If you want to further filter them please contact us at support@devdynamics.ai

### Team Tracking

&#x20;To ensure correct change failures are tagged to the team you also need to select which field to use for team tracking purposes. Once the option is selected its value has to be provided in the team config page. For example, if you select label (label field in issue management tickets) for team tracking then for all teams you need to provide a label as below.

<figure><img src="../.gitbook/assets/Screenshot 2023-11-29 at 7.48.25 PM.png" alt=""><figcaption></figcaption></figure>

