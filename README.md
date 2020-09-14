#HW4_submission_pandas
Pandas Homework HW4

Heroes of Pymoli: Standard import of dependencies and csv file.

Decided to do a len function on the unique screen names instead of a count function as I found there to be screen names making more than one purchase.

For Purchasing Analysis I did the same len function on the unique item names, a mean, count, and sum function to finish the table. From there just formated two of the data points into currency. Created a dataframe and boom goes the dynamite.

From Gender Demographics the first step was to drop the duplicates of screen names as it would double or even triple count some of the gender values. Did a len function on if the gender matched male, female, or other to get counts and then used those values to get a percentage of the total count of gender. Formated the values to percentage and then created a dataframe from a dictionary.

For Purchasing Analysis(Gender) I didnt really know where to start. I created a seperate DF from a groupby of Gender to get a value count of purchases. Created another new DF for the prices of purchases by gender. Created yet another df for the total purchase value so I could divide those totals by the gender counts I did in the previous step. After I got all of the data I needed I merged 4 DF together using inner join by Gender, renamed some columns, then did formating.

Age Demographics: Removed duplicates again then binned the ages into the designated bins and labels using the cut function. Use count to find players in those age ranges, then used list comprehension to get the percentage based off of total players.

Purchasing analysis (Age) I struggled with util I found the .agg function on stackoverflow. It allowed me to calculate count, mean, and sum of the columns I needed while grouping the intial data set by my new age groups. Renamed some columns then did a quick division to get total purchase per person.

For the last three DFs I utilized the .agg function again to get the basics of the DF from the original data. From there is was simply sorting, then using the .head function to get the top 5 rows needed.