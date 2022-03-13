# SEC-EDGAR-web-scraper
# About this project 

   This code is forked from https://github.com/galibin24/SEC-EDGAR-python-scraper. The project automates the retrieval of web-based financial data by scraping the SEC-EDGAR site. Users can pull data by ticker symbol (i.e. TSLA, MSFT, AAPL) and year, and automatically sort the data.
   
   Currently, the scraper is fully functional, utilizing the scrapy library. It will retrieve and organize data from 2021 to the current date.
   
# Labeling & Aggregation

   The labeling script (Label.py) analyzes the document type and stores to the "parsed" folder. 

   The aggregation script (Aggregate.py) is in the early stages, with the goal of labeling scraped/parsed data.
   
## Getting Started
   1. Copy the repository by either (a) downloading the code:
      ```
      Download ZIP
      ```, then extract all files to your desired path for the project.
         OR using HTTPS, copy the web URL:
         ```
         https://github.com/galibin24/SEC-EDGAR-python-scraper.git
         ```
         b. Open the Command Prompt (for Windows):
         ```
         Windows Key + X
         ```.
         c. Change directory to navigate to where you want to clone the repo:
         ```
         cd /some/path/to/folder
         ```.
         d. Clone the repo into the desired location:
         ```
         git clone https://github.com/galibin24/SEC-EDGAR-python-scraper.git
         ```.
         3. Change directory to the project folder:
         ```
         cd /some/path/to/folder/SEC-EDGAR-python-scraper
         ```.
      
   2. Install the required packages for the project from the requirements.txt file using pip. From the Command Prompt (for Windows), in the location of the project/code (either downloaded or where you just cloned the repo) run:
      ```
         pip install -r requirements.txt
      ```.
   3. Retrieve financial data from SEC-EDGAR by running the scraper.py script: 
      ```
         python scrape.py
      ```.
   4. Get desired company information. You will be promted to enter the ticker symbol(s) of interest (i.e. "TSLA, AAPL):
      ```
      Enter tickers: TSLA, AAPL
      ```, and press enter.
   5. Select the years for data you want for those companies. You will be prompted again:
      ```
      Enter from which year to start: YYYY
      ```.
   6. View scraped data by accessing the "files" folder:
      ```
      cd /files
      ```.   
   7. To label (or re-name) all the scraped files in the "files" folder run label.py script:
      ```
      python label.py
      ```.

## Contribution
I am actively seeking contributors to improve efficiency, structure and functionality.

## License

This project is licensed under the terms of the MIT license.

"# SEC-EDGAR-python-scraper" 

## Future Enhancements
This project functions to retrieve historical financial data for companies from 2021 to the current date, and then re-name these files in the "files" folder. Additional features will be added to the project to enhance functionality, including:
1. Pull all historical data for a company (starting with the first year of availability in SEC-EDGAR database).
2. Analyze financial data using various metrics for time series data (i.e. moving averages).
3. Pull historical and current stock pricing data using the Yahoo Finance (or another finance) API. This will include open, high, low, close, and adjusted close prices on a daily basis.
4. Visualize financial data over time using various metrics (i.e. dual bar and line chart showing Adjusted Close prices, moving averages, and volume over time). 
5. Add a UI through a web-application framework and visualization package (i.e. Django, Plotly/Dash). 
6. Build a database to allow users to store companies by ticker symbols, to track financial progress by building a portfolio or watch list. This will be a feature of the web-application, using SQL.
7. Apply Machine-Learning methods to build basic trading strategies to provide potential guidance to investors (ie. BUY, HOLD, SELL). 

## Disclaimer
I am NOT a Certified Public Accountant (CPA), certified financial planner/advisor, certified financial analyst, or lawyer. However, I am a CPA Candidate (passed REG, AUD) with two sections remaining, on track to get my license by 07/2022. Further, I have 10+ years experience as a profesional accountant/financial analyst, and formal training in accounting (with a professional certificate of Accountancy from the University of Louisville). Currently, I work as a Senior Data Scientist building analytics/visualization tools using global financial/accounting data. 

As such, the contents of the repo are an opinion, for informational and entertainment purposes only, and do not constitute financial, accounting, or legal advice. It is important to do your own research, and seek a licensed professional for financial/investment advice.