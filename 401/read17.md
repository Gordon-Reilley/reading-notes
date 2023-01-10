# Web Scraping

## How to Web Scrape with Python in 4 Minutes

- Web scraping is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.
- **Important notes about web scraping:**
  - Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.
  - Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.
- The first thing that we need to do is to figure out where we can locate the links to the files we want to download inside the multiple levels of HTML tags. Simply put, there is a lot of code on a website page and we want to find the relevant pieces of code that contains our data.
- On the website, right click and click on “Inspect”. This allows you to see the raw code behind the site.
- Notice that on the top left of the console, there is an arrow symbol.
- If you click on this arrow and then click on an area of the site itself, the code for that particular item will be highlighted in the console.
- Notice that all the .txt files are inside the `<a>` tag following the line above. As you do more web scraping, you will find that the `<a>` is used for hyperlinks.

## Web scraping - Wiki

- Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.
- Web scraping software may directly access the World Wide Web using the Hypertext Transfer Protocol or a web browser.
- While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.
- Scraping a web page involves fetching it and extracting from it. Fetching is the downloading of a page (which a browser does when a user views a page). Therefore, web crawling is a main component of web scraping, to fetch pages for later processing. Once fetched, extraction can take place. The content of a page may be parsed, searched and reformatted, and its data copied into a spreadsheet or loaded into a database. 
- As well as contact scraping, web scraping is used as a component of applications used for web indexing, web mining and data mining, online price change monitoring and price comparison, product review scraping (to watch the competition), gathering real estate listings, weather data monitoring, website change detection, research, tracking online presence and reputation, web mashup, and web data integration.
- Web pages are built using text-based mark-up languages (HTML and XHTML), and frequently contain a wealth of useful data in text form. However, most web pages are designed for human end-users and not for ease of automated use. As a result, specialized tools and software have been developed to facilitate the scraping of web pages.
- Newer forms of web scraping involve monitoring data feeds from web servers. For example, JSON is commonly used as a transport storage mechanism between the client and the web server.
- There are methods that some websites use to prevent web scraping, such as detecting and disallowing bots from crawling (viewing) their pages. In response, there are web scraping systems that rely on using techniques in DOM parsing, computer vision and natural language processing to simulate human browsing to enable gathering web page content for offline parsing.

## How to Scrape Websites Without Getting Blocked

- Web scraping is a task that has to be performed responsibly so that it does not have a detrimental effect on the sites being scraped. 
- Web Crawlers can retrieve data much quicker, in greater depth than humans, so bad scraping practices can have some impact on the performance of the site. While most websites may not have anti-scraping mechanisms, some sites use measures that can lead to web scraping getting blocked, because they do not believe in open data access.
- If a crawler performs multiple requests per second and downloads large files, an under-powered server would have a hard time keeping up with requests from multiple crawlers.
- Since web crawlers, scrapers or spiders (words used interchangeably) don’t really drive human website traffic and seemingly affect the performance of the site, some site administrators do not like spiders and try to block their access.
- Web spiders should ideally follow the **robot.txt** file for a website while scraping. It has specific rules for good behavior, such as how frequently you can scrape, which pages allow scraping, and which ones you can’t.
- **Here are a few easy giveaways that you are bot/scraper/crawler**
  - Scraping too fast and too many pages, faster than a human ever can
  - Following the same pattern while crawling. For example – go through all pages of search results, and go to each result only after grabbing links to them. No human ever does that.
  - Too many requests from the same IP address in a very short time
  - Not identifying as a popular browser. You can do this by specifying a ‘User-Agent’.
  - using a user agent string of a very old browser
### Things I want to know more about
- I'd like to do more research on how to grab on the proper practices for web scraping, so I won't run the risk of getting blocked or breaking a site by accident.
### Sources

- <https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460>
- <https://en.wikipedia.org/wiki/Web_scraping>
- <https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/>

[Back To Home](../README.md)