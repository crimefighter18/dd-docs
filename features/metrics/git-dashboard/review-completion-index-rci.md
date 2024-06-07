# Review Completion Index (RCI)

### 1. Introduction:

This document explains how to analyze and visualize engagement and thoroughness within your code review process using the Review Completion Index (RCI). RCI is presented as a percentage distribution of Pull Requests (PRs) that have received at least one review comment.

Monitoring RCI provides valuable insights into identifying incomplete reviews, gauging reviewer engagement, and tracking the effectiveness of implemented improvements.

### 2. Definitions:

* Review Completion Index (RCI): The percentage of Pull Requests (PRs) where at least one review comment has been submitted.

### 3. Explanation of Charts:

Detailed Chart:

<figure><img src="../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

The stacked bar chart displays the distribution of PRs based on whether they received at least one review comment (Completed Review with Comment, No Review Comments).

* Horizontal Axis: Represents the completion status of PR reviews (Completed Review with Comment, No Review Comments).
* Vertical Axis: Represents the percentage of total PRs for each completion status category.  (Completed Review with Comment, No Review Comments).
* Tooltips: Hovering over a bar segment reveals additional details:
* Completed Review with Comment: Count of PRs with at least one review comment.
* No Review Comments: Count of PRs with no review comments.

Color Indicators:

* Green: RCI ≥ 90% (Healthy)
* Amber: 70% ≤ RCI < 89% (Caution)
* Red: RCI < 70% (Warning)

### 4. Interpretation:

Identifying Incomplete Reviews: A low RCI (red/amber) may indicate:

* Reviewer Inactivity: Certain reviewers might not be completing assigned reviews.
* Unclear Expectations: Reviewers might be unsure about the expected level of detail for comments.
* Technical Limitations: Tools or workflows might hinder reviewers from leaving comments easily.

Gauging Review Engagement: A high RCI (green) suggests reviewers are actively participating and providing feedback, potentially improving code quality and developer satisfaction.

### 5. Key Points:

* Improved Code Quality: RCI helps identify PRs that might lack thorough review, potentially leading to improved code quality.
* Reviewer Engagement: Monitoring RCI provides insights into reviewer participation and helps ensure a healthy review culture.
* Process Improvement: Tracking changes in RCI over time allows you to assess the effectiveness of efforts aimed at improving review thoroughness.

### 6. Conclusion:

Monitoring RCI provides valuable insights into the engagement and thoroughness of your code review process. By analyzing the distribution and taking corrective actions when necessary, you can identify incomplete reviews, improve reviewer engagement, and ultimately deliver higher quality software.

Related Metrics:

* PR Merged without Review
* PR Review Time
* Reviewer Distribution
* Average Number of Comments per Review

Additional Considerations:

* Analyze RCI alongside other metrics to gain a holistic view of the review process.
* Conduct a combination of quantitative and qualitative analysis to understand the reasons behind low RCI.
