**Belly Button Biodiversity Dashboard**

This project is an interactive dashboard built to explore the Belly Button Biodiversity dataset, which catalogs the microbes found in human navels. The dashboard allows users to select individual samples and visualize the top microbial species (Operational Taxonomic Units, or OTUs) for each sample, along with additional information in a metadata panel. The data is visualized with a bar chart, a bubble chart, and demographic information, allowing insights into the microbial diversity of each sample.

Project Structure

index.html: The main HTML file, containing the structure of the dashboard and links to external scripts.
app.js: JavaScript file with D3 and Plotly code to fetch the JSON data, build interactive charts, and update the page dynamically based on user selections.
samples.json: The dataset file (referenced by URL in the code) containing microbial sample information, OTU IDs, and other demographic data.

Features

Dynamic Bar Chart: Displays the top 10 OTUs for the selected sample.
Interactive Bubble Chart: Shows all OTUs in the sample with marker size representing the OTU value and color coded by OTU ID.
Demographic Info Panel: Updates to display metadata for the selected sample.
Dropdown Menu: Allows the user to select different samples, which updates the charts and demographic information dynamically.

Setup Instructions

Prerequisites
Ensure you have:

An active internet connection to load external libraries (D3 and Plotly).
Visual Studio Code (or another code editor).
Python (if using the Python local server method).

**Running the Code**

Option 1: 
Visual Studio Code Live Server Extension
Open your project folder in Visual Studio Code.
Install the Live Server extension if you haven’t already.
Right-click on index.html and select "Open with Live Server".
Your browser should open automatically and display the dashboard at http://127.0.0.1:5500 or a similar address.

Option 2:
Using a Python Local Server
Open a terminal or command prompt in the project folder.
Start a simple HTTP server by running the following command:
bash
Copy code
python -m http.server
Open your browser and go to http://localhost:8000 to view the dashboard.

Usage
Open the dropdown menu at the top left to select a sample ID.

The dashboard will automatically update:

Bar Chart: Shows the top 10 OTUs for the selected sample.

Bubble Chart: Displays all OTUs in the sample, with marker size and color representing the OTU's prevalence and ID.

Demographic Panel: Updates with key information about the sample.

To explore other samples, select a new ID from the dropdown, and the charts and metadata will refresh.
