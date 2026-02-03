---
layout: default
title: 4-Create a bar graph 
nav_order: 5
parent: CO2 Emissions Activity
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---
# Create a bar graph

Start a new sheet by clicking the icon to the right of the sheet you created.

<img src="images\Tableau 3-1.png" alt="bottom toolbar" style="width:300px;">

Now, create a bar plot showing the countries with the 10 highest levels of CO2 emissions in 2023 (or the most recent year of data).

*Hint*: Take advantage of the filter option to filter both by year and by countries with the highest emissions. To filter by countries with the highest emissions in 2023, you will want to use the **Top** tab in the filtering window, and select the "By formula" option. Here's a function that sums the annual emissions, but only for the 2023 emissions of each country: 
```
SUM(IIF([Year (co-emissions-per-capita.csv)]=2023, [Annual CO₂ emissions (per capita)], 0))
```
<details>
<summary>Formula explanation</summary>
The IIF function assesses the logical expression Year = 2023 and returns the Annual emissions if true, and 0 if false. Then, the SUM function sums across all these values for each country. Because the values for all other emission years were 0, it only sums the 2023 emissions.
</details>

*Hint 2*: explore how to sort the bars by right-clicking on the country variable and selecting "Sort..."

<details>
<summary>View suggested solution</summary>

1.	Drag the Annual CO2 emissions (per capita) field into the Columns shelf and either the Entity or Country Name field into the Rows shelf.
<br/>
2.	Drag the Year field to the Filters shelf. To show data from 2023 only, enter 2023 to 2023 in the Range of Values tab. Click OK.
<br/>
3.	Drag either the Country Name or Entity field into the Filters shelf. To show the top 10 countries with the highest CO2 emissions, click the Top tab in the window that pops up, select By formula and type `SUM(IIF([Year (co-emissions-per-capita.csv)]=2023, [Annual CO₂ emissions (per capita)], 0))`. Click OK.
<br/>
4.	To sort the bars from highest to lowest, right-click on the Entity (or Country Name) field in the Rows shelf, and click on "Sort...". Select "Field" under Sort By, choosing "Descending" in Sort Order, and Annual CO2 emissions in the Field Name. Then, exit the pop-up window by clicking on the X in the top right.
<br/>
5.	Name the graph "Countries with the highest CO2 emissions in 2023".

</details>

[NEXT STEP: Create a world map](create-world-map.html){: .btn .btn-blue }

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
