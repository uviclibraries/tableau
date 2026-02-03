---
layout: default
title: 5-Create a world map 
nav_order: 7
parent: CO2 Emissions Activity
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---
# Create a world map

Start a new sheet by clicking the icon to the right of the sheet you created.

<img src="images\Tableau 3-1.png" alt="bottom toolbar" style="width:300px;">

Now, create a world map showing the average annual CO2 emissions for all countries over the past decade (or the most recent decade with data).

*Hint*: to make sure Tableau understand that the country names are geographic entities to be placed on a map, first hover over the Country Name field and click the arrow beside it. Select Geographic Role in the dropdown, then select Country/region. 

<details>
<summary>View suggested solution</summary>
1.	Drag the Country Name field into the Marks shelf. If a map doesn’t show up automatically, in the Marks shelf toggle and change Automatic to Map.
<br/>
<img src="images\Tableau-5-1.gif" alt="bottom toolbar" style="width:480px;">
<br/>
2.	Drag the Year field to the Filters shelf, then enter 2013 to 2023 under the Range of Values tab.
<br/>
<img src="images\Tableau-5-2.gif" alt="bottom toolbar" style="width:480px;">
<br/>
3.	Drag the Annual CO2 emission (per capita) field to the Marks shelf. Hover over it in the Marks shelf, click the arrow, hover over Measure, then select Average. This will generate average CO2 emissions for the specified year range. Click the icon beside the field and select Color. If you want to edit the colours, hover over the title of the legend on the right side of the window, and click Edit colors in the dropdown.
<br/>
<img src="images\Tableau-5-3.gif" alt="bottom toolbar" style="width:480px;">
<br/>
4.	Name the map "Map of Average CO2 Emissions (2013-2023)".
</details>

[NEXT STEP: Create a dashborad](create-dashboard.html){: .btn .btn-blue }

<style>

/* 
  This styles ALL <details> elements on the page.
  It gives them a border, padding, margin, rounded corners,
  and a light gray background so they look like "boxed" sections.
*/
details {
  border: 1px solid #ccc;        /* Gray border around the details box */
  background: #f9f9f9;           /* Light gray background color */
  padding: .75em;                /* Space inside the box */
  margin: 1em 0;                 /* Space above and below the box */
  border-radius: 3px;            /* Slightly rounded corners */
}

/*
  This targets <details> ONLY when they are OPEN.
  When the box is expanded, this gives it a different background color 
  to visually indicate that it’s active.
*/
details[open] {
  background: #fffbea;           /* Light yellow background when expanded */
}

/*
  This styles the <summary> (the clickable title bar of the toggle).
  Bold text + pointer cursor makes it look interactive.
*/
summary {
  font-weight: bold;             /* Makes the summary text bold */
  cursor: pointer;               /* Shows a hand cursor to indicate it's clickable */
}

</style>
