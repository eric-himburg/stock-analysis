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
A picture of the filtered data can be seen below.  There were three main challenges when working with this data.  First, all of the dates such as the funding deadline were intially a Unix timestamp.  This needed to be converted into a standard date format.  Second, the categories and subcategories of all the different Kickstarter campaign were compiled in the same column.  It was necessary to separate each one of these into a category and subcategory.  Third, some the plays did not have any backers.  This led to division by zero errors when calculating the average donor donation.  It was necessary to change these from errors to zero amounts.
![screenshot of the Excel file with Kickstarter play data only being displayed](screenshots/kickstarter_data_filtered.png)

## Summary
### Advantages and Disadvantages of Refactored Code
A plot of the theater outcomes versus launch data is shown below.  It can concluded by looking at the graph that more plays are funded in the summer months versus the winter months.  Specifically, there is a peak in successfully funded plays starting in May and slowly declining through December.  Notice how the amount of failed and canceled plays stays relatively the same throughout the year, with some modest variability.  Hence, based on this data the best chance one has to have a play successfully funded would be in the month of May.  The worst time to get a play funded would be in December.  
![theater outcomes versus month line graph](resources/Theater_Outcomes_vs_Launch.png)

### Application to Current VBA Code
A plot of the play outcomes based on funding goals is shown below.  A general trend that can be concluded from the graph is the higher the funding goal the less likely the play is to be successful.  Hence, if one wishes to have a successfully funded play, a lower funding goal is more likely to result in success.  These trends do reverese themselves temporarily in the mid-funding ranges of 35k - 50, which may be due to the type of play being funded or the type of donors solicited to fund these plays. An interesting observation is that none of the plays funded were canceled.  Meaning, all plays that met their funding goals were successfully produced.  
![outcomes of plays based upon funding goals](resources/Outcomes_vs_Goals.png)

 

