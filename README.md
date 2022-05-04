# Module 3 Challenge

## Crypto Arbitrage

This is an analysis of arbitrage opportunities identified between the price of bitcoin on two different exchanges.

- The goal is to identify profitable (covering a 1% trade fee) trading dates within the dataset.

---

## Technologies

Python Code

- import pandas

- import pathlib

## Installation Guide

- ```import pandas as pd```

- ```from pathlib import Path```


---

### Collect the Data

The data consists of CSV files that contain the date, high/low prices, and open/close prices
 - The entire date range for the data files is **01-01-2018 to 03-31-2018**.
 
 Read the data into Pandas dataframe.
 
---

### Data Prep
 
Complete for both datasets.
 
- For the bitstamp DataFrame, replace or drop all ```NaN```, or missing, values in the DataFrame.

- Use the ```str.replace``` function to remove the dollar signs **($)** from the values in the Close

- Convert the data type of the Close column to a ```float```

- Review for duplicated values and drop them if necessary.

---

### Analyze the Data

Complete for both datasets.

- Chose column "Close"

- Use ```.describe``` to get summary statistics and ```.plot``` the data

- Used the ```.plot``` to identify potential arbitrage opportunities early in the dataset.

- Selected a date in the early, middle, and late portion of the dataset.

- to determine spread, elected to subtract the lower priced exchange from the higher priced one.

Initial view of data shows more price separation earlier in the dataset.

This initial hypothesis held true througout the exercise.

After filtering potential returns that were greater than 0 and covered a 1% trade fee.

I found the best opportunity to maximize returns was to trade during a day in late January 2018. 

The average return for January 28, 2018 would have been `$247.55`. The average return for middle date February 15,2018 was `$11.27`. The average return for late date March 31, 2018 was `$6.24`.

The max return for January 28, 2018 would have been `$439.01`. The max return for middle date February 15,2018 was `$48.80`. The average return for late date March 31, 2018 was `$30.00`.

These two summary statistics offer **2 ways to interpret the data**. 

- In sum the average and maximum returns are highest in the early period.
