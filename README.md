# Web Scraping

As a Data Engineer, we need to write a lot of ETL pipeline. ETL process consists of three steps - extract, transform, and load. 
Extract part of the ETL process, which can be done using different methods like extracting data from API, analytics, or web scraping.
This repo shows one of the ways to extract data and build a dataset by using web scraping techniques.

## Goal

The goal is to scrape product information from Amazon for a search query on Xbox consoles and store it in a CSV file format for further analysis.

## Understanding Web Scraping Process

Each and every line is explained about how one can scrape from any of the authorized sites in the file mentioned below:
> understanding_amazon_web_scraping_process.ipynb

## Amazon Web Scraping Final

It contains a Python script that extracts product information from Amazon.com for a search query for "xbox consoles".

The script uses the BeautifulSoup library to parse the HTML content of the webpage and extract information about each product. Specifically, it uses functions to extract the title, price, rating, number of user reviews, and availability status for each product.

The script then loops through each product link on the search results page, retrieves the product information by calling the functions, and stores it in a dictionary. Finally, it converts the dictionary to a Pandas DataFrame, cleans the data by removing any rows with missing product titles, and saves the cleaned DataFrame to a CSV file called "amazon_data.csv".

Note that the __user agent__ in the script is left empty, so you will need to fill in your own user agent to avoid getting blocked by Amazon's anti-scraping measures.

## To get User Agent:

Click on [User agent](https://www.whatismybrowser.com/detect/) and select "What is my user agent?" under "Detect Web Browser" section
