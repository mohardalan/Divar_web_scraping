# Tehran Apartment Price Estimation

## Overview

This project aims to estimate the prices of apartments in Tehran, Iran, by utilizing web scraping and a simple linear regression model. We collect apartment data from the "divar.ir" website and apply data analysis and machine learning techniques to predict apartment prices based on various features.

## Project Details

### Web Scraping

To obtain apartment data from the "divar.ir" website, we employ a web scraping approach. This website displays a limited number of posts (24) on each page, making traditional scraping methods insufficient. To address this limitation, we utilize a technique demonstrated in [this video](https://www.youtube.com/watch?v=atpc1fmPuhY).

1. We create requests to the website's API to retrieve "tokens" associated with each post, considering specific search parameters and post-publication dates.
2. With the list of tokens in hand, we proceed to scrape the website for apartment features.

### Web Scraping with Selenium

The "divar.ir" website employs JavaScript to load post data instead of using standard HTML and CSS formats. This necessitates the use of the "Selenium WebDriver" for web scraping. Selenium allows us to navigate the website, interact with elements, and retrieve data effectively.

### Data Processing and Storage

Once the data is scraped, we organize it into a structured format using Python. We then save this structured data as a 'CSV' file for further analysis.

### Machine Learning Model

To estimate apartment prices in Tehran, we implement a simple linear regression model on the CSV dataset. Given that the data is in the Persian language, we perform data cleaning and preprocessing to make it suitable for machine learning. We split the dataset into training and test sets and train the regression model.

## Requirements

- Python 3.x
- Selenium WebDriver
- Pandas
- Scikit-Learn
- Other necessary dependencies (requirements specified in the project's files)

## Usage

1. Clone this repository to your local machine.
2. Install the required dependencies listed in the project's files.
3. Run the provided scripts to scrape data, process it, and train the linear regression model.
4. Use the model to estimate apartment prices in Tehran based on your data.

## Contribution

Contributions to this project are welcome. Please fork the repository, make your improvements, and submit a pull request. Make sure to follow the project's code of conduct.

## Acknowledgments

- The method demonstrated in [this video](https://www.youtube.com/watch?v=atpc1fmPuhY) was a key reference in our web scraping approach.
