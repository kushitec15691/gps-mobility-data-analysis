🛰️ GPS Mobility Data Processing & Visualization
This project demonstrates the full pipeline of cleaning, processing, and visualizing raw GPS data to uncover human mobility patterns. The dataset, originally captured in a non-standard format, was transformed into usable geospatial coordinates and visualized to extract meaningful insights such as trip segmentation, speed, and acceleration.

Developed by Kushmi Anuththara as part of an academic course at Dalarna University, this project simulates real-world challenges faced in urban planning, transportation research, and mobility analytics.

📌 Key Highlights
✅ Raw GPS data preprocessing: conversion from degrees-minutes to decimal degrees

✅ Speed, distance, and acceleration calculations

✅ Trip segmentation with Trip ID and Point ID generation

✅ Visualizations: heatmaps, scatter plots, and Folium-based interactive maps

✅ Insights into urban mobility trends through geospatial analytics

📂 Project Structure
File/Folder	Description
Lab2_Kushmi.ipynb	Jupyter notebook with all data cleaning, processing, and visualizations
kushmi_lab2.csv	Cleaned and transformed GPS data (including speed, trip ID, etc.)
gps_map.html	📍 Interactive Folium map showing GPS points and speed as popups
gps_map.png / gps_map_high_res.png	📷 Static map outputs for project presentation
Task2.1.png, Task2.2.png	Density heatmaps and scatter plots of GPS data
Lab2_KushmiAnuththara.pdf	Final project report with reflection and discussion on data quality

🔧 Data Cleaning and Processing Steps
Conversion of GPS Coordinates

From degree-minute (e.g. 60267285) ➝ Decimal degree format

Feature Engineering

Trip ID, Point ID

Speed transformation from raw values to km/h

Date and time formatting

Distance and time difference between consecutive points

Acceleration and average speed per trip

Quality Control

Addressed missing values, altitude placeholders, and format inconsistencies

Verified output using visual validation (plotted GPS trajectories)

📊 Visualization Outputs
🌍 World Map with Markers: Points plotted using Folium with popup speeds (see gps_map.html)

🔥 Heatmap: Density of GPS recordings to spot high-activity zones

🧭 Scatter Plot: Trajectory visualization using latitude vs. longitude

🧠 Additional metrics: Trip distance, duration, average speed and acceleration

🧪 Technologies Used
Python (pandas, numpy, geopy, matplotlib, seaborn)

Folium for interactive maps

Jupyter Notebook for analysis workflow

📝 Reflections
✔️ What is the value of GPS data?

✔️ Is GPS data always reliable? What are its limitations?

✔️ How can you evaluate the quality of GPS data?

These were answered in detail in the included PDF report Lab2_KushmiAnuththara.pdf.

🚀 How to Run
bash
Copy
Edit
git clone https://github.com/kushitec15691/gps-mobility-analysis
cd gps-mobility-analysis
jupyter notebook Lab2_Kushmi.ipynb
📍 Ideal For
Urban Mobility Modeling

Transport and Trip Behavior Research

Location Intelligence Projects

Spatial Data Cleaning Practice
