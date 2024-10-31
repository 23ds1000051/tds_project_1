## GitHub User & Repository Scraper

This project gathers detailed insights into GitHub users and their repositories, focusing on critical metrics like location, follower count, programming languages, licensing, and popularity trends. Using the GitHub API, it reveals key data points and trends among a targeted user group.

### Key Highlights
#### Efficient Data Collection: 
Data was systematically gathered from the GitHub API, targeting users located in Hyderabad with over 50 followers. To ensure comprehensive insights, the collection process included multiple stages:

  - User Filtering and Selection: Using location filters and follower thresholds, we initially narrowed down users     specifically from Hyderabad with at least 50 followers. This refined selection allowed for an analysis of the      more active and potentially influential users in this region.
  - Detailed Profile Retrieval: For each user in our target group, we performed additional API requests to gather      extensive profile details, including bio, company affiliation, email (if available), and account creation          date. This allowed for an in-depth look at the professional backgrounds and career trajectories within this        user subset.
  - Repository-Level Insights: Each selected user's repositories were then retrieved with pagination, ensuring up      to 500 repositories per user. This approach captured repository-specific data such as programming language,        license type, star count, and project visibility, helping identify trends in popular languages, licensing          choices, and project scale.

Data Completeness and Quality: By structuring the collection process to use pagination and limit the number of requests, we ensured data completeness while respecting API rate limits. This method provided a holistic view of both individual user profiles and broader repository metrics without sacrificing data quality.
This structured, multi-stage approach ensured that we captured both high-level and granular insights, allowing us to uncover significant trends and actionable data on GitHub’s developer community in Hyderabad.

#### Surprising Findings: 
Despite JavaScript's popularity, the MIT license leads as the most common, signaling a preference for permissive licensing. Additionally, many popular users are not marked as "hireable," despite high visibility in the community.

#### Developer Recommendation: 
Developers aiming to increase impact should consider contributing to repositories with high star counts under permissive licenses like MIT for broader visibility.

### Project Overview

### Data Collection Methodology
Data was scraped using the GitHub API, selecting users in Hyderabad with at least 50 followers. For each user, additional API calls gathered detailed profile and repository data. Pagination ensured data completeness, retrieving up to 500 repositories per user. The code to collect data is provided in the files. Try your desired location.

### Key Insights and Interesting Findings
Licensing Trends: The MIT license dominates among repositories, even with the popularity of JavaScript, indicating a community preference for permissive licensing.
Visibility and Hireability: A surprising number of highly-followed users are not marked as “hireable,” suggesting that user visibility doesn't always equate to availability for hiring.
Actionable Recommendation
Developers looking to increase visibility should contribute to well-starred repositories with permissive licenses (e.g., MIT) to gain more traction within the community.

### Top Insights from the Dataset

#### Notable Users and Trends:

Top 5 Users by Followers in Hyderabad: iam-veeramalla, in28minutes, stacksimplify, thenaveensaggam, MadhavBahl
Earliest Registered GitHub Users in Hyderabad: shabda, sitaramc, bagwanpankaj, srikanthlogic, kulbirsaini
Licensing Preferences: MIT License, Apache License 2.0, and Other
Most Common Company: IIIT Hyderabad
Most Popular Programming Language: JavaScript
Post-2020 Language Popularity: HTML
Highest Average Stars per Repository: Perl
Leader Strength and Influences:

Top 5 Leaders by Influence: in28minutes, iam-veeramalla, stacksimplify, ashokitschool, thenaveensaggam
Correlation Insight: Minimal correlation (0.006) between followers and public repositories, with an estimated gain of 0.063 followers per additional repository.
Additional Findings:

Weekend Repository Creators: hemanth22, anjijava16, wahid Khan74, elevenpassin, Shekharrajak
Most Common Surname: Kumar
Output Files

### The data collected is saved in two CSV files:

users.csv: Contains user details like login, name, company, location, email, hireable status, bio, public repos, followers, following, and account creation date.
repositories.csv: Includes repository details such as login, repository name, creation date, star count, watcher count, language, project status, and license.

### Usage

Generate CSV Files: Execute the Python code in this repository to produce users.csv and repositories.csv.
Customize Data Collection: Use a GitHub API key to adjust location or follower thresholds as needed.
The GitHub User & Repository Scraper offers a unique perspective into developer profiles and project preferences, helping align your projects with community trends for greater visibility and impact.
