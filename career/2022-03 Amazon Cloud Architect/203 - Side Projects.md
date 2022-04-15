---
created: 2022-03-14T22:48:25-06:00
updated: 2022-03-14T22:48:25-06:00
---
# 203 - Side Projects


## eqbank Download to Quicken & QuickBooks Online
*Work in progress*
- Either manipulate CSV download (painful for many accounts), or,
- Use the eqbank.ca API
	- Captured with Firefox Network console
	- Pasted into Insomnia HTTP Debugger/Client/Tester
		- Open Source Postman alternative)
	- Working on JSON
	- Manually pasting token from new logins into Insomnia params to get around 2FA, otherwise I'd use the login to get a token automatically.
- Automate CSV Download with TestCafe E2E Testing Utility

## MS Power BI Connector for Moodle (Open Source soon!)
- I wanted to see more data on my son's progress through school.
- Grade 7, COVID-19 year-one at home.
- Moodle webpages were inconsistent across courses.
- More data should have been available.
- Tried a Cypress e2e test to scrape data, then saw the problem.
- Upgraded to using Moodle Mobile Web Services
	- built-into Moodle, no extra settings, service, third party, etc.
- GitHub Repo structured, an documented, with using the package as a lab in school. Imagine, kids creating their own dashboards to see their grades! Hello little data scientists...
