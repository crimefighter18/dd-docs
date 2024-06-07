# Review Responsiveness Index (RRI)

### 1. Introduction:

This document explains how to analyze and visualize the responsiveness of your code review process using the Review Responsiveness Index (RRI). RRI is presented as a percentage distribution of reviews completed within 24 hours of being requested.

Monitoring RRI provides valuable insights into identifying bottlenecks, gauging team responsiveness, and tracking improvements in the review process.

### 2. Definitions:

* Review Responsiveness Index (RRI): The percentage of Pull Requests (PRs) where a review is completed within 24 hours of being requested.

### 3. Explanation of Charts:

KIP Card:

![](https://lh7-us.googleusercontent.com/docsz/AD\_4nXftm3dY2tELiJT6eM50DUQQxdjIUbmhWcZXQ0DKCZZtNVGnN9g5yFyiy9gEQxpIc6gcfcCMSjB-YRi7iyDRKLGDd\_ReZGk9fxa9bZV7KE\_6ALNnTdmgLPtKG32trpmRDKySq\_fP8sCcknWoY1hG3BrOtGOi?key=-INm7B8w7RH2\_Tgu\_VwbSQ)\
Detailed Chart:

<figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXdyDuZ_wp6ozkiUuiBwcZVLXkxi89WZSDZd6TwyeUmy8_I3TMwWaCdGjXibreQjLUMU-y5B_nLU7RmysVj6kgUwWkJic6ZOMd5HgydnCKHHdBTf3HVdNt3TLXjThFNHQaXlzKiDwFNX-L9lSzPWUPaFozHX?key=-INm7B8w7RH2_Tgu_VwbSQ" alt=""><figcaption></figcaption></figure>

The stacked bar chart displays the distribution of PR reviews based on completion time relative to the request (within 24 hours or after 24 hours).

* Vertical Axis: Represents the percentage of total PRs for each timeframe category. (Reviewed within 24 hours, Reviewed after 24 hours).
* Tooltips: Hovering over a bar segment reveals additional details:
* Reviewed within 24hrs, as percentage of Total PRs merged:
  * Count of PRs reviewed within 24 hours.
* Reviewed after 24hrs,  as percentage of Total PRs merged:
  * Count of PRs reviewed after 24 hours.

Color Indicators:

* Green: RRI ≥ 80% (Healthy)
* Amber: 60% ≤ RRI < 80% (Caution)
* Red: RRI < 60% (Warning)

### 4. Interpretation:

Identifying Bottlenecks: A low RRI (red/amber) may indicate bottlenecks in the review process due to:

* Reviewer Availability: Not enough reviewers to handle the workload, leading to backlogs.
* Unbalanced Workload: Certain reviewers might be overloaded, causing delays for their assigned PRs.
* Notification Issues: Reviewers might not be receiving timely notifications about assigned PRs.

Gauging Team Responsiveness: A high RRI (green) suggests quick feedback loops and efficient collaboration, which can promote faster development cycles.

### 5. Key Points:

* Improved Workflow: Monitoring RRI helps identify and address bottlenecks, leading to a more efficient code review process.
* Faster Development Cycles: High RRI indicates quick turnaround times for PR reviews, which can accelerate development cycles.
* Collaboration & Responsiveness: RRI provides insights into the overall responsiveness of your review team, fostering a culture of timely communication and collaboration.

### 6. Conclusion:

Monitoring RRI provides valuable insights into the effectiveness of your code review process. By analyzing the distribution and taking corrective actions when necessary, you can identify bottlenecks, improve reviewer responsiveness, and ultimately deliver software faster.

Related Metrics:

* PR Merged without Review
* PR Review Time
* Reviewer Distribution

Additional Considerations:

* Track changes in RRI over time to assess the effectiveness of implemented improvements.
* Analyze RRI distribution by factors like PR complexity, reviewer, and time of day to pinpoint specific issues.
