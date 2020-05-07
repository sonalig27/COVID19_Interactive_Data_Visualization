# COVID19_Interactive_Data_Visualization
Built an interactive COVID19 data visualization tool using Python plotly and Dash

Problem statement:
Built an interactive web based tool for users to interact with to
visualise the real time data on the spread of the pandemic across the globe as well as across different states in the US
and compare the results across different countries as well as the states in the US and draw informative insights.

Dataset:
the publicly available dataset – “2019 Novel Coronavirus COVID-19 (2019-nCoV) Data Repository by Johns Hopkins CSSE”. 
source: https://github.com/CSSEGISandData/COVID-19/tree/master


Resources Used:
Header image displayed on the web-tool - source: https://www.stjosephshealth.org/images/covid19-header.jpg
Used a couple of Dashboards for reference:
https://coronavirus.1point3acres.com/en
https://www.worldometers.info/coronavirus/country/us/
https://indiasmile.org/covid
The tutorials and examples on the plotly and Dash reference Documentation were really very helpful.
Plotly Docs :https://plotly.com/python/
Dash Docs: https://dash.plotly.com/


dependencies:
As we are using plotly and dash to generate the interactive data visualization graphs for our web tool.
We need to install numpy, pandas, plotly, dash, dash-renderer, dash_html_components, dash_core_components.
We can install this dependencies using following comman in our jupyter notebook:

1) !pip install pandas
2) !pip install numpy
3) !pip install plotly
4) !pip install dash
5) !pip install dash-renderer
6) !pip install dash_html_components
7) !pip install dash_core_components
8) pip install dash_table


how to run:
1) after installing all the dependencies mentioned above, execute all the cells in the jupyter notebook.
2) as the dash application runs on a web browser and it runs by default on the local server,
on executing the last cell in the jupyter notebook the server link will be displayed, click on the link to see the output web portal.
3) Web portal will open up in a different tab, it will display the project generated output(graphs and tables).
4) user can provide input for the slider, dropdowns, textbox to display the realtime interactive plots according to user selection.
6) On hovering over the graphs the mouse pointer will show the corresponding plot details.
5) every graph has multiple options namely:
 download as png, zoom-in, zoom-out, pan, select (to display only the specific selected area of graph), etc.
7) even the tables displayed will take user input and display the number of records according to user selection.


Program working:
It is a web-based tool built using dash framework and ploty library. On executing the program based on following steps, a web portal opens up
and displays below details:
For country dataset:
1) Summary count of the worldwide COVID-19 confirmed cases, Active cases, deaths and recoveries
2) Slider to select the number of records to be displayed in the below mentioned table (step 3)
3) Interactive table displaying confirmed cases, active cases, deaths and recoveries 
	sorted in non-ascending order of confirmed cases coutry wise.
4) Interactive bar-graph showing confirmed cases, deaths and recoveries plotted date wise.
5) Dropdown to select confirmed cases/Active cases/Deaths/recoveries for generating the piechart (step 6)
6) Interactive pie chart for confirmed cases/Active cases/Deaths/recoveries across the countries in the world
7) Interactive Scatter plot displaying confirmed cases country wise (size of each bubble corresponds to confirmed case count of the country)
8) Interactive Line plot displaying deaths country wise
9) Interactive line plot with markers displaying recoveries country wise
10) text input for country name to generate the below scatter plot of step 11
11) Interactive Line plot with markers, showing summary of confirmed cases, Deaths, recoveries for a country date wise.
12) Interactive geo Choropleth plot displaying the country name, confirmed cases, Active cases, Deaths, recoveries on the mouse tool-tip
	with color scale corresponding to the confirmed case count.

For US dataset:
1) Summary count of the COVID-19 confirmed cases, Active cases, deaths and recoveries across the US
2) Slider to select the number of records to be displayed in the below mentioned table (step 3)
3) Interactive table displaying confirmed cases, active cases, deaths and recoveries 
	sorted in non-ascending order of confirmed cases state wise in the US.
4) Interactive bar-graph showing confirmed cases and deaths plotted date wise.
5) Dropdown to select confirmed cases/Active cases/Deaths for generating the piechart (step 6)
6) Interactive pie chart for confirmed cases/Active cases/Deaths across different states in the US
7) Interactive Scatter plot displaying confirmed cases state wise (size of each square corresponds to confirmed case count of the state)
8) Interactive Line plot with markers displaying deaths country wise
9) Interactive Scatter-geo plot displaying the states name, confirmed cases, Active cases, Deaths, recoveries on the mouse tool-tip
	with bubble size corresponding to the confirmed case count of the state.
