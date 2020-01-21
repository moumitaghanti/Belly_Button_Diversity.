# Belly Button Biodiversity

![Bacteria by filterforge.com](Images/bacteria_by_filterforgedotcom.jpg)

In this assignment, you will build an interactive dashboard to explore the [Belly Button Biodiversity DataSet](http://robdunnlab.com/projects/belly-button-biodiversity/).

## Step 1 - Plotly.js

Plotly.js is used to  build interactive charts for your dashboard.

* A PIE chart is created, that uses data from samples route (`/samples/<sample>`) to display the top 10 samples.

  *  `sample_values` as the values for the PIE chart.

  *  `otu_ids` as the labels for the pie chart.

  *  `otu_labels` as the hovertext for the chart.

  ![PIE Chart](Images/pie_chart.png)

* A Bubble Chart is created to use data from samples route (`/samples/<sample>`) for visualization.

  * `otu_ids` for the x values.

  * `sample_values` for the y values.

  *  `sample_values` for the marker size.

  * `otu_ids` for the marker colors.

  * `otu_labels` for the text values.

  ![Bubble Chart](Images/bubble_chart.png)

* Displays the sample metadata from the route `/metadata/<sample>`

  * Displays each key/value pair from the metadata JSON object somewhere on the page.

* All of the plots are updated any time with a new sample is selected.

* An example dashboard page might look something like the following.

![Example Dashboard Page](Images/dashboard_part1.png)
![Example Dashboard Page](Images/dashboard_part2.png)

## Step 2 - Heroku

Flask app is deployed to Heroku.

* You can use the provided sqlite file for the database.

* Ask your Instructor and TAs for help!

- - -

## Advanced Challenge Assignment (Optional)

The following task is completely optional and is very advanced.

* Adapt the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the Weekly Washing Frequency obtained from the `/metadata/<sample>`route.

* You will need to modify the example gauge code to account for values ranging from 0 - 9.

* Update the chart whenever a new sample is selected.

![Weekly Washing Frequency Gauge](Images/gauge.png)

- - -

## Flask API

Use Flask API starter code to serve the data needed for your plots.

### The Heroku app link is
https://bellybutton-app-2019.herokuapp.com/