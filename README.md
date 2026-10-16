# Purpose

This code generates state-level choropleth maps for the contiguous United States using Python, `geopandas`, and Census data. The visualizations use a gradient to display key demographic shifts over time.

---

## Data Sources

The maps use historical datasets from the US Census Bureau and USDA:
* **Urbanization**: Taken from Census historical data (`pop-urban-pct-historical.xls`) as `statedata.csv`.
* **Agricultural Activity**: Derived from USDA Census of Agriculture reports (`ag-number-of-farms.xls`), cleaned and processed into `farmdata.csv` (fixed minor formatting issues).
* **Family Size**: Taken from Census Table ST-F1 reports (`tabst-f1-1990.xls` and `tabst-f1-2000.xls`) as `1990familydata.csv` and `2000familydata.csv`.
* **Geospatial Shapefiles**: Uses the Census state boundary shapefile (`cb_2018_us_state_5m.zip`) to render the maps.

---

### Dependencies
Ensure you have the following Python packages installed:
```bash
pip install geopandas pandas matplotlib
