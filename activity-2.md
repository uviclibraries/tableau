---
layout: default
title: Activity 2
nav_order: 3
parent: Workshop Activities
---

# Activity 2 - Data Visualization Exercises

If you and your group have any questions or get stuck as you work through this in-class exercise, please ask the instructor for assistance. Enjoy!

We are continuing to use the Global Superstore Orders 2016 Excel spreadsheet

1.  **Treemap: Total Profit by Region**
    - Create a new sheet by clicking on the <img src="images\activity-2\icon.png" alt="new sheet icon" style="width:30px;"> icon on the page-bottom menu
    - From the dimensions list, left-click on **Region** and drag it up to the **Rows** shelf

    <img src="images\activity-2\rows.png" alt="columns and rows" style="float:right;width:360px;">

    - From the measures list, left-click on **Profit** and drag it up to the **Columns** shelf. It will default to **SUM(Profit)** and a bar chart will diaplay showing both negative and positive profits
    - Click on the **Show Me** icon <img src="images\activity-2\show-me.png" alt="show me icon" style="width:60px;"> in the top right corner of the screen to see the suggested visualizations
    - Click on **treemaps** (4th one down on left)
    - A grey pill stating **3 negative** should appear st the bottom right corner. Click on this pill to view the two options for dealing with the negative values: **Filter Data** or **Use Absolute Values**
    - By selecting **Use Absolute Values**, the negative values will appear as the same size as positive values but in a different colour
    - Right-click **Sheet 2** and rename it to **Profit by Region Treemap**. Automatically the data viz title changes to reflect the new name. Right-click the data viz title to edit further
    - !! Remember if you make any mistakes, use the back arrow key at the top left of the top toolbar to go back !!

    <img src="images\activity-2\treemaps.gif" alt="treemaps example" style="width:720px;">

    - **Your final output should look like this:**

    <img src="images\activity-2\treemaps.png" alt="treemaps" style="width:720px;">

2.  **World Map: Total Sales by Country**
    - Create a new sheet by clicking on the <img src="images\activity-2\icon.png" alt="new sheet icon" style="width:30px;"> icon on the page-bottom menu

    <img src="images\activity-2\calculated-field.png" alt="calculated field menu" style="float:right;width:360px;">

    - From the dimensions list, right-click and drag **Country** to the central **drop field here** area in the middle of the screen. Select **Country** from dialigue box that appears
    - To create a new measure, click **Analysis** on the top menu bar, and select **Create Calculated Field** from the drop-down menu. In the pop-up text box, rename the default title **Calculation1** to **Profit per Item**. The text box below allows formulas to be written, combining numerical operators and measures together. Left-click drag the **Profit** measure into the text box, type the division symbol ( / ), them left-click drag the **Quantity** measures, calculating profit per item

    <img src="images\activity-2\calculated-field.gif" alt="creating a calculated field" style="width:720px;">

    - ***change here: different on MAC slightly***

    <img src="images\activity-2\color-icon.png" alt="color icon" style="float:right;width:60px;">

    - From the measures list, right-click and drag the new **Profit per Item** measure to the Color icon (see right) in the Marks box. Select **AVG(Profit per Item)**. Now each country on the map will be colour-coded by the measure
    - To scroll around the world map, click on the black right-facing arrowhead in the zoom menu bar at the rop-left corner of the map, and select the crossed arrows. This will allow users to pan across the map
    - Let's replace our calculated measure. Right-click the **AVG(Profit per Item)** green pill from the marks box and select **remove**

    <img src="images\activity-2\color.gif" alt="color coding" style="width:720px;">

    - From the measures list, right-click on **Sales** and drag to the Color icon in the Marks box. Select **SUM(Sales)**
    - Edit map title and rename it **Total Sales by Country**
    - Click on the downward arrow in the Legend box and select **Edit Colors** to choose an appropriate colour (e.g. blue teal). Click on **Color** in the Marks box and select **Edit Colors**

    <img src="images\activity-2\edit-color.gif" alt="changing the colors" style="width:720px;">

    - **Your final output should look like this:**

    <img src="images\activity-2\final-color.png" alt="final map output" style="width:720px;">

