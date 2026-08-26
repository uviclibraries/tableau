---
layout: default
title: 2-Data Visualization
nav_order: 3
parent: Sales Data Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Data Visualization Exercises

If you and your group have any questions or get stuck while working through this in-class exercise, please ask the instructor for assistance. Enjoy!

We are continuing to use the **Global Superstore Orders 2016** Excel spreadsheet. In the previous activity, you learned how to build visualizations in Tableau. To create a new visualization, click the **New Worksheet** icon <img src="images\activity-2\icon.png" alt="new worksheet icon" style="width:30px;"> on the sheet tabs at the bottom of the window. You can then select which variables (dimensions or measures) you want to assign to rows, columns, or other characteristics of the visualization (e.g., colour and size), choose a visualization type, and make any additional adjustments as needed.

In this activity, we will create different types of visualizations in Tableau to explore different trends in the data. In the next activity, you will learn how to combine these visualizations into a single interactive dashboard.

1. **Treemap: Total Profit by Region**
    - Create a new worksheet by clicking the <img src="images\activity-2\icon.png" alt="new worksheet icon" style="width:30px;"> icon at the bottom of the window.
    - From the **Dimensions** list, right-click **Region** and drag it to the **Rows** shelf

    <img src="images\activity-2\rows.png" alt="columns and rows" style="float:right;width:360px;">

    - From the **Measures** list, right-click **Profit** and drag it to the **Columns** shelf. Tableau will default to **SUM(Profit)** and display a bar chart showing both negative and positive profits
    - Click the **Show Me** icon <img src="images\activity-2\show-me.png" alt="Show Me icon" style="width:60px;"> in the top-right corner of the screen to view the visualizations Tableau recommends
    - Select **Treemap** (4th option down on the left)
    - A grey **3 negative** indicator should appear in the bottom-right corner. Click this indicator to view the two options for dealing with the negative values: **Filter Data** or **Use Absolute Values**
    - Select **Use Absolute Values**. The negative values will appear as the same size as positive values, but in a different colour
    - Rename the worksheet by right-clicking the **Sheet 2** tab at the bottom of the window and selecting **Rename**. Rename it **Profit by Region Treemap**. The visualization title will automatically update to reflect the new worksheet name. You can right-click the visualization title if you would like to edit it further
    - **Remember:** If you make a mistake, use the back arrow at the top-left of the toolbar to undo your last action
    
    <button onclick="toggle('gif1')">Show/Hide Animation</button>
    <div id="gif1">
           <img src="images\activity-2\treemaps.gif" alt="treemaps example" style="width:720px;"> <br>
         </div> 
    
    - **Your final output should look like this:**

    <img src="images\activity-2\treemaps.png" alt="treemaps" style="width:720px;">

2. **World Map: Total Sales by Country**
    - Create a new worksheet by clicking the <img src="images\activity-2\icon.png" alt="new worksheet icon" style="width:30px;"> icon at the bottom of the window
    - From the **Dimensions** list, right-click **Country** and drag it to the central **Drop field here** area in the middle of the screen. Select **Country** from the menu that appears
    - To create a new measure, click **Analysis** in the top menu bar and select **Create Calculated Field** from the drop-down menu. 
    - **Mac users:** The **Analysis** menu is located in the Mac menu bar at the very top of the screen rather than in the Tableau application window
    - The **Calculation Editor** will open. Rename the calculated field from **Calculation1** to **Profit per Item**
    - In the formula area, create the calculation for profit per item by dragging **Profit** from the **Data** pane into the formula area, typing `/`, and then dragging **Quantity** into the formula area. Your calculation should divide **Profit** by **Quantity**
    
    <button onclick="toggle('gif2')">Show/Hide Animation</button>
    <div id="gif2">
           <img src="images\activity-2\calculated-field.gif" alt="creating a calculated field" style="width:720px;"> <br>
         </div> 
    
      <img src="images\activity-2\color-icon.png" alt="color icon" style="float:right;width:60px;">

     - From the **Measures** list, right-click and drag the new **Profit per Item** measure to **Color** on the **Marks** card (see image on the right). Select **AVG(Profit per Item)** from the menu that appears. Each country on the map will now be colour-coded based on the average profit per item
    - To pan around the world map, click the black right-facing arrowhead in the map's zoom controls and select the **Pan** option (crossed arrows). This allows you to move around the map
    - We will now replace the calculated measure. Right-click **AVG(Profit per Item)** on the **Marks** card and select **Remove**
    
    
    <button onclick="toggle('gif3')">Show/Hide Animation</button>
    <div id="gif3">
            <img src="images\activity-2\color.gif" alt="color coding" style="width:720px;"><br>
         </div> 
    
    - From the **Measures** list, right-click **Sales** and drag it to **Color** on the **Marks** card. Select **SUM(Sales)** from the menu that appears
    - Edit the map title and rename it **Total Sales by Country**
    - Try changing the colours by clicking **Color** on the **Marks** card and selecting **Edit Colors**
    
    <button onclick="toggle('gif4')">Show/Hide Animation</button>
    <div id="gif4">
              <img src="images\activity-2\edit-color.gif" alt="changing the colors" style="width:720px;"><br>
         </div> 
    
    
    - **Your final output should look like this:**
    
        <img src="images\activity-2\final-color.png" alt="final map output" style="width:720px;">

