# CSCE679 Data Visualization Assignment 1

Preview: https://peterchiang0101.github.io/CSCE679-Assignment1/

# Interaction log:

## Prompt:

In this task, you need to draw a **Matrix View** to visualize the **Monthly Temperature** of Hong Kong, where the color of each matrix cell encodes the temperature. You can find the data in temperature_daily.csv. You only need to focus on the last 10 years of data.

Here are the basic requirements:

1.  In the matrix, the x direction indicates the year, and the y direction indicates the month. Each cell indicates the corresponding month of a specific year.
2.  You need to visualize the maximum and minimum temperatures by month using the background color of each cell. Please use a mouse click to switch between the maximum and minimum temperatures.
3.  When hovering the mouse on each cell, a tip should appear to show the date and the temperature value.
4.  Add a mini line chart to each cell to show daily temperature changes. The x-axis represents the days in a month, and the y-axis represents the temperature.
5.  A legend is needed to show the mapping between colors and values.
6.  An example figure is attached.
7.  Use D3.js

Attachment: temperature_daily.csv, example figure

## Response:

Here is a complete, interactive D3.js implementation that meets all your requirements. It reads the temperature_daily.csv file, calculates the necessary monthly aggregations for the last 10 years, and builds the interactive matrix view with embedded mini line charts.

D3.js HTML Implementation
Save the following code as an index.html file in the same folder as your temperature_daily.csv file.

Attachment: index.html

---

## Prompt: 

can you spilt css and html?

## Response: 

Done! I've successfully separated the CSS and HTML:

Created files:

styles.css - Contains all stylesheet rules organized with clear section comments
Updated:

matrix.html - Replaced the embedded <style> block with a <link rel="stylesheet" href="styles.css" /> reference
Your workspace now has better separation of concerns with:

HTML structure in matrix.html
Styles in styles.css
Data in temperature_daily.csv
JavaScript remaining in matrix.html
This makes it easier to maintain and modify styles independently from the HTML markup!

---

## Prompt: 

can you seperate javascript?

## Response: 

Done! I've successfully separated the JavaScript into an external file. Here's what was created:

Created:

script.js - Complete JavaScript code with all functions, configuration, and data processing
Updated:

matrix.html - Now contains only HTML structure with references to external resources:
<link rel="stylesheet" href="styles.css" /> for styling
<script src="script.js"></script> for JavaScript logic
Your project now has a clean separation of concerns across three files:

matrix.html - HTML markup only
styles.css - All CSS styling
script.js - All JavaScript logic
temperature_daily.csv - Data file
This makes the code much more maintainable and follows web development best practices!

---

# Reflection:

I have not previously used D3.js, but with the help of GPT, the requirements were easily met. I am also learning how to write the correct version of the visualization from it.
