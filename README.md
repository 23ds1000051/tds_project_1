#### GitHub User & Repository Scraper

This project is designed to gather detailed insights into GitHub users and their repositories, focusing on specific metrics such as location, follower count, programming languages, licenses, and popularity trends. Leveraging the GitHub API, it highlights key data points and trends among a defined user group.

### Key Insights:

Data Collection Methodology
Data was scraped from the GitHub API, specifically targeting users from Hyderabad with at least 50 followers. For each user, additional API calls gathered comprehensive profile and repository information. Pagination ensured data completeness, retrieving up to 500 repositories per user.

### Interesting and Surprising Findings:

Licensing Trends: Despite the popularity of JavaScript, the MIT license dominated among repositories, suggesting a preference within the open-source community for permissive licensing.
Visibility and Hireability: Surprisingly, many highly-followed users are not marked as “hireable,” despite their potential visibility and influence within the GitHub community.
Actionable Recommendations for Developers
To increase their impact, developers might consider contributing to repositories with high star counts and permissive licenses (such as MIT) for greater visibility.

### Top Insights from the Dataset:

Key Users: 
Top 5 Users by Followers in Hyderabad: iam-veeramalla, in28minutes, stacksimplify, thenaveensaggam, MadhavBahl
Earliest Registered GitHub Users in Hyderabad: shabda, sitaramc, bagwanpankaj, srikanthlogic, kulbirsaini
Popularity and Language Trends
Most Common Licenses: MIT License, Apache License 2.0, Other
Most Common Company: IIIT Hyderabad
Most Popular Programming Language: JavaScript
Second Most Popular Language Among Post-2020 Joiners: HTML
Language with Highest Average Stars per Repository: Perl
Leader Strength & Correlations
Top 5 Users by Leader Strength: in28minutes, iam-veeramalla, stacksimplify, ashokitschool, thenaveensaggam
Correlation Between Followers and Public Repositories: 0.006
Estimated Follower Gain per Additional Repository: 0.063 followers
Additional Insights
Most Active Repository Creators on Weekends: hemanth22, anjijava16, wahid Khan74, elevenpassin, Shekharrajak
Most Common Surname: Kumar

### Output Files:

The data collected is stored in two CSV files:

users.csv: Contains profile details such as login, name, company, location, email, hireable status, bio, public repos, followers, following, and creation date.
repositories.csv: Contains repository details including login, full name, creation date, stargazers count, watchers count, language, project and wiki status, and license name.

### Usage
The files include Souce Code.
Generate CSV Files: Run the Python code in the repository to generate users.csv and repositories.csv.
Customize Data Collection: Use your GitHub API key to set different locations or follower thresholds.
This GitHub User & Repository Scraper provides a unique view of developer profiles and project preferences, helping you understand community trends and align your projects for greater impact and visibility.
