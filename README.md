##  Wuzzuf Employment Search Scraper
This project is a web scraper built using Python's requests and BeautifulSoup libraries to extract job listings from Wuzzuf, a popular employment search platform.

##  Getting Started
To use this scraper, make sure you have Python installed on your system. You can install the required libraries using pip

##  Implementation
Run the wuzzuf_scraper.py script.
The script will fetch job listings from Wuzzuf based on the provided search query (e.g., Python).
It extracts job titles, company names, job locations, job requirements, and job links.
The extracted data is saved to an Excel file named company_names.xlsx on the desktop.

Sample code
# Importing Lbraries
import requests
from bs4 import BeautifulSoup
import pandas as pd

# Fetching the URL
result = requests.get("https://wuzzuf.net/search/jobs/?q=python&a=hpb")

# Parsing the HTML content
src = result.content
soup = BeautifulSoup(src, 'lxml')
See code for codes.
