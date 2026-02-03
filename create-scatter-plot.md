---
layout: default
title: 3-Create a scatter plot
nav_order: 4
parent: CO2 Emissions Activity
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---
# Create a scatter plot

Start a new sheet by clicking the icon to the right of the sheet you created.

<img src="images\Tableau 3-1.png" alt="bottom toolbar" style="width:480px;">

Now, create a scatter plot showing the relationship between CO2 emissions per capita and GDP per capita across all countries for the past decade.

<details>
<summary>View suggested solution</summary>

1.	Under the CO2 emissions table heading on the left pane, click and drag the **Annual CO2 emissions (per capita)** field to the Rows bar. Under the GDP per capita table heading, click and drag the **GDP per capita field** to the Columns bar. Click and drag the **Country Name** field (under the same heading) to the Marks shelf. There, click the icon beside Country Name and select Colors. You have created a scatter plot with cumulative CO2 emissions per capita (cumulative because Tableau is doing by default the sum of emissions per country, as you can see under Columns and Rows on the top) on the y-axis and cumulative GDP per capita on the x-axis from 1750-2023, with a legend showing countries.
<br/> 
   <img src="images\Tableau-3-1.gif" alt="bottom toolbar" style="width:480px;">
<br/>       
2.	To specify a time frame for the chart, drag the Year field from under either table heading to the Filters shelf. Enter a year range, such as 2013 to 2023 (os use the most recent year available, the dataset is updated over the years). Click OK.
<br/>
   <img src="images\Tableau-3-2.gif" alt="bottom toolbar" style="width:480px;">
<br/> 
3.	Name the chart CO2 Emissions by GDP per Capita per Country (2013-2023).
4.	Rename the y-axis to "Cumulative annual CO₂ emissions (per capita)" and the x-axis to "GDP per capita"

</details>

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

[NEXT STEP: Create a bar graph](create-bar-graph.html){: .btn .btn-blue }
  
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
