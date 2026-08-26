---
layout: default
title: 3-Building Dashboards
nav_order: 4
parent: Sales Data Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Building a Dashboard

If you and your group have any questions or get stuck as you work through this in-class exercise, please ask the instructor for assistance. Enjoy! For this exercise, we are going to build a dashboard using the different visualizations created in Activity 2.

## Part 1
1.  Building a data dashboard
    - Click the **Dashboard** icon <img src="images\activity-3\icon-dashboard.png" alt="new dashboard icon" style="width:30px;"> on the bottom toolbar to create a new dashboard.
    - On the left side of the window, under **Size**, click the drop-down arrow next to **Range** and select **Automatic**. This will automatically adjust the size of the dashboard to fit the screen on which it is displayed. <img src="images\activity-3\2-dashboard-menu.png" alt="dashboard menu" style="float:right;width:250px;">
    - Under **Sheets** on the left side, you will see the worksheets you created in Activity 2.
    - From the **Sheets** list, drag the **Total Sales by Country** map onto the dashboard.
    - From the **Sheets** list, drag the **Quarterly Profit and Sales by Product** chart onto the bottom half of the dashboard. The two visualizations should now be arranged from top to bottom.

<button onclick="toggle('gif1')">Show/Hide Animation</button>
<div id="gif1">
           <img src="images\activity-3\1-setup.gif" alt="building a dashboard" style="width:720px;"><br>
     </div>

<img src="images\activity-3\1-filter-icon-cropped.png" alt="filter icon" style="float:right;width:120px;">

### 2. Creating a Visualization Filter

- Click the white space on the **Total Sales by Country** map. Icons should appear in the top-right corner of the visualization.
- Click the **Use as Filter** icon to make the map act as a filter for the other visualization.
- Click on any country on the map. The **Quarterly Profit and Sales by Product** chart will automatically update to display data for the selected country.

<button onclick="toggle('gif2')">Show/Hide Animation</button>
<div id="gif2">
            <img src="images\activity-3\1-filter.gif" alt="using a visualization as a filter" style="width:720px;"><br>
     </div>

### 3. Saving Your Visualizations and Dashboard to Tableau Public

- Click **File > Save to Tableau Public As...**
- Sign in when prompted. If you do not already have a Tableau Public account, you will need to create one.
- Your workbook, including the visualizations and dashboard, will be saved to Tableau Public.

### 4. Saving Your Workbook in Tableau Desktop

- Click **File > Save As** and save the workbook to your desired location.

**Your final output should look like this:**

<img src="images\activity-3\1-final.png" alt="dashboard final output" style="width:720px;">

## Part 2

This part will cover the creation of an interactive dashboard using the visualizations created in Activity 2.

- Click the **Dashboard** icon <img src="images\activity-3\icon-dashboard.png" alt="new dashboard icon" style="width:30px;"> on the bottom toolbar to create a new dashboard.
- On the left side of the window, under **Size**, click the drop-down arrow next to **Range** and select **Automatic**. This will automatically adjust the size of the dashboard to fit the screen on which it is displayed.
- Under **Sheets** on the left side, you should see the following worksheets: **Profit by Year**, **Orders by Person**, and **Date/Category/Profit**.
- From the **Sheets** list, drag **Date/Category/Profit** onto the dashboard. It will initially take up the available space on the dashboard.
- From the **Sheets** list, drag **Profit by Year** onto the lower half of the dashboard. Tableau will allow you to place the visualizations in different areas of the dashboard and will automatically adjust their sizes. At this point, your dashboard should look like this:

<img src="images\activity-3\2-filter-setup.png" alt="filter setup" style="width:720px;">

- From the **Sheets** list, drag **Orders by Person** onto the lower-right side of the dashboard.
- Manually resize **Orders by Person** so that it does not take up too much space. Experiment with the placement and size of the visualizations. The goal is to create a dashboard that presents the data in a clear and meaningful way.

<img src="images\activity-3\2-filter-icon.png" alt="filter icon" style="float:right;width:90px;">

- Now you will make the dashboard interactive. Click on the **Orders by Person** visualization. A menu should appear in the top-right corner of the visualization.
- Click **Use as Filter**. This will allow you to use the **Orders by Person** visualization to filter the other visualizations on the dashboard.
- Click on any name in the **Orders by Person** visualization. The other visualizations will automatically update to display data for the selected person.
- The dashboard now tells a story about a salesperson, including their profits by year and a breakdown of the categories of goods they sold. Your dashboard should now look like this:

<img src="images\activity-3\2-realtime-changes.png" alt="interactive dashboard example" style="width:720px;">

<button onclick="toggle('gif3')">Show/Hide Animation</button>
<div id="gif3">
          <img src="images\activity-3\2-realtime-changes.gif" alt="interactive dashboard animated example" style="width:720px;"><br>
     </div>

- You can make any of the visualizations on the dashboard act as a filter to tell a different story. For example, click on the **Date/Category/Profit** visualization and select **Use as Filter** from the menu in the top-right corner.
- Then, select **Bookcases** under the **Furniture** category by clicking directly on the corresponding line in the visualization. The other visualizations will update to display data for that selection.
- Feel free to experiment with the different filters and selections to see if you can come up with a different interpretation of the data!


<button onclick="toggle('gif4')">Show/Hide Animation</button>
<div id="gif4">
          <img src="images\activity-3\2-filters-play.gif" alt="playing with filters" style="width:720px;"><br>
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

[NEXT STEP: Earn a Workshop Badge](informal-credentials.html){: .btn .btn-blue }
