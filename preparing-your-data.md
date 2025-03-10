---
layout: default
title: 1-Preparing your Data
nav_order: 2
parent: CO2 Emissions Activity
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

If you haven’t already, [download and install](https://www.tableau.com/academic/students) Tableau for Students

Open Tableau Desktop and get familiar with the interface
- Discover Pane (right): Educational resources and links to relevant content
- Recent Flows (middle): Previous files are displayed here.
- Connections Pane (left): Select a data source

# Connecting to Data
1. Download data for [Per Capita Co2 emissions by country](https://ourworldindata.org/grapher/co-emissions-per-capita?tab=table) and [GDP per capita](https://ourworldindata.org/grapher/gdp-per-capita-worldbank?tab=table). You can find the download button below each table on the right. Then, click the Data tab and select Download full data. Open the zip file in the folder where you saved the data to (usually Downloads).

2. On the blue pane on the left, click Text file. This will allow you to select one of the .csv files that you downloaded.

3. You can now view the spreadsheet on the bottom pane. Hover over the top row of the sheet and click the arrow at the top right of the column. Select Rename and Rename this column to Country Name on both sheets. Hover over the top row of this column and click the arrow again, then select Create Group. Click OK. This will allow Tableau to later automatically generate a map based on country names.

4. Connect the second file that you downloaded. Click Add beside Connections on the top left and select Text file again.

5. To join both spreadsheets, select the second spreadsheet under Connections, then click and drag the file name under Files (below Connections) to an empty space on the right. 

6. To the left of the spreadsheet on the bottom, select Country Name under the GDP per capita file, the = symbol under Operator, and Entity under the CO2 emissions per capita file. This tells Tableau that these columns contain the same identifiers across both sheets. As you can see on the spreadsheet to the right, the two files have now been combined.

7. Save your file by clicking File > Save as on your computer toolbar. Since Tableau may crash from time to time, we recommend saving your work frequently by clicking File > Save.

