# Wildfire mapping project



**Summary:**

This project is about mapping wildfires in the whole world to answer the project question: "Where have wildfires occured in the past five days and how strong were they?". The final result includes two maps that map wildfires across the whole world with either Point- or hexbin data.



**Data Sources:**

The Point data to map the wildfires was obtained through Nasa's Fire Information for Resource Management System (FIRMS).

* API: https://firms.modaps.eosdis.nasa.gov/api/data\_availability/
* Nasa's map: https://firms.modaps.eosdis.nasa.gov/map/#d:24hrs



**Setup Instructions:**

To run this code, Python and the following libraries are required:

\- geopandas

\- matplotlib

\- cartopy

\- geodatasets

\- pandas

\- numpy



The project was developed using a Conda environment and all required packages are listed in the "environment.yml" file too.



**Execution instructions:**

Assuming all setup instructions have been followed you have to run the code from top to bottom. It is especially important to refresh cell 5, the one that loads new data from firms via the API, in order to get a current/correct map. In the second line of each map you can put your wished continent that you want to visualize (continent\_extent = \*your wished continent\*). For example north\_america, europe, earth etc. To see what exactly is possible look at cell 2 where all options are listed. If you wish to visualize a part of the map that is not already in the list you can do so by adding the coordinates of that region in the same way as they are there. However it is not guaranteed that the visualization will be good (especially for very small regions).



The first map that is created is done with raw Point data and shows every single satellite fire detection but only shows the FRP (Fire Radiative Power\~ Fire power) from 1-40 because of better visualisation. It also has a little text box that states the top 3 countries with the most Fire detections of the past 5 days.

The second map is done by aggregating the Point data to create a hexbin map. This makes for a better visualization, especially for each of the continents. It can also display FRP from 1-1000 and is therefore better for looking at fire strength.









Project Title \& Description: A one or two-sentence summary of the spatial question you are answering.



Data Sources: Explicit links to where the raw open data was obtained.



Setup Instructions: Exactly what software and libraries are required to run the code (e.g., pointing to an environment.yml or requirements.txt file).



Execution Order: Clear instructions on how to run the project (e.g., “Run the data\_cleaning.ipynb notebook first, followed by spatial\_analysis.ipynb”).