3. **Line & Bar Chart (Dual Combo): Quarterly Profit and Number of Sales by Product 2012-2015**
    
    <img src="images\activity-2\new-sheet.png" alt="drop field menu" style="float:right;width:240px;">
    
    - Create a new worksheet by clicking the <img src="images\activity-2\icon.png" alt="new worksheet icon" style="width:30px;"> icon at the bottom of the window
    - From the **Dimensions** list, right-click **Order Date** and drag it to the **Columns** shelf
    - From the menu that appears, select **QUARTER(Order Date)**. Note: This option may not automatically appear
        - **Windows users:** Click the small arrow next to **YEAR(Order Date)** and select **Quarter**
        - **Mac users:** Click the **+** next to **YEAR(Order Date)** to drill down to Quarter
    - From the **Measures** list, right-click **Sales** and drag it to the **Rows** shelf. From the menu that appears, hover over **Measure** and select **Count**
    - From the **Measures** list, right-click **Profit** and drag it to the **Rows** shelf. Select **SUM(Profit)** from the menu that appears
    - From the **Dimensions** list, right-click **Category** and drag it to the **Rows** shelf


    <button onclick="toggle('gif5')">Show/Hide Animation</button>
    <div id="gif5">
              <img src="images\activity-2\linebar-1.gif" alt="making a line bar graph" style="width:720px;"> <br>
         </div> 
    
    - Click the **Show Me** icon <img src="images\activity-2\show-me.png" alt="Show Me icon" style="width:60px;"> in the top-right corner and select the **Bar Line Chart** option (3rd option up from the bottom-right). Click the **Show Me** icon again to close the menu
    - Rename the worksheet by right-clicking its sheet tab at the bottom of the window and selecting **Rename**. Rename it **Quarterly Profit and Sales by Product**
    
    <button onclick="toggle('gif6')">Show/Hide Animation</button>
    <div id="gif6">
              <img src="images\activity-2\linebar-2.gif" alt="making a line bar graph 2" style="width:720px;"><br>
         </div>


    - **Your final output should look like this:**

    <img src="images\activity-2\linebar.png" alt="final linebar output" style="width:720px;">

4. **Building Sales Graphs for the Interactive Dashboard**<br>

