## What is this?
This is just my notes for scrapy, its web scraping methods, best practices and proxy.

## Compare to beatiful soup and selenium
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


## Setup virtual enviornment and scrapy
Since I only use windows, this notes will focus on windows.

first, install python, pip and virtual enviornment, after that, check the version in vscode
```
python --version
pip --version
```
for installing virtual enviornment, use
```
pip install virtualenv
```

# What is virtual enviornment?
It is like a folder that exists on top of python,
where you can add modules into the project, and it only stays in the project.

why should we do this?
because if we have multiple projects, and uses the same modules but different version of it,
it might be troublesome to upgrade, and it might conflict with each other.

# Set up a virtual enviornment

```
pip install virtualenv
```
then Navigate to the folder where you want to create the virtual environment, and run the virtualenv command.
```
cd /folder
virtualenv venv .
```
The "dot" in the above command indicate you want to install virtualenv on this folder,
you can also change the directory before installing it.

After that, run the following script to activate the virtual enviornment
```
.\scripts\activate
```
Successfully activate will result in a bracket () around the folder name.
you can now install any modules for your project that only belongs to this main folder.

# Installing Scrapy
```
pip install scrapy
```
To check if its successfully installed, just type scrapy into the terminal, and you should see a list of commands.
