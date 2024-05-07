## Stock Project - 1)
The code automates the process of collecting and processing financial data from Naver Finance and KRX to rank companies based on financial indicators. It utilizes web scraping, data manipulation, and analysis techniques.

### Connecting Categories to Company Names and Company Codes:
 - Connects to the sector classification site of Naver Finance to retrieve sector categories and company names.
 - Utilizes company codes provided by the Korea Exchange to obtain company names and codes.
 - Merges the retrieved category-company names with company names and codes to create a dataframe containing category, company name, and company code.

### Fetching Financial Information for Each Company:
 - Retrieves annual financial statements data for each company from Naver Finance.
 - Processes the retrieved financial statements data to extract information such as net profit ratio, ROE, debt ratio, and PER.
 - Saves the extracted financial information for each company into separate files.

### Processing Financial Statements:
 - Combines the fetched financial information into a single dataframe.
 - Removes unnecessary data and standardizes column names.

### Utilizing the Data:
 - Merges the company category data with the financial statement data to create a single dataframe.
 - Processes the data by removing unnecessary whitespace and standardizing data types.
 - Ranks the data and calculates the overall rank, then sorts and saves the data based on the overall rank.

## Stock Project - 2)
This code collects news headline data from the Naver News website for specific categories (Finance, Securities, Industry/Business, SME/Venture) and processes the data to extract hot keywords.

### Getting News Headline Data:
 - Using Selenium and BeautifulSoup, it retrieves news headlines from a specified date on the Naver News webpage.
 - It navigates to the respective category URL and retrieves news headlines page by page.
 - The collected news headlines are converted into a dataframe and saved as a CSV file.

### Processing News Headline Data:
 - It extracts nouns from the collected news headlines.
 - For each category, it aggregates the extracted nouns into a single list.
 - Filters out words with a length of less than 2 characters.
 - Removes unnecessary words and selects the top 200 keywords.
 - Counts the frequency of each word and identifies the top appearing words.

## Stock Project - 3)
This code retrieves stock price data and visualizes it through graphs.

### Ranking Companies based on Comprehensive Data:
 - It processes the keyword file to calculate the frequency of keywords in each category.
 - Then, it combines the company ranking information file with the keyword frequency to create a comprehensive ranking. It extracts information on the top-ranked companies and saves the results.

### Drawing Price Graphs:
 - It uses the top 5 companies' codes from the comprehensive ranking to fetch stock price information from Naver Finance.
 - The retrieved price information is divided into daily, weekly, and monthly intervals, and graphs are plotted accordingly.
 - Each graph also includes a trend line representing the price trend.
