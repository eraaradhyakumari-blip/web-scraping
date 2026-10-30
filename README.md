# Quotes Web Scraping Project

## Project Overview
This project is a Python-based web scraping application that extracts quotes from [Quotes to Scrape](https://quotes.toscrape.com/). It uses the Requests library to fetch webpage content and BeautifulSoup to parse HTML data.

The project automatically visits multiple pages and saves the HTML content of each page into separate files.

## Objectives
- Learn the fundamentals of web scraping using Python.
- Fetch webpage data using the Requests library.
- Parse HTML content using BeautifulSoup.
- Extract quote information from multiple pages.
- Store scraped HTML files locally.

## Technologies Used
- **Python** – Programming language.
- **Requests** – Fetch webpage content.
- **BeautifulSoup** – Parse and extract HTML elements.
- **OS Module** – Create directories and manage files.
- **Jupyter Notebook / VS Code** – Development environment.

## Project Structure

```text
Quotes-Web-Scraping/
│
├── scraped_data/
│   ├── quotes1.html
│   ├── quotes2.html
│   ├── quotes3.html
│   └── ...
│
├── quotes_scraper.py
└── README.md
```

## Installation and Setup

### Step 1: Install Python Libraries

```bash
pip install requests beautifulsoup4
```

### Step 2: Import Required Libraries

```python
import requests
from bs4 import BeautifulSoup
import os
```

### Step 3: Run the Project

```bash
python3 quotes_scraper.py
```

## How It Works

1. The program starts scraping from page 1.
2. Requests fetches the HTML content from the website.
3. BeautifulSoup parses the HTML document.
4. The program searches for quote elements using the CSS selector `div.quote`.
5. If no quotes are found, the loop stops.
6. Each valid webpage is saved as a separate HTML file inside the `scraped_data` folder.
7. The page counter increases automatically.

## Expected Output

```text
Downloaded data from page 1
Downloaded data from page 2
Downloaded data from page 3
Downloaded data from page 4
...
Downloaded data from page 10
No valid pages anymore...
```

## Output Files

The scraped HTML files are stored in the `scraped_data` directory.

Example:
- quotes1.html
- quotes2.html
- quotes3.html
- quotes4.html

## Learning Outcomes

After completing this project, I learned:

- Web scraping fundamentals.
- HTTP requests and responses.
- HTML parsing and CSS selectors.
- Python loops and conditional statements.
- File handling and directory management.
- Automating data collection from multiple webpages.

## Future Improvements

- Extract individual quotes and author names.
- Save extracted data in CSV and Excel formats.
- Remove duplicate quotes.
- Add error handling for failed HTTP requests.
- Build a dashboard using Streamlit.

## Author

**Aaradhya Kumari**

Python Developer | Web Scraping Learner

## Project Status

Completed – Basic Multi-Page Web Scraping Project.
