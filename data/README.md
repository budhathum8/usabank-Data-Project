# Data Dictionary

S&P 500 data from [Nasdaq](https://www.nasdaq.com/market-activity/index/spx/historical?page=1&rows_per_page=10&timeline=y10) AND
S&P 500 data from [S&P 500](https://en.wikipedia.org/wiki/S%26P_500).

## Calendar

| field | description | cleaning notes |
| ----- | ----------- | -------------- |
| date | date | fromate is YYYY-MM-DD |
| Market_Share | string | with "$" and a float with 2 decimal places |
|Stock_Price | string | with "$" and a float with 2 decimal places |
| listing_id | | |

## Reviews

| field | description | cleaning notes |
| ----- | ----------- | -------------- |
| date | Data was collected or reviewed | Remove any incorrect or incomplete dates if needed |
| Net_Income | Net income amount should be a numeric value | Remove currency symbols for missing or negative values if unexpected |
| reviewer_Assets | Ensure it's numeric | Remove any unnecessary symbols |
| reviewer_Share | This could be a percentage or proportion | Ensure the value is in percentage form, without symbols like % |
| comments | Any additional notes or context provided by the reviewer | Remove irrelevant comments if needed |

## Listings

| Colimn | Non-Null | Dtype |
| ------ | -------- | ----- |
| Date | non-null | object |
| Total_Assets | non-null | int64 |
| Shareholder_Equity | non-null | int64 |
| Market_Share | non-null | int64 |
| Stock_Price | non-null | int64 |
| | | |
| | | |
