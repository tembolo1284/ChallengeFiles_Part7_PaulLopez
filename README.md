# Project Title
This application is the ETF Analyzer for Challenge 7!  I begin by creating a database and importing a db file to populate the database.
Very exciting!  I then query the database for the PYPL stock alone. I run a daily return analysis on it and plot the results.
I then run a cumulative return analysis and plot the results of that. It's clear the PYPL stock is growing nicely.

After the above is complete I use some SQL to pull in the time and closes that are ONLY strictly greater than 200.0.
I also construct a query that pulls in the top ten daily returns.  So much for individual stock analysis!

Now I analyze the entire portfolio!  The first thing I do is construct a SQL query that joins all four tables together by the common
column of 'time'. I then average across all the daily returns of the stocks (assume equal weighting for the mean) and create
a dataframe with a date and average daily return of the four stocks. I then convert these average daily returns
into an annualized return.  For the final step I use the average daily returns and create a dataframe with a date and
cumulative return for each date. This final cumulative return dataframe I then plot for analysis.

## Technologies

I am using python version 3.7.10 and am importing the following from the built-in libraries and from functions i've created myself:
import numpy as np
import pandas as pd
import hvplot.pandas
import sqlalchemy

---

## Installation Guide

I have python version 3.7.10 and git version 2.33.0.windows.2 installed on a laptop running windows 10 pro.

I launch jupyter lab from the gitbash terminal and then run the etf_analyzer noteback from the 
webpage that launches.


---

## Usage

The user just needs to hit the button and run the code. The user is free to update any queries as they see fit.

That's it!


---

## Contributors
Just me, Paul Lopez.


---

## License
No licenses required. Just install everything for free, pull from my repository, and enjoy!
