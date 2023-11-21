# Equip-Data_Proj

# Context for project 

I am an operations and analytics specialist at the Wake Forest Wellbeing Center. At the Wellbeing Center, we rely on a third-party system to track a variety of data. While this system is effective at capturing the necessary information, it falls short when it comes to data output. The data we receive from this system is typically in the form of poorly formatted and extremely messy CSV files. This presents a significant challenge  when it comes to performing statistical analysis on larger data sets. As a result, the Wellbeing Center has access to a wealth of data from which it is largely unable to gain meaningful quantitative insights. 

A specific example of this dynamic was the Wellbeing Center’s gym equipment rental data. The chaotic nature of the data output significantly impeded the staff's capacity to quantitatively analyze rental patterns. In response to this challenge, I took on the responsibility of developing efficient and reproducible code to clean over 60,000 rows (about two years) of equipment rental data.  


# Issues with data 

Incorrectly Imported Columns: The initial data import included columns that were incorrectly placed, adding unnecessary complexity to the dataset.

Irrelevant Rows: Many rows contained information irrelevant to the analysis, cluttering the dataset. 

Extraneous Columns: Several columns were extraneous, further complicating the data structure.

Messy Date and Time Information: The date, time, and day of week data for each rental were contained together when having those data points in separate columns would have facilitated easier analysis. 

No Measure of Time Bins: There was no existing column that tracked in which "time bin" each item was checked out during, making it difficult to determine time patterns for rentals. 

Inadequate Item Tracking: The most critical issue was the lack of a dedicated column for tracking what item was checked out. Instead, item names were combined with other information in a single column, making it challenging to isolate the necessary details. Specifically, the item name was followed by the names of the individuals who rented it, often with irrelevant information in between, all within a single column. An item column was needed to enable analysis. 

# Solutions

I used both tidyverse and base R functions to systematically clean the data, ensuring that it was in a usable and structured format. In addition, I applied several distinct for loops as part of the data cleaning process. The first for loop was instrumental in eliminating irrelevant rows, effectively decluttering the dataset and leaving only pertinent information for analysis. The second for loop was used to address the item tracking challenge, greatly increasing the analytical power of the data frame. The final for loops were used to populate a 'TimeBin' column, which tracked the two-hour time bin in which each item was checked out. The specifics of all the loops can be found in my code.

# End result and benefit

The end result of this project was the successful transformation of messy gym rental equipment data into a clean data frame, allowing me to perform previously impossible quantitative analysis on rental trends. For example, the cleaned data set allowed me to determine that men's basketballs are our most popular rental item. Through this analysis, I also identified crucial patterns in the rental of men's basketballs, enabling us to optimize our basketball open recreation hours. Previously, we relied on anecdotal evidence to set these hours, but now with clean data and comprehensive analysis, we can accurately determine the peak days and hours that basketballs are checked out, thus maximizing gym efficiency.

# Note

I have received clearance from my supervisor to publish this sample data. It's important to note two minor distinctions between the sample data provided for the public version of this project and the actual dataset. To maintain transparency, I'll outline these differences. The sample data frame included here covers a two-week period, while the original project encompassed almost two years of data. Furthermore, the original dataset contained student names and emails. To ensure anonymity, I replaced the various student names and emails from the original data set with ‘NAME’ and ‘EMAIL.’ Apart from these modifications, the data remains consistent with the original project, albeit shorter in duration and with redacted student information.