3.  **Line & Bar Chart (Dual Combo): Quarterly Profit and Number of Sales by Product 2012-2015**
    
    <img src="images\activity-2\new-sheet.png" alt="drop field menu" style="float:right;width:240px;">
    
    - Create a new sheet by clicking on the <img src="images\activity-2\icon.png" alt="new sheet icon" style="width:30px;"> icon in the page-bottom menu
    - From the dimensions list, right-click on **Order Date** and drag to the columns shelf. From the dialogue box that appears, select the **QUARTER(Order Date)** measure option (green w/ calendar & clock icon) (see figure **->**)
    - From the measures list, right-click on **Sales** and drag to the rows shelf. Select **CNT(Sales)** from the pop-up box
    - Again, from the measures list, right-click on **Profit** and drag to the rows shelf, then select **SUM(Profit)**
    - From the dimensions list, left-click on **Category** and drag to the rows shelf

    <img src="images\activity-2\linebar-1.gif" alt="making a line bar graph" style="width:720px;">

    - Click the **Show Me** icon <img src="images\activity-2\show-me.png" alt="show me icon" style="width:60px;"> (top-right) and select the **dual combination chart** (3rd up from the bottom right). Click again on the **Show Me** icon again to close it
    - Rename the title to **Quarterly Profit and Sales by Product**

    <img src="images\activity-2\linebar-2.gif" alt="making a line bar graph 2" style="width:720px;">

    - **Your final output should look like this:**

    <img src="images\activity-2\linebar.png" alt="final linebar output" style="width:720px;">

4.  **Building Sales Graphs for the Interactive Dashboard**<br>
    
    <img src="images\activity-2\new-worksheet.png" alt="new worksheet button" style="float:right;width:180px;">
    
    -   **Profit by Year Graph**
        1.  Return to Data Source and drag the "People" sheet to the same area as "Orders"
        2.  Click on the **New Worksheet** tab at the bottom of the graph from the tables menu, click and drag **Person** to the **Columns**
        
            <img src="images\activity-2\another-icon-menu.png" alt="filter menu" style="float:right;width:360px;">
        
        3.  Click on **Ship Date** and drag it to the **Columns** as well
        4.  Click on **Profit** and drag it to the **Rows**. It will automatically produce **SUM(Profit)**
        5.  From the **Tables**, grab **Person** and drag it into the **Filters** section and click **OK** in the pop-up window. This will allow us to filter the graph by a specific person
        
            <img src="images\activity-2\show-me-advanced.png" alt="show me menu" style="width:280px;">
        
        6.  From the **Tables**, grab **Ship Date** and drag it into the **Color** section in the **Marks** pane
        7.  The last step is to click on **Show Me** icon <img src="images\activity-2\show-me.png" alt="show me icon" style="width:60px;"> in the top-right corner and select the **Side-by-Side Bars** option. After that, right-click on the name of your table at the bottom of the pane and rename it **Profit by Year**
        
            <img src="images\activity-2\side-by-side-bars.gif" alt="side by side bar graph" style="width:720px;">
        
        8.  **Your final result should look like this:**

            <img src="images\activity-2\side-by-side-bars.png" alt="side by side bar graph final output" style="width:720px;">

    
    <img src="images\activity-2\new-worksheet.png" alt="new worksheet button" style="float:right;width:180px;">
    
    -   **Orders by Person Graph**
        1.  Click on the **New Worksheet** tab at the bottom of the graph
        2.  From the **Tables** select **Person** and drag it onto **Rows**
        
            <img src="images\activity-2\text.png" alt="marks menu" style="float:right;width:360px;">
        
        3.  From the **Tables** select **Sales** and drag it onto **Text** in the **Marks** bar. The goal here is to show the numeric value without any calculations (Tableau will auromatically convert the numbers to SUM)
        4.  Right-click on your **Sheet** name at the bottom of the pane and rename it **Orders by Person**
        
            <img src="images\activity-2\orders-by-person.gif" alt="orders by person graph example" style="width:720px;">
        
        5.  **Your end result should look like this:**

            <img src="images\activity-2\orders-by-person.png" alt="orders by person graph final output" style="width:720px;">

    <img src="images\activity-2\sub-category.png" alt="filters and marks menus" style="float:right;width:240px;">
    -   **Date/Category/Profit Graph**
        1.  Click on the **New Worksheet** tab at the bottom of the graph
        2.  Click and drag **Ship Date**, **Category** and **Sub-Category** into the **Columns**
        3.  Click and drag **Profit** into **Rows**
        4.  Your Columns and Rows should look like this:
        
            <img src="images\activity-2\columns-rows-4(3).png" alt="columns and rows logo" style="width:360px;">
        
        5.  Click and drag **Sub-Category** onto the **Color** pane in the **Marks** section
        6.  Click and drag **Country** into the **Filters** section. In the pop-up window click **All** and click **OK**
        7.  Rename your table **Date/Category/Profit
        
            <img src="images\activity-2\date-category-profit.gif" alt="date category profit graph" style="width:720px;">
        
        8.  **Your graph should look like this:**

        <img src="images\activity-2\date-category-profit.png" alt="date category profit graph final output" style="width:720px;">


[NEXT STEP: Creating Your First Dashboard (Activity 3)](activity-3.html){: .btn .btn-blue }
