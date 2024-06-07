# Reviewer Distribution

### Reviewer Distribution

### 1. Introduction:

This document explains how to analyze and visualize reviewer participation in your code review process using the Reviewer Distribution metric. It's presented as a Pareto chart, ranking reviewers by the number of reviews conducted and showing the cumulative percentage of the total reviews.

This metric provides valuable insights into ensuring balanced participation among team members and mitigating risks associated with reviewer workload and knowledge distribution.

### 2. Definitions:

* Reviewer: Team members who are authorized to conduct code review for Pull Requests (PRs).
* Review: A single instance of a code review completed on a Pull Request.
* Pull request approved with feedback: PRs that reviewers have commented on at least once.
* Pull request approved without feedback: PRs that do not have any comment by reviewers.
* Total Members: The total number of team members added to the team(s) where code reviews are conducted.

### 3. Explanation of Charts:

KPI Card:

\
![](https://lh7-us.googleusercontent.com/docsz/AD\_4nXeAYReM7dbC\_s80crR8qp3tVjv1ySdDvWqjuj5\_Z2alFyQgjcK0akywooVaBC-6WxSRjtcF5F4FhLDOOYYxxz1NLCssxpRgRs-KxOckil\_JHFB4dKkUqyPT2VO9-xsYXAsYRieWWHsY79ofTXf13P4M\_O6O?key=xtdLPyiyKjFJ1GiTLEmLYg)

Detailed Chart:

<figure><img src="https://lh7-us.googleusercontent.com/docsz/AD_4nXd5p1yE9vNQulXhI-E_mpRu34PQ2FBasGvQVEntbAd376q1KHQK4s147JeeXR0ZftsfT98ENTatB3dOlYUeMjKZSx9Vyt7DGtQCv_KcaFqNta4o4aIQSEnMwLPqWiy1kmmFpbMN53enUta34JAX-bXYz6c?key=xtdLPyiyKjFJ1GiTLEmLYg" alt=""><figcaption></figcaption></figure>

The Pareto Chart displays the distribution of code review participation among team members.

* Vertical Axis: Represents individual reviewers ranked by the number of reviews conducted (highest to lowest).
* Horizontal Axis: Represents the cumulative percentage of total reviews completed.
* Blue bar: PRs Approved without feedback&#x20;
* Yellow Bar: PRs Approved with feedback&#x20;
* Red Line: Cumulative Percentage PRs Reviewed&#x20;
* Tooltips: Hovering over a data point reveals additional information:

Color Indicators:

* Green: 45% of reviewers or more are actively participating.
* Amber: Less than 45% but equal to or more than 30% of reviewers are participating.
* Red: Less than 30% of reviewers are actively participating.

### 4. Interpretation:

Identifying Trends: The Pareto chart helps visualize the distribution of code review participation over time.

* Uneven Distribution (Red/Amber): This may indicate a small group of reviewers are handling a disproportionate workload, potentially leading to fatigue, knowledge silos, and bottlenecks.
* Balanced Distribution (Green): This suggests reviews are spread relatively evenly among a moderate number of reviewers, promoting knowledge sharing and process efficiency.

### 5. Key Points:

* Balanced Participation: Monitoring Reviewer Distribution ensures all team members contribute to the code review process, mitigating risks associated with reviewer overload and knowledge concentration.
* Knowledge Sharing: Identifying reviewers with high participation helps understand where expertise lies and can inform knowledge sharing initiatives.
* Targeted Training: Reviewer Distribution data can be used to identify team members who might benefit from additional review training, promoting wider participation.

### 6. Conclusion:

Monitoring Reviewer Distribution using a Pareto chart provides valuable insights into the health of your code review process. By analyzing the distribution and taking corrective actions when necessary, you can ensure balanced participation, promote knowledge sharing, and ultimately deliver higher quality software.

Related Metrics:

* Quality: Bug Open count, Review Time, Cycle Time, Review Responsiveness, Review Completion

### Additional Considerations:

* Track changes in the distribution over time to identify trends and assess the effectiveness of implemented initiatives.
* Conduct regular analysis to understand the reasons behind review concentration and identify specific solutions.
