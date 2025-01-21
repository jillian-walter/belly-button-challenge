# belly-button-challenge
HTML/Javascript Interactivity Challenge for Penn Data Science &amp; Visualization Bootcamp.
This challenge utilizes CSV data from Rob Dunn Lab's BellyButton Biodiversity Study, located at https://robdunnlab.com/projects/belly-button-biodiversity/. HTML and Javascript are used to create the interactive website in which users can explore findings from the bellybutton culture study.

Within the HTML file "Index_JW", we pull in multiple references/libraries using the to formulate the styling, interactivity and charts that will be featured on the website, listed below:

- CSS Stylesheet vis href, preset structure: https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css
  
- Plot structure from D3 Library using <script src=>: https://d3js.org/d3.v7.min.js
  
- Plot structure from Plotly using <script src=>: https://cdn.plot.ly/plotly-latest.min.js
  
- Supporting Javascript file using <script src=>: local drive file appJW.js


Within Javascript, we start by selecting the dataset (samples.json) and creating three functions that will be called to later in the code to create the dropdown menu and two supporting charts. The first, which will be called last, is the startDashboard function, which launches the interactive dashboard on HTML with a set sampleID to appear when the site is first opened. 
The function startDashboard iterates through each row of the JSON file and appends the value of each sampleID to the dropdown menu. 

Next, we work on the function for the charts in the dataset. Using Plotly and D3, we create a Bar Chart which details the number of each bacteria found in a given sample. Using the slice function, we order the top 10 bacteria types in descending order along the Y axis of the horizontal bar chart. Hover and callout features are added for easy readability.




