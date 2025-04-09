# Geospatial-mapping
Geospatial visualization of a list of some of the biggest football stadiums in Wales, it was achieved using Geopy and some other libraries.
# This project was done using Geopy create geospatial visualization. I Used API to extract information on the biggest football stadiums in wales
•	Checked the data for inconsistencies and cleaned it, removed empty rows from the dataset using dropna(how='all) to ensure only valid data is processed.
•	Extracted latitude and longitude from a string column (latitude and longitude) using a custom function (extract_lat_lon).
•	Dropped rows where latitude and longitude could not be extracted to ensure accurate geospatial plotting.
•	Parsed latitude and longitude values from the dataset, handling directional indicators (e.g., N, S, E, W) and converting them into floating-point numbers.
•	Created new columns (latitude and longitude) in the DataFrame to store the extracted coordinates.
•	Initialized a Folium map centered on Wales ([52.1307, -3.7837]) with an appropriate zoom level (zoom_start=8).
•	Added markers to the map for each stadium, using the extracted latitude and longitude for placement.
•	Created interactive popups for each stadium marker, displaying detailed information such as: Stadium name, Capacity, Associated team(s), Postcode
•	Saved the generated map as an HTML file (welsh_football_stadiums.html) for viewing in a web browser.
•	Used the folium library for map creation and marker placement.
•	Used the geopy library for geocoding (though not explicitly used in the provided code snippet, it is imported and may have been used for additional geospatial tasks).
