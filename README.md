# Trazmeo_assignment1
1. Record High and Low Temperatures (2005-2014) Visualization:
Objective: Visualize daily record highs and lows over a decade.
Logic:
Data filtered for years 2005-2014.
Grouped by "Day of Year" (MM-DD format) to find max (TMAX) and min (TMIN).
Shaded area between highs and lows to show temperature range.
Modules Used: Pandas (grouping), Matplotlib (line and fill_between plots).
2. 2015 Record Breakers Overlay:
Objective: Identify and overlay 2015 temperatures that broke historical records.
Logic:
Filter data for 2015.
Compare 2015 TMAX with historical TMAX, and TMIN with historical TMIN.
Plot scatter points for days when 2015 temperatures exceeded or fell below records.
Modules Used: Pandas (grouping and comparisons), Matplotlib (scatter overlay).
3. Handling Leap Days (February 29):
Objective: Ensure data consistency by removing leap days.
Logic:
Filter out rows where date is Feb 29.
Reason: Avoid issues in comparing daily records that do not exist every year.
Modules Used: Pandas (date filtering).
4. Clean Visualization (Legends, Labels, No Chart Junk):
Objective: Make graphs clear and professional.
Logic:
Added axis labels, titles, and legends.
Used consistent color schemes (Red for High, Blue for Low).
Avoided unnecessary chart elements (3D, excessive colors, etc.).
Modules Used: Matplotlib (custom formatting).
5. Mapping Station Locations (Interactive Map using Folium):
Objective: Plot station locations near Ann Arbor on an interactive map.
Logic:
Extract unique station IDs.
Use approximate coordinates (as dataset lacks explicit lat/lon).
Plot using Folium map markers.
Reason for Folium: Makes interactive maps easily explorable.
Modules Used: Folium (interactive maps).
6. Plotting Temperature Summary for 2015:
Objective: Daily TMAX and TMIN for 2015 to observe seasonal patterns.
Logic:
Pivoted data for easy plotting of TMAX and TMIN side by side.
Converted tenths of °C to °C.
Added proper titles, axis labels, and legend.
Modules Used: Pandas (pivot), Matplotlib (line plots).

Module	- Reason
Folium	- Interactive mapping. Easier to visualize spatial data than static maps.
Matplotlib	- High control over visualization elements for professional presentation.
Pandas	- Efficient handling of large datasets and time-series manipulations.
NumPy-	Simplifies numerical operations like array indexing and math operations.
