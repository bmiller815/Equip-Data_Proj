# Equip-Data_Proj

Context for project 
I am an Operations and Analytics Specialist at the Wake Forest Wellbeing Center. At the Wellbeing Center we rely on a third-party system to track a variety of data. While this system is effective at capturing the necessary information, it falls short when it comes to data output. The data we receive from this system is typically in the form of poorly formatted and extremely messy CSV files. This presents a significant challenge  when it comes to performing statistical analysis on larger data sets. As a result, the Wellbeing Center has access to a wealth of data that it is largely unable to gain meaningful insights from. 

A specific example of this dynamic was the Wellbeing Center’s gym equipment rental data. The chaotic nature of the data output significantly impeded the staff's capacity to quantitatively analyze rental patterns. In response to this challenge, I took on the responsibility of developing efficient and reproducible code to clean almost two years worth of equipment rental data.  


Issues with data 
Incorrectly Imported Columns: The initial data import included columns that were incorrectly placed, adding unnecessary complexity to the dataset.
Irrelevant Rows: Many rows contained information that was irrelevant to the analysis, cluttering the dataset. 
Extraneous Columns: Several columns were extraneous, further complicating the data structure.
Messy Date and Time Information: The date, time, and day of week data for each rental were contained together when having those data points in separate columns would have facilitated easier analysis. 
Inadequate Item Tracking: The most critical issue was the lack of a dedicated column for tracking what item was checked out. Instead, item names were combined with other information in a single column, making it challenging to isolate the necessary details. Specifically, the item name was followed by the names of the individuals who rented it, often with irrelevant information in between, all within a single column. An item column was needed to enable analysis. 

Solution
I used both tidyverse and base R functions to systematically clean the data, ensuring that it was in a more usable and structured format. In addition, I applied two distinct for loops as part of the data cleaning process. The first for loop was instrumental in eliminating irrelevant rows, effectively decluttering the dataset and leaving only pertinent information for analysis. The second for loop was used to address the item tracking challenge, greatly increasing the analytical power of the data frame. The specifics of the two loops can be found in my script. 

End result and benefit
The end result of this project was the successful transformation of messy gym rental equipment data into a clean data frame. Having a clean data frame will allow previously impossible quantitative analysis on gym equipment rental to be performed. For example, this data set will allow us to optimize our basketball open recreation hours. Previously, we relied on anecdotal evidence to set these hours, but now, with clean data, we can accurately determine the peak days and hours that basketballs are checked out. With that knowledge we will be able to line up open recreation hours with peak hours and days, thus maximizing gym efficiency.
