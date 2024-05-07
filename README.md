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
