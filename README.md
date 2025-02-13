# Predicting Tomato Prices from Web-Scraped Data

## Project Overview
This project focuses on developing a **web scraper** to extract tomato price data from the **Agmarknet** website and using an **XGBoost (XGB) model** to predict modal prices for different locations.

## Data Source
**URL Scraped:** [Agmarknet Tomato Prices](https://agmarknet.gov.in/SearchCmmMkt.aspx?Tx_Commodity=78&Tx_State=0&Tx_District=0&Tx_Market=0&DateFrom=30-Jun-2020&DateTo=30-Jun-2020&Fr_Date=30-Jun-2020&To_Date=30-Jun-2020&Tx_Trend=0&Tx_CommodityHead=Tomato&Tx_StateHead=--Select--&Tx_DistrictHead=--Select--&Tx_MarketHead=--Select--)

The web scraper extracts tomato price data for **Karnataka** from **Jan 1, 2015, to Feb 1, 2021**, and stores it in a CSV file.

## Implementation
1. **Web Scraper**: Uses **Selenium** and **webdriver-manager** to scrape tabular data from Agmarknet.
2. **Data Processing & Model Training**:
   - The extracted data is stored in **Agri_data.csv**.
   - An **XGB model** is trained on Google Colab to predict modal prices.

## Dependencies
- **Web Scraping**: `selenium`, `webdriver-manager`
- **ML & Data Processing**: `numpy`, `pandas`, `train_test_split`, `GridSearchCV`, `XGBoost`

## Execution Steps
- The **web scraper** is executed locally as Selenium requires a web browser.
- The **XGB model** is trained on **Google Colab** after uploading the scraped CSV file.

## Files
- **`web-scraper.ipynb`**: Code for web scraping.
- **`xgb_model.ipynb`**: Code for training the XGB model.
- **`Agri_data.csv`**: Web scraped agricultural data.
- **`output.csv`**: Predicted and actual modal prices.

## Author
**Aditya Mishra**  
For inquiries, contact: **@eddyy2612**

