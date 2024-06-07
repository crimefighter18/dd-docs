# Work Breakdown: Distribution of Work (Lines of Code)

### **1. Introduction:**

This document explains how to analyze and visualize the distribution of work across different categories using the **Work Breakdown** metric. It's presented as a stacked bar chart showing the percentage of code attributed to new development (New Work), rework, refactoring, and helping others. This metric provides valuable insights into team dynamics, development efficiency, and potential areas for improvement.

### **2. Definitions:**

* **Work Breakdown:** A categorization of development efforts into various activities:
  * **New Work (Green):** New Work (%) tracks the percentage of code added to the codebase that doesn't directly replace existing code.. Lines of code written for new features or functionalities.
  * **Rework (Red):** Churn (%) tracks the percentage of code that is rewritten or deleted within a specific timeframe (typically 21 days, but adjustable). Lines of code modified or fixed due to errors or requirement changes.
  * **Refactor (Blue):** Refactor (%) tracks the percentage of code that has been updated or rewritten after a specific timeframe (typically 21 days). Lines of code refactored to improve code quality, readability, or maintainability without changing functionality.
  * **Help Others (Yellow):** Helped Others (%) tracks the percentage of code that has been updated by a contributor other than the one who initially wrote it. Lines of code updated by a different contributor than the original author.

### **3. Explanation of Charts:**

**KPI Card:**

<div align="left">

<figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

</div>

**Detailed Chart:**

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

The stacked bar chart displays the distribution of work categories (New Work, Rework, Refactor, Help Others) for a chosen timeframe (e.g., week, month).

* **Horizontal Axis:** Represents the time period (e.g., weeks, months).
* **Vertical Axis:** Represents the percentage of total lines of code.
* **Stacked Bars:** Each section of the bar represents a work category percentage.
  * **Green:** New Work
  * **Red:** Rework
  * **Blue:** Refactor
  * **Yellow:** Help Others
* **Color Indicators:**
  * **Green:** Less than 20% Rework (indicating efficient development with minimal rework).
  * **Amber:** Between 20% and 40% Rework (indicating some inefficiency requiring attention).
  * **Red:** More than 40% Rework (indicating significant rework, potentially due to unclear requirements or inefficient processes).

### **4. Interpretation:**

**Identifying Development Efficiency:** The Work Breakdown chart helps visualize the distribution of effort across different activities.

* **High New Work (Green):** A healthy percentage of new work indicates active development progress.
* **Low Rework (Green):** A low percentage of rework suggests efficient development practices and well-defined requirements.
* **Balanced Refactor (Blue):** A moderate amount of refactoring indicates ongoing code quality improvement.
* **Balanced Help Others (Yellow):** Collaboration through code contributions suggests knowledge sharing and a supportive team environment.

### **5. Key Points:**

* **Development Insights:** Work Breakdown provides insights into team dynamics, effort allocation, and potential areas for improvement.
* **Rework Efficiency:** Monitor the Rework percentage to identify opportunities for improving requirement clarity, development processes, or code quality.
* **Teamwork and Collaboration:** Help Others percentage indicates knowledge sharing and collaborative development practices.

### **6. Conclusion:**

Monitoring Work Breakdown provides valuable insights into your team's development efforts and efficiency. By analyzing the distribution of work categories and taking corrective actions when necessary, you can optimize development processes, minimize rework, and promote a collaborative work environment.
