---
layout: default
title: Activity 2
nav_order: 3
parent: Workshop Activities
---

# Activity 2 - Data Visualization Exercises

If you and your group have any questions or get stuck as you work through this in-class exercise, please ask the instructor for assistance. Enjoy!

We are continuing to use the Global Superstire Orders 2016 Excel spreadsheet

1.  **Treemap: Total Profit by Region**
    - Create a new sheet by clicking on the ***image*** icon on the page-bottom menu
    - From the dimensions list, left-click on **Region** and drag it up to the **Rows** shelf
    - From the measures list, left-click on **Profit** and drag it up to the **Columns** shelf. It will default to **SUM(Profit)** and a bar chart will diaplay showing both negative and positive profits
    - Click on the **Show Me** icon ***image*** in the top right corner of the screento see the suggested visualizations
    - Click on **treemaps** (4th one down on left)
    - A grey pill stating **3 negative** should appear st the bottom right corner. Click on this pill to view the two options for dealing with the negative values: **Filter Data** or **Use Absolute Values**
    - By selecting **Use Absolute Values**, the negative values will appear as the same size as positive values but in a different colour
    - Right-click **Sheet 2** and rename it to **Profit by Region Treemap**. Automatically the data viz title changes to reflect the new name. Right-click the data viz title to edit further
    - !! Rememberif you make any mistakes, use the back arrow key at the top left of the top toolbar to go back !!
    - **Your final output should look like this:**
2.  **World Map: Total Sales by Country**
    - Create a new sheet by clicking on the ***image*** icon on the page-bottom menu
    - From the dimensions list, right-click and drag **Country** to the central **deop field here** area in the middle of the screen. Select **Country** from dialigue box that appears
    - To create a new measure, click **Analysis** on the top menu bar, and select **Create Calculated Field** from the drop-down menu. In the pop-up text box, rename the default title **Calculation1** to **Profit per Item**. The text box below allows formulas to be written, combining numerical operators and measures together. Left-click drag the **Profit** measure into the text box, type the division symbol ( / ), them left-click drag the **Quantity** measures, calculating profit per item
    - ***change here: different on MAC slightly***
    - From the measures list, right-click and drag the new **Profit per Item** measure to the Color icon ***image*** in the Marks box. Select **AVG(Profit per Item)**. Now each country on the map will be colour-coded by the measure
    - To scroll around the world map, click on the black right-facing arrowhead in the zoom menu bar at the rop-left corner of the map, and select the crossed arrows. This will allow users to pan across the map
    - Let's replace our calculated measure. Right-click the **AVG(Profit per Item)** green pill from the marks box and select **remove**
    - From the measures list, right-click on **Sales** and drag to the Color icon ***image*** in the Marks box. Select **SUM(Sales)**
    - Edit map title and rename it **Total Sales by Country**
    - Click on the downward arrow in the Legend box and select **Edit Colors** to choose an appropriate colour (e.g. blue teal). Click on **Color** in the Marks box and select **Edit Colors**
    - **Your final output should look like this:**
3.  **Line & Bar Chart (Dual Combo): Quarterly Profit and Number of Sales by Product 2012-2015**
    - Create a new sheet by clicking on the ***image*** icon in the page-bottom menu
    - From the dimensions list, right-click on **Order Date** and drag to the columns shelf. From the dialogue box that appears, select the **QUARTER(Order Date)** measure option (green w/ calendar & clock icon) (see figure) ***image***
    - From the measures list, right-click on **Sales** and drag to the rows shelf. Select **CNT(Sales)** from the pop-up box
    - Again, from the measures list, right-click on **Profit** and drag to the rows shelf, then select **SUM(Profit)**
    - From the dimensions list, left-click on **Category** and drag to the rows shelf
    - Click the **Show Me** icon (top-right) and select the **dual combination chart** (3rd up from the bottom right). Click again on the **Show Me** icon again to close it
    - Rename the title to **Quarterly Profit and Sales by Product**
    - **Your final output should look like this:**
4.  **Building Sales Graphs for the Interactive Dashboard**<br>
    - **Profit by Year Graph**
        + Return to Data Source and drag the "People" sheet to the same area as "Orders"
        + Click on the **New Worksheet** tab at the bottom of the graph from the tables menu, click and drag **Person** to the **Columns**
        + Click on **Ship Date** and drag it to the **Columns** as well
        + Click on **Profit** and drag it to the **Rows**. It will automatically produce **SUM(Profit)**
        + From the **Tables**, grab **Person** and drag it into the **Filters** section and click **OK** in the pop-up window. This will allow us to filter the graph by a specific person
        + From the **Tables**, grab **Ship Date** and drag it into the **Color** section in the **Marks** pane
        + The last step is to click on **Show Me** in the top-right corner and select the **Side-by-Side Bars** option. After that, right-click on the name of your table at the bottom of the pane and rename it **Profit by Year**
        + **Your final result should look like this:**
    - **Orders by Person Graph**
        + Click on the **New Worksheet** tab at the bottom of the graph
        + From the **Tables** select **Person** and drag it onto **Rows**
        + from the **Tables** select **Sales** and drag it onto **Text** in the **Marks** bar. The goal here is to show the numeric value without any calculations (Tableau will auromatically convert the numbers to SUM)
        + Right-click on your **Sheet** name at the bottom of the pane and rename it **Orders by Person**
        + **Your end result should look like this:**
    - **Date/Category/Profit Graph**
        + Click on the **New Worksheet** tab at the bottom of the graph
        + Click and drag **Ship Date**, **Category** and **Sub-Category** into the **Columns**
        + Click and drag **Profit** into **Rows**
        + Your Columns and Rows should look like this:
        + Click and drag **Sub-Category** onto the **Color** pane in the **Marks** section
        + Click and drag **Country** into the **Filters** section. In the pop-up window click **All** and click **OK**
        + Rename your table **Date/Category/Profit
        + Your graph should look like this:

[NEXT STEP: Creating Your First Dashboard (Activity 3)](activity-3.html){: .btn .btn-blue }
