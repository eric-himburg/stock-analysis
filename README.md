# An Analysis of Green Energy Stocks
## Overview of the Project
There are many different forms of green energy such as hydro, geothermal, wind and bio.  In order to determine which forms of green energy are good investments, twelve different green energy stocks were analyzed over a period of two years.  The total volume and change in starting prices of the stocks were examined over years 2017 and 2018.  Code in VBA was created to perform this analysis and was refactored in order to lower the time needed to perform the calculations.  A summary of the stock performance and the results of refactoring the code are given in the sections that follow.   

## Results
### Green Stock Performance
#### 2017
As can be seen in the image below, eleven of the twelve green energy stocks had positive returns in 2017.  The three stocks with the best returns included DAQO New Energy Corp (DQ), Enphase Energy (ENPH) and Solar Edge Technologies (SEDG).  All of the stocks listed have total daily volumes above the 25 million criteria used to determine if a stock is a more reliable investment.  However, it should be noted that DQ's total daily volume is just barely above this criterion, being traded several times less than the other green stocks. Also, of note is that while SunRun Inc. (RUN) only had a modest return of 5.5%, it had one of largest total daily volumes of 267 million.  
![screenshot of the Excel file with 2017 green energy stocks](Resources/VBA_Challenge_2017.png)
#### 2018
As can be seen in the image below, only two of the twelve green energy stocks had positive returns in 2018.  The two stocks that performed well, with over 80% returns, included Enphase Energy and SunRun Inc.  Additionally, both of these stocks had total daily volumes in the hundreds of millions, indicating they are a less risky investment option.  For two years straight, Enphase Energy and SunRun Inc. have have positive returns and large total daily volumes.  All other stocks, including DAQO New Energy Corp, had negative returns for 2018.     
![screenshot of the Excel file with 2018 green energy stocks](Resources/VBA_Challenge_2018.png)

### Code and Execution Times
#### Original Code
Stock data for the twelve green energy companies was imported into EXCEL and then VBA code was created to analyze the data.  
![screenshot showing a portion of the VBA code used to analyze the stock data](Screenshots/allstocksanalysis.png)


#### Refactored Code
In order to make the code more efficient, 
![screenshot showing a portion of the VBA code used to analyze the stock data](Screenshots/refactored_allstocksanalysis.png)

## Summary
### Advantages and Disadvantages of Refactored Code


### Application to Current VBA Code


 

