# Web Scrape with Python in 4 minutes

## Web Scraping
Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort. In this article, we will go through an easy example of how to automate downloading hundreds of files from the New York MTA. This is a great exercise for web scraping beginners who are looking to understand how to web scrape. Web scraping can be slightly intimidating, so this tutorial will break down the process of how to go about the process.

# what is webs craping

**Web scraping, web harvesting, or web data extraction** is data scraping used for extracting data from websites. Web scraping software may directly access the World Wide Web using the Hypertext Transfer Protocol or a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

# How to scrape websites without getting blocked

## Web Scraping best practices to follow to scrape without getting blocked

- **Respect Robots.txt :**  Web spiders should ideally follow the robot.txt file for a website while scraping. It has specific rules for good behavior, such as how frequently you can scrape, which pages allow scraping, and which ones you can’t.

- **Make the crawling slower, do not slam the server, treat websites nicely**

- **Do not follow the same crawling pattern :** Humans generally will not perform repetitive tasks as they browse through a site with random actions.

- **Make requests through Proxies and rotate them as needed :** When scraping, your IP address can be seen. A site will know what you are doing and if you are collecting data. They could take data such as – user patterns or experience if they are first-time users.

- **Rotate User Agents and corresponding HTTP Request Headers between requests :** A user agent is a tool that tells the server which web browser is being used. If the user agent is not set, websites won’t let you view content. Every request made from a web browser contains a user-agent header and using the same user-agent consistently leads to the detection of a bot.