# End-to-End-Cricket-Analytics

## Aim:

To use the data of ICC Men's T20 World Cup 2022 to come up with the best possible playing-11 team.

## About the data:

The players for the final playing-11 have been divided into five categories, namely,

1) Power Hitters/ Openers
2) Anchors/ Middle Order
3) Finishers/ Lower Middle Order
4) All Rounders/ Lower Order
5) Specialist Fast Bowlers/ Tail End

The parameters and the corresponding criteria for each category can be found in the parameters.pdf file in the repository.

## Process:

### 1) Scraping the data:

For this project, four types of data were scraped from the [ESPNcricinfo](https://stats.espncricinfo.com/ci/engine/records/index.html) website: match results, batting and bowling stats for each match and, individual player details.

Web scraping was performed using Selenium and BeautifulSoup libraries in Python. The code for web scraping can be found in ESPNwebscraping.ipynb file and the scraped data can be found in the scraped-data folder in this repository.

### 2) Data Cleaning and Preprocessing:

After scraping, the data had to be cleaned and preprocessed so that it could be effectively used for visualization in PowerBI. Some operations performed include removing unnecessary columns and removing special characters from name of players.

Data cleaning and preprocessing was done using Pandas and re libraries of Python. The code for data preprocessing can be found in Cricket-preprocessing.ipynb file and the cleaned data can be found in the cleaned-csv folder.

### 3) Data Visualization and Dashboard building:

All the cleaned csv data was imported in Microsoft PowerBI to build dashboards. Some required transformations were done to the data and the required DAX measures were built. Finally, an interactive dashboard was built using the data and measures.

Player Analytics for each category can be found by following the sub-tabs in the Player Analytics tab.
The final playing-11 can be chosen in the Final Playing-11 tab in the dashboard.

The list of shortlisted players for the final playing-11 can also be found in the Final-11.xlsx file in the repository.
