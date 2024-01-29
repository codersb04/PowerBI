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

## Bins and List in PowerBI
We can divide the coulumns into groups according to there distribution, this will be helpfull if someone want to know the categories of the particular columns. Grouping can be done in 2 ways:
1. Bins: It can be done on number type or date type. Grouping accordin to the range of numbersand giving the range as size of bin. example we can group the months products, to check how many product sold in just January month
2. List: It can be Performed on all type of data, we just group the data and give the title like selecting the order number from 12 to 25 and name the group as "First order". It works in the same way as an if else statement.</br></br>
Reference: How to use Bins and Lists in Power BI | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=9j_EBt3RNrs&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=7

## Visualization Tools
PowerBI have lots of different visualization tools to represent information into different forms. Graphs used here are:

- Stacked bar chart
- Donut Chart
- 100% stacked column chart
- Card
- Line Chart
- Line and clustered column chart
- Table
- Scattered Chart</br></br>

Reference: Popular Visualizations in Power BI | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=3NV5Jtbhfcw&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=9

## Final PowerBI Project
Dataset is taken from link: https://github.com/AlexTheAnalyst/Power-BI/blob/main/Power%20BI%20-%20Final%20Project.xlsx</br>
Steps Followed:

- CLeanning the data
- Changing into correct data type
- Removing the unnecessary information
- Calculating the average salary from the given range of values in each field
All the above steps are done using the power queries</br>

Following visualization is created:

- Treemap:  To represent the countries
- Donut Chart: Shows the difficulty levell to break into the tech
- Gauge: Shows how many are appy with their work/life balance and salary
- Stacked Bar chart: Average salary by job title
- Stacked column chart: Represents Favourite programming language</br></br>

Reference: Full Power BI Guided Project | Microsoft Power BI for Beginners, Alex The Analyst, https://www.youtube.com/watch?v=pixlHHe_lNQ&list=PLUaB-1hjhk8HqnmK0gQhfmIdCbxwoAoys&index=9


