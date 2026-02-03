---
layout: default
title: 1-Preparing your Data
nav_order: 2
parent: CO2 Emissions Activity
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Before you start
If you haven’t already, [download and install](https://www.tableau.com/academic/students){:target="_blank"} Tableau for Students.

If you have just finished with the Sales Data Activity, click on File > Close to start with a new project for this activity.

If you are just starting here, open Tableau Desktop and get familiar with the interface
- Discover Pane (right): Educational resources and links to relevant content
- Recent Flows (middle): Previous files are displayed here.
- Connections Pane (left): Select a data source

# Connecting to Data

For this activity, we will create visualizations about CO2 emissions per country, and relate that to the GDP (i.e., gross domestic product) per capita of each country. For that, we will use two different datasets, and will need to connect Tableau with both datasets. 

1. To get the datasets, download data for [Per Capita Co2 emissions by country](https://ourworldindata.org/grapher/co-emissions-per-capita?tab=table){:target="_blank"} and [GDP per capita](https://ourworldindata.org/grapher/gdp-per-capita-worldbank?tab=table){:target="_blank"}. You can find the download button below each table on the right. Then, click the Data tab and select Download full data. Open the zip file in the folder where you saved the data to (usually Downloads). You can see that they are .csv files, which are a type of text file.
   
2. Then, connect Tableau to these datasets. On the blue pane on the left, under **Connect**, click Text file. This will allow you to select one of the .csv files that you downloaded. Start with the gdp-per-capita-worldbank.csv file.

3. You can now view the spreadsheet in the bottom pane. As you can see, the column containing country names is called **Entity**. We want a more descriptive name, so we will rename that column. Hover over the top row of the sheet and click the arrow at the top right of the column called **Entity**. Select Rename and Rename this column to **Country Name**. Hover over the top row of this column and click the arrow again, then select Create Group. Click OK. This will allow Tableau to later automatically generate a map based on country names.

<img src="images\Tableau1-3.gif" alt="bottom toolbar" style="width:480px;">

4. Connect the second file that you downloaded. Click Add beside Connections on the top left and select Text file again. To join both spreadsheets, select the second spreadsheet under Connections, then click and drag the file name under Files (below Connections) to an empty space on the right.

5. You will see that both datasets will appear connected by a line, but an error icon signals that something is wrong with the relationship between the two datasets. In this case, you have to specify to Tableau which column should connect both tables. To this, we will use the box on the bottom left. Select Country Name under the GDP per capita file, the = symbol under Operator, and Entity under the CO2 emissions per capita file. This tells Tableau that these columns contain the same identifiers across both sheets. The error icon should disappear after this.

<img src="images\Tableau1-2.gif" alt="bottom toolbar" style="width:480px;">

6. You have now connected to the two datasets, and specified how they are linked by the Country Name column. Now save your file by clicking File > Save as on your computer toolbar. Since Tableau may crash from time to time, we recommend saving your work frequently by clicking File > Save.

[NEXT STEP: Create line graphs](create-line-graphs.html){: .btn .btn-blue }
