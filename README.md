# glassdoor_job_scraper
Python script leveraging Selenium for job seekers looking for WFH roles from top Work-life companies. Based on criteria, will mass pull roles that you can consider applying for without having to dig around Glassdoor.

## Process
The glassdoor job scraper follows a three piece scraping process:
I. Company Scrape
    The first step is to pull companies that have a top work-life balance for a role you are interested in. For example, pull companies with a work-life balance >= 3.5 stars for Analyst roles. This scrape will pull a max of ~9,900 companies as Glassdoor has a bug that doesn't show more companies after page 1,000 on the company explore section of the site.

II. Job Scrape from pulled companies
    From each of the companies scraped, the scraper will go to their company site and pull their current job openings. A call out here is that if the company has more than 40 job openings, only the first 40 jobs will be pulled as glassdoor limits the amount of jobs shown on the company profile page.

III. Examine jobs scraped and filter out those that don't fit your search criteria and see which of those are open to WFH policy.


