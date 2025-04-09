# Geospatial-mapping
Geospatial visualization of a list of some of the biggest football stadiums in Wales, it was achieved using Geopy and some other libraries.
This project was done using geopy library for geocoding  to create a geospatial visualization. I used API to extract information on the biggest football stadiums in Wales, checked the data for inconsistencies, cleaned it, and removed empty rows from the dataset using dropna(how='all) to ensure only valid data was processed.

I extracted latitude and longitude from a string column (latitude and longitude) using a custom function (extract_lat_lon), dropped rows where latitude and longitude could not be extracted to ensure accurate geospatial plotting, Parsed latitude and longitude values from the dataset, handling directional indicators (e.g., N, S, E, W) and converting them into floating-point numbers.
Created new columns (latitude and longitude) in the DataFrame to store the extracted coordinates, initialized a Folium map centered on Wales ([52.1307, -3.7837]) with an appropriate zoom level (zoom_start=8).

I added markers to the map for each stadium, using the extracted latitude and longitude for placement. I created interactive popups for each stadium marker, displaying detailed information such as: Stadium name, Capacity, Associated team(s), Postcode. I saved the generated map as an HTML file (welsh_football_stadiums.html) for viewing in a web browser, then used the folium library for map creation and marker placement.

The HTML file link when copied and pasted on the internet, shows a vivid Geospatial visualization of work done.
