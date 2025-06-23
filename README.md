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
  <img src="/Image/" alt="India State Population Map" width="600"/>
</p>

---

## 🛠️ Requirements

Install the following Python libraries:

```bash
pip install geopandas pandas matplotlib
