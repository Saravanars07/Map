# Map

# 🗺️ India State Population Elimination Map (GeoPandas)

This Python project visualizes the **state-wise population distribution of India** using GeoPandas and Matplotlib. It allows you to **"eliminate" states** either by:
- selecting a **cumulative population threshold**, or
- manually specifying **state names**.

The remaining states are then plotted on a map with **population labels**, making it an interactive and educational visualization tool.

---

## 📌 Features

- Loads India's state boundaries from a GeoJSON map file
- Allows two elimination modes:
  1. **Direction-based cutoff by population**
  2. **Manual state selection**
- Customizable cutoff direction: `north-south`, `south-north`, `west-east`, `east-west`
- Visualizes only the remaining states on the map
- Labels each visible state with its estimated **population (in millions)**

---

## 🖥️ Demo Output

<p align="center">
  <img src="/Image/Map.jpeg" alt="India State Population Map" width="600"/>
</p>

---

## 🛠️ Requirements
Install the following Python libraries:
```bash
pip install geopandas pandas matplotlib
```


## 🚀 How to Use
 1. Run the Script
  Run the script from your terminal or IDE:
  ```
  bash
  python state_population_map.py
  ```
 2. Choose Elimination Mode
  When prompted:
  ```
  Choose elimination method:
  1. Eliminate by cumulative population and direction
  2. Eliminate by specifying state names
  ```
  Option 1: Cumulative Population
    You'll be asked to enter:
  - Population cutoff (in millions), ```e.g. 600```
  - Direction of elimination:``` north-south```, ```south-north```, ```west-east```, ```east-west```.

  The script removes states in that directional order until the total population eliminated meets your cutoff.
  
  Option 2: Specify State Names
    You’ll be shown a list of available states. Enter names like:
   ``` 
   Bihar, Uttar Pradesh, Maharashtra 
   ```
---
## 🧠 How It Works
  - The script loads the India map using GeoPandas
  - It matches the state names with a pre-defined population dictionary
  - You choose how to eliminate states (by direction or by name)
  - Eliminated states are removed from the map
  - The remaining states are plotted with population annotations

---
## 🧩 Customization
  - 🔢 Update the population numbers in the state_populations dictionary
  - 🗺️ Replace the GeoJSON file with a newer version if needed
  - 🎨 Change the color scheme by editing:
  ```
  python
  remaining_map_dissolved.plot(ax=ax, color="lightgreen", edgecolor="black")
  ```
---

## 📘 License
This project is licensed under the MIT License. Feel free to fork, modify, and use it for educational or analytical purposes.

---

## 🙌 Acknowledgements
  - GeoPandas
  - matplotlib
  - [Survey of India GeoJSON data (via public domain sources)]
    
---

## 💬 Example Use Cases
  - Teaching state-wise population distribution
  - Simulating redistricting and demographic filters
  - Preparing base maps for further spatial analysis

---

## 👨‍💻 Author

Developed by Saravanars07
For suggestions or collaborations, feel free to open an issue or pull request.



