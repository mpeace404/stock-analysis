# Stock-Analysis

## Overview of Project

### Purpose

Our client, Steve, wanted to use the worksheet previously created to be able to run the same analysis on other stocks. The goal was to refactor the code to make it cleaner and for it to run faster; while the original code may word for a handful of stocks, if he should decide to analyze hundreds, or even thousands of stocks the code as originally written might not be adequate.

## Analysis and Challenges

## Results

The beginning of the code creates the input box to get the year the analysis should be run on, begins the timer, and formats the header row. 
Then it builds the array of tickers followed in the project
![image](https://user-images.githubusercontent.com/82191831/125208640-c33a1200-e261-11eb-8fc7-62419cae540f.png)


The next section activates the necessary worksheet, gets a count of how many rows should be looped over, and creates a ticker index. 
Then it creates output arrays for ticker volume, starting prices and ending prices, and initializes the ticker volume to 0

![image](https://user-images.githubusercontent.com/82191831/125208786-9e926a00-e262-11eb-8b2c-31135cd4d243.png)


Next, the for loop that fills in the spreadsheet with the requested data is created. This block goes over all rows in the spreadsheet, and determines volume of the current ticker, and starting and ending price to calculate the return later on.

![image](https://user-images.githubusercontent.com/82191831/125208891-40b25200-e263-11eb-8e0d-83d082b3bcd4.png)


The next portion outputs the results to the AllStocksAnalysis page

![image](https://user-images.githubusercontent.com/82191831/125209002-f41b4680-e263-11eb-972e-259fa5448ac6.png)


Finally, the last section formats the AllStocksAnalysis page with colors, text styling, and formatting. 
It also ends the timer, and provided the popup that shows the time it took to run the script. 

![image](https://user-images.githubusercontent.com/82191831/125209179-28433700-e265-11eb-8b83-75a1a21dcaeb.png)


## Summary

Refactoring code has many advantages, it gives you another look at the code to see if any of it is repetitive, if any variables could be used to decrease said repetition, which ultimaely works to improve the time it takes the code to run. Refactoring is a lot like proofreading your code with fresh eyes to see what can be made better and what could be dropped completely. On the other hand, refactoring can cause more errors and hours of corrections if not done carefully; it's a good idea to work from a copy of the code that was originally built.

One main disadvantage of the refactored script is that it's still built for the original 12 stocks, it may get slower and slower as more tickers are added. There could be a solution that automates which tickers are used, and may improve elapsed time when analyzing hundreds or thousands of stocks.
