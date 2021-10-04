---
layout: default
title: Activity 1
nav_order: 2
parent: Workshop Activities
---

# Activity 1 - Connecting to Data

if you and your group have any questions or get stuck as you work through this in-class exercise, please ask the instructor for assistance. Have fun!

_Please note that creating a Tableau account and using the application requires your email address and data you load into Tableau Public to be stored on/shared with Tableau servers located outside Canada. B.C. privacy legislation requires we inform you of this and obtain your consent to this arrangement. Participation in this workshop will be considered as your consent._

1.  **Getting Familiar with Tableau**
    - If you haven't already, [download and install](https://www.tableau.com/academic/students){:target="_blank"} Tableau for Students
    - Open Tableau Desktop and get familiar with the interface
        - Discover Pane (right): Educational resources and links to relevant content
        - Recent Flows (middle): Previous files are displayed here.
        - Connect Pane (left): Select a data source
2.  **Getting Started With Data**
    - In Connections Pane (left), click **Microsoft Excel**. Open the **Global Superstore Orders 2016.xlsx** file you downloaded to your computer or, if you haven't already, [download it now](https://goo.gl/yTDhMB){:target="_blank"}
    - In the Connections Pane (below), we see all the sheets in the Excel file. Drag the **Orders** sheet into the flow pane as shown
    - The **Orders** sheet can be renamed by simply double-clicking on the column name if it is not clear
    - You can also change the default data type by clicking on the data icon as shown. There are 4 data types: numeric (***image***), text (***image***), geospatial (***image***), date(***image***), and date-and-time (***image***)
3.  **Working With Data**
    - Click the **Sheet 1** tab on the bottom toolbar to create our first worksheet
    - We see column names on the left side menu, broken up into dimensions (blue) and measures (green). Dimensions are fields that cannot be aggregated; Measures are fields that can be measured, aggregated, or used for mathematical operations
    - Let's get the relationship between two variables: Sales (in Measures), and Order Date (in Dimensions)
        - Right-click and drag the **Sales** measure into the **Rows** shelf (top)
        - In the dialogue box that appears, select AVG(Sales) for average sales
        - Right-click and drag the **Order Date** dimension into the **Columns** shelf (top)
        - In the dialogue box that appears, select YEAR(Order Date). In Tableau, it will automatically visualize it

    - Click the **"+"** in the YEAR(Order Date) blue pill and drill down to get quarters
    - Click **Show Me** (top right) to display the different plot types that Tableau recommends. Try a few and think about their effect on the 4 data visualization principles
    - The **Marks** card area (to the left of the visualization charts) is where you can control the visual features of your plot, Try changing the colour and size
    - You can also control the visual appearance of your plot according to dimensions of interest. For example, right-click drag the **Category** in the dialigue box that appears. Please note that the dialog box does not always appear

[NEXT STEP: Building Data Visualizations (Activity 2)](activity-2.html){: .btn .btn-blue }
