---
layout: default
title: 1-Connecting to Data
nav_order: 2
parent: Sales Data Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Connecting to Data

if you and your group have any questions or get stuck as you work through this in-class exercise, please ask the instructor for assistance. Have fun!

_Please note that creating a Tableau account and using the application requires your email address and data you load into Tableau Public to be stored on/shared with Tableau servers located outside Canada. B.C. privacy legislation requires we inform you of this and obtain your consent to this arrangement. Participation in this workshop will be considered as your consent._

1.  **Getting Familiar with Tableau**
    - If you haven't already, [download and install](https://www.tableau.com/academic/students){:target="_blank"} Tableau for Students (Instructions on how to download are located in the pre-workshop activites)
    - Open Tableau Desktop and get familiar with the interface
        - Discover Pane (right): Educational resources and links to relevant content
        - Recent Flows (middle): Previous files are displayed here
        - Connections Pane (left): Select a data source
2.  **Getting Started With Data**
     - In the **Connections Pane** (left), click **Microsoft Excel**. Open the **Global_Superstore_Orders_2016.xlsx** file you downloaded to your computer. If you haven't already downloaded it, [download it now](resources/Global_Superstore_Orders_2016.xlsx){:target="_blank"}.
    - In the **Connections Pane** (see animation below), you will see all the sheets in the Excel file. Drag the **Orders** sheet into the **Flow Pane** as shown.
    - The **Orders** sheet can be renamed by simply double-clicking on the **sheet name**. Rename the sheet to **Global Superstore Orders**.
    - The data can be viewed in the data grid. You can rename a column by double-clicking on the column name (see animation below).
    - You can also change the default data type by clicking on the data icon as shown. There are five data types: numeric (<img src="images\activity-1\mini-icon-1.png" alt="numeric symbol" style="width:30px;">), text (<img src="images\activity-1\mini-icon-2.png" alt="text symbol" style="width:30px;">), geospatial (<img src="images\activity-1\mini-icon-3.png" alt="geospatial symbol" style="width:30px;">), date (<img src="images\activity-1\mini-icon-4.png" alt="date symbol" style="width:30px;">), and date-and-time (<img src="images\activity-1\mini-icon-5.png" alt="date and time symbol" style="width:30px;">).

<button onclick="toggle('gif1')">Show/Hide Animation</button>
<div id="gif1">
          <img src="images\activity-1\import-drag.gif" alt="import example" style="width:720px;"><br>
     </div>

    

3.  **Working With Data**
    - Click the **Sheet 1** tab on the bottom toolbar to create your first worksheet
    
    <img src="images\activity-1\tab.png" alt="bottom toolbar" style="width:480px;">
    
    - You will see column names on the left-side menu, broken up into dimensions (blue) and measures (green). Dimensions are fields that contain qualitative or categorical information, while measures are fields that contain quantitative information and can be aggregated or used in mathematical operations.
    - Let's explore the relationship between two variables: **Sales** (in Measures) and **Order Date** (in Dimensions).
        - Click and drag the **Sales** measure into the **Rows** shelf (top).
        - In the dialog box that appears, select **AVG(Sales)** to display the average sales.
        - Click and drag the **Order Date** dimension into the **Columns** shelf (top).
        - In the dialog box that appears, click **YEAR(Order Date)** if it is not already selected. Tableau will automatically create a visualization
        

    <button onclick="toggle('gif2')">Show/Hide Animation</button>
<div id="gif2">
          <img src="images\activity-1\relationship.gif" alt="setting up a relationship animated" style="width:720px;"><br>
     </div>


- Click the **"+"** in the **YEAR(Order Date)** blue pill and drill down to get quarters
- Click **Show Me** (top right) to display the different plot types that Tableau recommends. Try a few and think about their effect on the 4 data visualization principles
    
<img src="images\activity-1\show-me.png" alt="different plot types" style="width:720px;">
    
- The **Marks** card (to the left of the visualization) is where you can control the visual features of your plot. Try changing the colour and size.
- You can also control the visual appearance of your plot based on dimensions of interest. For example, right-click and drag the **Category** dimension onto the **Color** card. Select **Category** in the dialog box that appears. Please note that the dialog box does not always appear.

<button onclick="toggle('gif3')">Show/Hide Animation</button>
<div id="gif3">
           <img src="images\activity-1\style-change.gif" alt="changing graph styles" style="width:720px;"><br>
     </div>

   

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

[NEXT STEP: Building Data Visualizations](building-data-visualizations.html){: .btn .btn-blue }
