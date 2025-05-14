# 🛰️ GPS Mobility Data Processing & Visualization

This project demonstrates the full pipeline of **cleaning, processing, and visualizing raw GPS data** to uncover human mobility patterns. The dataset, originally captured in a non-standard format, was transformed into usable geospatial coordinates and visualized to extract meaningful insights such as trip segmentation, speed, and acceleration.

Developed by Kushmi Anuththara as a portfolio project for urban mobility modeling and geospatial analytics.

---

## 📌 Key Highlights

- ✅ Convert GPS coordinates from degrees-minutes to decimal degrees
- ✅ Calculate speed, distance, duration, and acceleration
- ✅ Segment trips and assign unique IDs to each point
- ✅ Create interactive maps, heatmaps, and scatter plots
- ✅ Apply data quality checks and transformation

---

## 📁 Project Structure

| File/Folder                  | Description |
|------------------------------|-------------|
| `Lab2_Kushmi.ipynb`          | Main Jupyter Notebook for data cleaning, processing, and visualization |
| `kushmi_lab2.csv`            | Cleaned dataset with trip and point IDs, speed, distance, acceleration |
| `gps_map.html`               | Interactive Folium map visualizing all GPS points |
| `gps_map.png` / `gps_map_high_res.png` | Static map outputs |
| `Task2.1.png`, `Task2.2.png` | Heatmap and scatter plot of point density and movement |
| `Lab2_KushmiAnuththara.pdf` | Final project reflection and summary |

---

## 🔧 Data Processing Workflow

### 1. Coordinate Conversion

Raw format (e.g., `60267285`) → Decimal degrees using:

### 2. Feature Engineering

- Create `Trip_ID` and `Point_ID`
- Convert time and date to readable format
- Calculate:
  - Speed (in km/h)
  - Distance between points
  - Time differences
  - Acceleration between points
  - Trip-level aggregates

### 3. Data Quality Handling

- Removed/handled placeholder values (e.g., `-1` for altitude)
- Visual verification of trajectory patterns using maps

---

## 📊 Visualization Outputs

| Visualization | Description |
|---------------|-------------|
| 🌍 `gps_map.html` | Interactive Folium map with popups for speed and location |
| 🔥 `Task2.1.png` | Heatmap showing high-density GPS activity areas |
| 🧭 `Task2.2.png` | Latitude vs. Longitude scatter plot for trip path |

---

## 🧪 Tools & Libraries Used

- Python: `pandas`, `numpy`, `math`, `geopy`, `datetime`
- Visualization: `folium`, `matplotlib`, `seaborn`
- Notebook: Jupyter

---

## 📝 Reflection (See Report)

The final report answers:
- What is the purpose of collecting GPS mobility data?
- Is GPS data always reliable? What are the limitations?
- How can we evaluate and ensure the quality of GPS data?

📄 See: `Lab2_KushmiAnuththara.pdf`

---

## 🚀 How to Run This Project

```bash
git clone https://github.com/kushitec15691/gps-mobility-data-analysis
cd gps-mobility-data-analysis
jupyter notebook Lab2_Kushmi.ipynb
