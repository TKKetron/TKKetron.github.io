---
title: "Web scraper"
excerpt: "A web scraper that went to a desired website and gathered relevant information and saved it to a JSON file when there was no API to be used"
collection: portfolio
---

This was a simple web-scraper in c# using Selenium. I chose to use the Selenium chrome version because it was well documented. This we scraper was very crude and pulled the raw HTML from various sites and even interacted with the elements on screen to allow the java script in hte background of websites to update the page. For instance it would search for data that may not change the URL but would update the contents of the page then perform string manipulation to store that data in a readable format for either myself or other programs like my [DND program](https://tkketron.github.io/portfolio/DnD-Done-Right/) to read from. Check out the source code [HERE](https://github.com/TKKetron/Web-Scraper/tree/master).