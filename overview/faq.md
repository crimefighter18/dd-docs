# ❓ FAQ



### How does DevDynamics ensure the security of my data?

As a SOC2-certified company, DevDynamics prioritizes the protection of your data. Our platform employs encryption measures during transit and while at rest, ensuring your data remains secure and confidential. We are deeply committed to upholding data privacy standards and regulations. Moreover, should you request it, we promptly and securely delete customer data as part of our data management procedures.

### How to integrate tools behind a firewall?

To enable DevDynamics to connect with tools that are situated behind your firewall, you must permit the following IP address on your firewall settings:&#x20;

* 3.131.112.244

Additionally, to ensure your tools can successfully make webhook calls to DevDynamics, please allow outgoing traffic to [https://api.devdynamics.ai](https://api.devdynamics.ai/)

### How does the team filter work?

When you apply a team filter within DevDynamics, the system considers all [team members](../setup/manage-teams.md) associated with that team and filters the data accordingly. For instance, in Git Metrics, applying a team filter results in data filtration based on team members who have performed activities on Git.

Please be aware that not all integrations provide us with users' email IDs. Therefore, in order to map team members to their respective integration user accounts, it is necessary to link contributors to their emails. You can perform this mapping at [https://app.devdynamics.ai/settings/contributors](https://app.devdynamics.ai/settings/contributors). For detailed instructions, refer to [https://docs.devdynamics.ai/setup/merge-contributors](https://docs.devdynamics.ai/setup/merge-contributors).

Keep in mind that certain integration data points may lack specific assignees, such as deployment data. In such cases, filtering is conducted based on the projects you have selected in your team configuration.

###





