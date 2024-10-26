# tds_project_1
# GitHub User & Repository Scraper

This project collects detailed information about GitHub users and their repositories using GitHub’s API, focusing on metrics like location, followers, repository languages, licenses, and popularity. 

### Key Insights
- **How the Data was Scraped**:  
  Data was collected by querying the GitHub API based on location (Hyderabad) and minimum followers (50). For each user found, additional API calls retrieved details about their profiles and repositories, such as followers, programming languages, and license types. Pagination ensured all available data (up to 500 repositories) was retrieved.  

- **Interesting and Surprising Fact**:  
  Despite JavaScript’s popularity among the repositories, the **MIT license** emerged as the most used license, indicating a strong preference in the open-source community for permissive licensing. Additionally, many users with large follower counts are not marked as "hireable," which is surprising given their visibility and potential influence.

- **Actionable Recommendation for Developers**:  
  Developers looking to increase their impact should consider contributing to repositories with high star counts and permissive licenses (like MIT) to increase visibility.

---

Two CSV files are generated as output:

### **1. users.csv**  
This file contains the following columns:  
- `login`  
- `name`  
- `company`  
- `location`  
- `email`  
- `hireable`  
- `bio`  
- `public_repos`  
- `followers`  
- `following`  
- `created_at`  

---

### **2. repositories.csv**  
This file lists repositories with the following columns:  
- `login`  
- `full_name`  
- `created_at`  
- `stargazers_count`  
- `watchers_count`  
- `language`  
- `has_projects`  
- `has_wiki`  
- `license_name`  

---

### Usage:

Generate CSV Files: The included Python code allows you to generate the users.csv and repositories.csv files.
Customize Location and Followers: By providing a GitHub API key, you can collect data for your desired location and followers threshold.

