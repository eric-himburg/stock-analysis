# An Analysis of Green Energy Stocks
## Overview of the Project
There are many different forms of green energy such as hydro, geothermal, wind and bio.  In order to determine which forms of green energy are good investments, twelve different green energy stocks were analyzed over a period of two years.  The total volume and change in starting prices of the stocks were examined over years 2017 and 2018.  Code in VBA was created to perform this analysis and was refactored in order to lower the time needed to perform the calculations.  A summary of the stock performance and the results of refactoring the code are given in the sections that follow.   
## Results
### Green Stock Performance
Kickstarter data was downloaded into an EXCEL spreadsheet.  Numerical data was turned into monetary values or dates as required, with some rounding and calculations needed to determine averages.  Dates were converted from Unix timestamps into a more standard format.  Categories of funding were separated into subcategories so that the data could be sorted to view data from plays as opposed to data from unrelated areas such as food trucks.  Once the data was filtered into plays, the outcome of all plays were plotted by funding goals and launch dates. This was done by making a pivot chart and a line graph.

### Code Execution Times
A picture of the filtered data can be seen below.  There were three main challenges when working with this data.  First, all of the dates such as the funding deadline were intially a Unix timestamp.  This needed to be converted into a standard date format.  Second, the categories and subcategories of all the different Kickstarter campaign were compiled in the same column.  It was necessary to separate each one of these into a category and subcategory.  Third, some the plays did not have any backers.  This led to division by zero errors when calculating the average donor donation.  It was necessary to change these from errors to zero amounts.
![screenshot of the Excel file with Kickstarter play data only being displayed](screenshots/kickstarter_data_filtered.png)

### Play Outcomes Pivot Table
A picture of the pivot table created, which was used to create the theater outcomes based on launch data plot, can be seen below.  The data was filtered to show only theater data.  Additionally, it was necessary to remove "live" plays from the table.      
![screenshot of the pivot table breaking down play campaign outcomes](screenshots/pivot_table.png)

## Summary
### Advantages and Disadvantages of Refactored Code
A plot of the theater outcomes versus launch data is shown below.  It can concluded by looking at the graph that more plays are funded in the summer months versus the winter months.  Specifically, there is a peak in successfully funded plays starting in May and slowly declining through December.  Notice how the amount of failed and canceled plays stays relatively the same throughout the year, with some modest variability.  Hence, based on this data the best chance one has to have a play successfully funded would be in the month of May.  The worst time to get a play funded would be in December.  
![theater outcomes versus month line graph](resources/Theater_Outcomes_vs_Launch.png)

### Application to Current VBA Code
A plot of the play outcomes based on funding goals is shown below.  A general trend that can be concluded from the graph is the higher the funding goal the less likely the play is to be successful.  Hence, if one wishes to have a successfully funded play, a lower funding goal is more likely to result in success.  These trends do reverese themselves temporarily in the mid-funding ranges of 35k - 50, which may be due to the type of play being funded or the type of donors solicited to fund these plays. An interesting observation is that none of the plays funded were canceled.  Meaning, all plays that met their funding goals were successfully produced.  
![outcomes of plays based upon funding goals](resources/Outcomes_vs_Goals.png)

 

