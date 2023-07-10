# nosql_challenge

Background
--------
Extract information from the [Mars News Website](https://static.bc-edx.com/data/web/mars_news/index.html) and the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html) via both automated browsing with Splinter and HTML parsing with Beautiful Soup. Analyze the data extracted and save it to a CSV file. 

## Objective ##
#### Part 1: Scrape Titles and Preview Text from Mars News ####
- Use automated browsing to visit the [Mars News Website](https://static.bc-edx.com/data/web/mars_news/index.html). 
- Create a Beautiful Soup object and use it to extract text elements from the website.
- Extract the titles and preview text of the news articles that were scraped. Store the scraping results in Python data structures as follows:
  - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: `title` and `preview`.
  - Store all the dictionaries in a Python list.
  - Print the list in the notebook.

#### Part 2: Scrape and Analyze Mars Weather Data ####
