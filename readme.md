# US Electoral College Analysis


This project focuses on the electoral college voting system in the United States. The electoral college is solely used to elect the president and vice president, and requires a simple majority of votes in order for a candidate to be elected. The notebooks contained in this repository include an analysis of state populations, the number of electoral college votes each state is apportioned, and visualizations to better understand the dynamics of population and state voting power. Primarily, this project can help illustrate how a presidential candidate is elected to office even if they lose the popular vote. (To note, all other elections use the popular vote to fill political roles.)

## Contents

### Jupyter Notebooks
1.) 1_historical_electoral_college_data.ipynb: Retrieves data from a table in the electoral college wikipedia article (https://en.wikipedia.org/wiki/United_States_Electoral_College), and cleans and saves it for use in later notebooks.

2.) 2_population_data.ipynb: Explores data from the US Census Bureau 2020 population results.

3.) 3_electoral_college_representation: Illustrates the distribution of electoral college votes by state and analyzes the data for representation imbalance.

4.) 4_electoral_voting_visualized.ipynb: Visualizes each state’s population, electoral representation, and voting power. Compares state population to electoral representation.

### Images:
Static images are embedded in some markdown cells; some are to show a static image of a visualization, others are to show the challenges of certain code blocks.
### HTML files:
The interactive visualizations do not render in github, saving the files as .html preserves the underlying data. These files can then be linked in a markdown file and viewed in the browser. (For more info see the “Visualizations” title below.)


## Data
* The population data comes from the US Census Bureau’s 2020 results (table 2): https://www.census.gov/data/tables/2020/dec/2020-apportionment-data.html
* A Kaggle utility dataset based on the 2020 census contained some incorrect population values but was used to format the table used in the notebooks as well as the state abbreviations: 
https://www.kaggle.com/datasets/alexandrepetit881234/us-population-by-state
* The electoral college data comes from the wikipedia page “United States Electoral College: Chronological Table”: 
https://en.wikipedia.org/wiki/United_States_Electoral_College#Chronological_table


## Python Version and Libraries

Python 3.14

* pandas: https://pandas.pydata.org/
* matplotlib: https://matplotlib.org/
* plotly: https://plotly.com/python/choropleth-maps/
* requests: https://pypi.org/project/requests/
* Beautiful soup: https://beautiful-soup-4.readthedocs.io/en/latest/
* csv: https://docs.python.org/3/library/csv.html
* re (regex): https://docs.python.org/3/library/re.html

See the requirements.txt file for all the libraries and versions used in the notebooks. 

### Visualization Displays

Some of the visualizations used in the fourth notebook (4_electoral_voting_visualized.ipynb) are created using the plotly’s choropleth interactive maps. The map displays are not included in the notebook due to github’s rendering, which strips the javascript functionality. For this reason, the static images are embedded in a markdown after the code block. There is also a link to the github page for the html of the visualization, which keeps the interactivity intact. 

### LLM Usage

Claude facilitated my ability to learn how to retrieve (scrape) data from a webpage, create some of the example legends and devices in visualizations, and debug why the choropleth maps were not displayed in my github repo.  Otherwise, all other code blocks, markdowns, insights, and decisions were my own.



