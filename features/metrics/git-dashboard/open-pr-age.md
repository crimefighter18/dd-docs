# Open PR Age

### **1. Introduction:**

This document explains how to analyze and visualize the timeliness of your code review process using the **Open PR Age** metric. It categorizes Pull Requests (PRs) based on the length of time they have remained open and presents the distribution in a pie chart.

Monitoring Open PR Age provides valuable insights into identifying bottlenecks in the review process, mitigating risks associated with long-standing PRs, and promoting efficient code review practices.

### **2. Definitions:**

* **Pull Request (PR):** A proposed modification to a codebase that is submitted for review before being merged into the main branch.
* **Open PR Age:** The amount of time a PR has remained open since its creation.

### **3. Explanation of Charts:**

**KPI Card:**

<div align="left">

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

</div>

**Detailed Chart:**

<figure><img src="../../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

The pie chart displays the distribution of open PRs across different age categories:

* **Less than 1 Day:** PRs open for less than 24 hours.
* **Less than 3 Days:** PRs open between 1 and 3 days (not including the first day).
* **Less than 7 Days:** PRs open between 4 and 7 days (not including the 3rd day).
* **Less than 14 Days:** PRs open between 8 and 14 days (not including the 7th day).
* **Less than 1 Month:** PRs open between 15 days and 30 days (not including the 14th day).
* **Above 1 Month:** PRs open for more than 30 days.

**Color Indicators:**

* **Green:** More than 90% of PRs are open for less than one day (indicating a highly responsive review process).
* **Amber:** Between 80% and 90% of PRs are open for less than one day (indicating room for improvement in review timeliness).
* **Red:** Less than 80% of PRs are open for less than one day (indicating significant delays in the review process).

### **4. Interpretation:**

**Identifying Bottlenecks:** The Open PR Age pie chart helps visualize the distribution of PRs across different age groups.

* **High Percentage of Old PRs (Red):** This may indicate bottlenecks in the review process, reviewer overload, or lack of prioritization. Investigate further to identify and address the root causes.
* **Moderate Age Distribution (Amber):** While some PRs are reviewed quickly, there's potential for improvement in overall review timeliness. Consider implementing process changes or communication strategies.
* **Favorable Age Distribution (Green):** This suggests a highly responsive review process with most PRs being addressed promptly. Analyze if there are best practices to share and maintain this efficiency.

### **5. Key Points:**

* **Review Timeliness:** Open PR Age helps assess the effectiveness of your code review process in terms of time taken to review and merge PRs.
* **Risk Mitigation:** Addressing old PRs helps minimize context loss, unproductive work, and dependency risks associated with long-standing code changes.
* **Process Improvement:** Monitoring Open PR Age allows you to identify areas for improvement and implement changes to promote faster review turnaround times.

### **6. Conclusion:**

Monitoring Open PR Age provides valuable insights into the timeliness of your code review process. By analyzing the distribution and taking corrective actions when necessary, you can identify bottlenecks, promote faster review cycles, and ensure a more efficient and productive development workflow.