Above, you learned how to create different types of graphs. Now we will create additional charts that we will later combine into a single interactive dashboard.
    
    
   -   **Profit by Year Graph**
         1. Go to **Data Source** in the bottom-left corner. From the **Sheets** list, drag the **People** sheet onto the same area as the **Orders** sheet. Because both tables contain a field called **Region**, Tableau will automatically create a relationship between the two tables using **Region**. This allows information from the **People** table to be used alongside information from the **Orders** table
        2. Click the **New Worksheet** icon at the bottom of the window to create a new worksheet <img src="images\activity-2\new-worksheet.png" alt="new worksheet button" style="float:right;width:150px;">
        3. From the **People** table in the **Data** pane, click and drag **Person** to the **Columns** shelf <img src="images\activity-2\another-icon-menu.png" alt="filter menu" style="float:right;width:300px;">
        4. From the **Orders** table in the **Data** pane, click and drag **Ship Date** to the **Columns** shelf
        5. From the **Orders** table in the **Data** pane, click and drag **Profit** to the **Rows** shelf. Tableau will automatically use **SUM(Profit)**
        6. From the **People** table in the **Data** pane, click and drag **Person** to the **Filters** shelf. In the filter window that appears, click **OK**. This will allow you to filter the graph by a specific person
        7. From the **Orders** table in the **Data** pane, click and drag **Ship Date** to **Color** on the **Marks** card
        8. Click the **Show Me** icon <img src="images\activity-2\show-me.png" alt="Show Me icon" style="width:60px;"> in the top-right corner and select the **Side-by-Side Bar Chart** option
        9. Rename the worksheet by right-clicking its sheet tab at the bottom of the window and selecting **Rename**. Rename it **Profit by Year**

           <img src="images\activity-2\show-me-advanced.png" alt="show me menu" style="width:220px;">

        
        <button onclick="toggle('gif7')">Show/Hide Animation</button>
        <div id="gif7">
                  <img src="images\activity-2\side-by-side-bars.gif" alt="side by side bar graph" style="width:720px;"><br>
             </div> 
        
         -  **Your final result should look like this:**
        
            <img src="images\activity-2\side-by-side-bars.png" alt="side by side bar graph final output" style="width:720px;">
        
            
            <img src="images\activity-2\new-worksheet.png" alt="new worksheet button" style="float:right;width:200px;">
    
5. **Orders by Person Graph**
        1. Click the **New Worksheet** icon at the bottom of the window to create a new worksheet
        2. From the **People** table in the **Data** pane, click and drag **Person** to the **Rows** shelf
        
            <img src="images\activity-2\text.png" alt="marks menu" style="float:right;width:360px;">
        
        3. From the **Orders** table in the **Data** pane, click and drag **Sales** to **Text** on the **Marks** card. Tableau will automatically aggregate the values as **SUM(Sales)**
        4. Rename the worksheet by right-clicking its sheet tab at the bottom of the window and selecting **Rename**. Rename it **Orders by Person**
        
            <img src="images\activity-2\orders-by-person.gif" alt="orders by person graph example" style="width:720px;">
        
        5.  **Your end result should look like this:**

            <img src="images\activity-2\orders-by-person.png" alt="orders by person graph final output" style="width:720px;">

    <img src="images\activity-2\sub-category.png" alt="filters and marks menus" style="float:right;width:120px;">
-   **Date/Category/Profit Graph**
        1. Click the **New Worksheet** icon at the bottom of the window to create a new worksheet
        2. From the **Orders** table in the **Data** pane, click and drag **Ship Date** to the **Columns** shelf
        3. From the **Orders** table in the **Data** pane, click and drag **Category** to the **Columns** shelf
        4. From the **Orders** table in the **Data** pane, click and drag **Sub-Category** to the **Columns** shelf
        5. From the **Orders** table in the **Data** pane, click and drag **Profit** to the **Rows** shelf
        6. Your **Columns** and **Rows** shelves should look like this:
        
            <img src="images\activity-2\columns-rows-4(3).png" alt="columns and rows logo" style="width:480px;">
        
7. From the **Orders** table in the **Data** pane, click and drag **Sub-Category** to **Color** on the **Marks** card
8. From the **Orders** table in the **Data** pane, click and drag **Country** to the **Filters** shelf. In the filter window that appears, select **All** and click **OK**
9. Rename the worksheet by right-clicking its sheet tab at the bottom of the window and selecting **Rename**. Rename it **Date/Category/Profit**
        
            <img src="images\activity-2\date-category-profit.gif" alt="date category profit graph" style="width:720px;">
        
10.  **Your graph should look like this:**
        <img src="images\activity-2\date-category-profit.png" alt="date category profit graph final output" style="width:720px;">


<script>  

    function toggle(input) {
        var x = document.getElementById(input);
        if (x.style.display === "none") {
            x.style.display = "block";
        } else {
            x.style.display = "none";
        }
    }
</script>

[NEXT STEP: Creating Your First Dashboard](dashboards.html){: .btn .btn-blue }
