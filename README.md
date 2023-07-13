# What is this?
This is just my notes for scrapy, its web scraping methods, best practices and proxy.

# Compare to beatiful soup and selenium
Beautiful soup is good for small scale web scraping application where the data you want is returned in the html response.
However, for manage concurrency, retries, data cleaning, data storage etc, scrapy is a much better choice.

For selenium, it is good if you want to interact with the webpage elements to get the data, or if the site only returns the data
you want after the javascript has rendered.

Compared to the above two options, scrapy allows you to do the following:
- It can select CSS and parse XPath expressions
- do data formatting and store them, for example CSV, JSON, XML
- Automatic retries
- Cookies and session handling
- Robust encoding support
- concurrency management
- crawl spiders and in-built pagination support


# Setup virtual enviornment and scrapy

