# Buldhana District Rainfall Analysis

An exploratory data analysis and visualization project using rainfall data from the talukas of Buldhana district, Maharashtra. The project focuses on comparing monthly rainfall patterns from June to September 2025 using Python and an interactive Plotly heatmap.

## Project Overview

This project analyzes rainfall measurements recorded across different talukas of Buldhana district.

The analysis uses rainfall data for:

- June 2025
- July 2025
- August 2025
- September 2025

The data is organized by **Taluka** and visualized using an interactive heatmap, making it easier to compare rainfall values across different locations and months.

##  Technologies Used

- **Python**
- **Pandas** – Data loading and manipulation
- **NumPy** – Numerical operations
- **Matplotlib** – Visualization library
- **Seaborn** – Data visualization
- **Plotly** – Interactive visualization

##  Dataset

The dataset contains rainfall measurements for different talukas in Buldhana district.

### Dataset Features

| Column | Description |
|--------|-------------|
| `Taluka` | Name of the taluka |
| `Jun-25` | Rainfall recorded in June 2025 (mm) |
| `Jul-25` | Rainfall recorded in July 2025 (mm) |
| `Aug-25` | Rainfall recorded in August 2025 (mm) |
| `Sep-25` | Rainfall recorded in September 2025 (mm) |

##  Analysis

The dataset is loaded using Pandas, and the rainfall columns for June–September 2025 are selected.
The `Taluka` column is used as the index to create a matrix suitable for visualization.

```python
month_columns = ['Jun-25', 'Jul-25', 'Aug-25', 'Sep-25']

df_heatmap_data = df.set_index('Taluka')[month_columns]
