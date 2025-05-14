
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
