# What is the best source of protein for me? The nutritional and environmental cost of foods 

### 1. Description
A collection of data visualizations about the environmental costs of 50 protein-rich foods. The project aims to graphically relate data from foods' nutrients of animal, dairy, and plant-based protein sources with their impact, measuring greenhouse gas emissions, wasted water, and land use in the production. 


### 2. Statement
Nowadays, the search for protein-rich foods is on the prescription of many fitness and muscle-building diets. But what else are we consuming along with these proteins? The idea of these charts is to support us in making a more holistic decision about the food we eat by measuring nutritious qualities beyond the protein, along with their impacts on the environment in their production. 
The data visualizations include a radar chart, a progress bar chart, and a network of nodes and edges. The radar model presented a convenient way to broadly cover both the nutritional qualities and the environmental production costs. With eight axes equalized for a 100g portion, several variables can be showcased in different scales of measure and proportions. 

The progress bar was used as a way to express portions within the 100g portion. This distribution clearly shows the differences in portion sizes among the three categories, with the animal source presenting significantly fewer servings than the other two categories. This suggests that a holistic decision may consider multiple related factors. A typical portion of beef steak, for instance, despite causing an extremely high cost to the environment, is enough to provide a good amount of protein.

Finally, the network graph served to generate classic and nutritionally meaningful pairings within the 50 foods studied, focusing on creating well-balanced, high-protein meals. It connects pairs of nodes that represent the foods, illustrated by their images, through edges colored by the mix of the categories’ colors, with thickness proportional to the level of connection — strong, moderate, or acceptable.


### 3. Workflow
The project was executed in three main stages: gathering and managing data, designing the visualizations, and executing in Python. It was necessary to: 1. Gather data from the food nutrients and qualities, as well as data on their environmental costs; 2. Clean and manage each of the data sets separately; 3. Select meaningfully the foods to be worked with, considering protein value, balance among categories, raw ingredients, and, mainly, that which coincides in both data sets; 4. Merge both data sets, creating adequate matches among the foods; 5. Sketch the series of graphs in the same visual language that supports average people’s decisions about their meal decisions, while working with tangible measures and dimensions of those foods; 6. Research pictures of the foods, as well as manipulate them; 7. Create the dynamic graphics using the Plotly library; 8. Styling the graphs with specific libraries within Plotly; 9. Export the files in HTML.

The sources of data are the US Department of Agriculture for nutrition values and Our World in Data for environmental data. The first one offers an API, and the second is possible to download a spreadsheet in .csv format with the data, thus data will be gathered from it locally. The coding for the project was built based on the libraries: Pandas, for data manipulation, and plotly for the execution of the graphs. It was used with plotly.express, and plotly.graph_objects, networkx. 

A challenge for this project was to figure out a way to join both datasets since there was no common ID or variable, and the item descriptions were different in most cases. To circumvent this issue, the matches were made manually. In addition, to properly compare the quantities of each quality of the foods, it was necessary to research what is considered a typical serving of each food. Another challenge was to learn the graphs libraries at the same time as seeking certain autonomy to create an appealing and consistent visual identity throughout the several visuals.


### 4. Further uses
The next primary step will be to build and publish a website on which the interactive charts will be plotted the interactive charts, followed by textual information about the project context and research. In addition, the radar and portion charts could benefit from the pictures used in the network graphic, guaranteeing the visual identity of, and the easy understanding of, the foods that are being compared.

In that sense, a possibility for further exploration would be to test ways to quantify the measure units of the environmental costs visually. For instance, the land used could be measured by baseball courts, and the water wasted by gallons or bottles. 

Other minor improvements in the charts are welcome, such as the highlight of the radar polygons by the hover, and the creation of a chart that would present all the radars side by side. Along with the network chart, it is possible to create a calculator that could sum all the variables explored while the user selects the food nodes. 


### 5. Files list
The files were cleaned up before submitting, in order to demonstrate the final workflow. A note is that each of the files had a few attempts and directions switched before the final result. 

658-nutrition-emssion-match-3.csv
Created to manually match both datasets, from the USDA and The World in Data.

aliceviggiani-664-nutrition-environment-3.csv
List of the foods, along with information about the portions, nutritional qualities, and environmental costs. It was the base for the other ones. 

658-nutrition-radar-2.csv
658-nutrition-emssion-nodes-7.csv
658-nutrition-emssion-edges-9.csv
Supportive spreadsheets for specific uses, as the radar or network chart

aliceviggiani-664-food-radar-1.ipynb
aliceviggiani-664-food-chart-1.ipynb
aliceviggiani-664-food-network-1.ipynb
Python notebook to create the graphs

aliceviggiani-664-food-radar-1.html
aliceviggiani-664-food-chart-1.html
aliceviggiani-664-food-network-1.html
The HTML generated to visualize and interact with the graphs.
