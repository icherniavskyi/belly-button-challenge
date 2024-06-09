# belly-button-challenge

# Interactive Dashboard for Bacterial Data Visualization

## Overview
This interactive dashboard is designed to visualize bacterial data samples using D3.js and Plotly.js. It fetches data from a JSON source, displays metadata, and constructs dynamic charts based on user selection from a dropdown menu.

## Features
- **Metadata Display**: Show metadata for a selected bacterial sample.
- **Bubble Chart**: Displays the bacteria cultures per sample; the pixel size of the bubble is determined by sample size.
- **Bar Chart**: Shows the top 10 bacterial species (OTUs) in a horizontal bar chart.

## Folders & Files
### static\js folder: folder contains main js script for rendering and managing visualization;
- `app.js`: Contains all JavaScript functions for fetching data, rendering charts, and managing user interactions.
### main folder:
- `index.html`: The HTML file that hosts the dashboard.
- `sample.json`: JSON file conaining bacterial data samples.

## Usage
1. **Starting the Dashboard**: Open the `index.html` in a web browser to start the application.
   - Altenative: You can use this link: [belly-button-challenge](https://icherniavskyi.github.io/belly-button-challenge/) to access static web page hosting visualization.
3. **Selecting a Sample**: Use the dropdown menu to select a sample. The metadata and charts will update automatically based on the selected sample.

## JavaScript Functions
- `buildMetadata(sample)`: Fetches and displays metadata for a selected sample.
- `buildCharts(sample)`: Builds both a bubble chart and a bar chart for the selected sample.
- `init()`: Initializes the dashboard by populating the dropdown menu and loading the initial visualizations.
- `optionChanged(newSample)`: Called when a new sample is selected from the dropdown menu.

## Libraries Used
- D3.js: For manipulating documents based on data.
- Plotly.js: For building interactive charts.

## Data Source
The data is fetched from a static JSON file hosted at `https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json`.
  - Alternative: You can access data by openning the `sample.json` file in the main folder.
