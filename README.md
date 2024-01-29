# PowerBI
This repository contains my PowerBI practices and projects</br></br>
PowerBI is good tool for data analysis and data processing. It's very handy and easy to understands. With lots of visualization options, it helps us to better understand our data. With function of 'Tranform data' we can easily processes our data and clean our dataset like removing the Null values, Changing the type of column, Unpivoting the table using Power query and these changes can be undone also in simplified way.</br></br>
I did this course from Youtube channel **Alex the Analyst**(https://www.youtube.com/watch?v=g0m5sEHPU-s&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys)</br></br>
All the dataset files or any other related files is include with this repository.

## DAX in PowerBI
DAX (Data Analysis Expressions) is a formula language used in Power BI to create custom calculations and aggregations for data analysis. </br>
Here Apocolypse Food Prep dataset is used. And function such as SUM, SUMX and IF is used to get some information about the table.</br>
Examples:
- Count of sales = COUNT('Apocolypse Sales'[Order ID])
- Day of Week = WEEKDAY('Apocolypse Sales'[Date Purchased],2)
- Order_Size = IF('Apocolypse Sales'[Units Sold]>25,"Big Order", "Small Order")
- Sum of Products Sold = SUM('Apocolypse Sales'[Units Sold])
- Profit = (sum('Apocolypse Store'[Price]) - SUM('Apocolypse Store'[Production Cost]))* SUM('Apocolypse Sales'[Units Sold])
- Profit_Column = (sum('Apocolypse Store'[Price]) - SUM('Apocolypse Store'[Production Cost]))* SUM('Apocolypse Sales'[Units Sold])
- Profit_column_sumx = SUMX('Apocolypse Sales', ('Apocolypse Store'[Price] - 'Apocolypse Store'[Production Cost])*'Apocolypse Sales'[Units Sold]) #SUMX will calculate the profit by each row</br></br>
Refrence: How to use DAX in Power BI | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=vcijg0gUXSg&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=5

## Drill down in PowerBI
Drill down is used in visualization in PowerBI when we want to know more details about a the graph drawn, it is usefull to understand the data distribution in depth.</br></br>
Reference: How to use Drill Down in Power BI | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=ulFY20KTzFQ&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=5

## Conditional Formatting in PowerBI
Conditional formatting can be used to enhance the visualization, we can add more colours, different icon and different font in order to differentiate the values making it more comprehensible. </br></br>

Reference: How to use Conditional Formatting in Power BI | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=m0h3Ghl6mgY&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=7
