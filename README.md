# Spotify-Data-Analysis

## Overview  
This project explores and visualizes a dataset of Spotify tracks to uncover trends in music over the years, such as track durations, popularity, and other audio features.  

## Dataset  
- **Source:** `tracks.csv` (contains Spotify music track metadata)  
- **Key Columns:**  
  - `name` – Song title  
  - `artists` – Artist(s)  
  - `duration` – Duration in milliseconds  
  - `popularity` – Popularity score  
  - `year` – Release year  
  - Other audio features like danceability, energy, tempo, etc.  

## Tools & Libraries  
- **Python 3**  
- `numpy`, `pandas` – Data manipulation  
- `matplotlib`, `seaborn` – Data visualization  

## Analysis Performed  
- **Data Loading & Inspection**
  - Viewing dataset with `.head()`  
  - Checking for null values  
  - Inspecting dataset info with `.info()`  

- **Data Exploration**  
  - Sorting tracks by popularity  
  - Analyzing year-wise trends in track durations  
  - Visualizing relationships between audio features and popularity  

## Example Visualization  
```python
fig_dims = (18, 7)
fig, ax = plt.subplots(figsize=fig_dims)
sns.barplot(x=years, y=total_dr, ax=ax, errorbar=None)
ax.set_title('Year vs Duration')
plt.xticks(rotation=90)
plt.show()

## How to Run
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/radhishukla/Spotify-Data-Analysis/blob/main/Spotify_Data_Analysis.ipynb)    
1. **Clone** this repository or download the notebook.  
2. **Install dependencies:**  
   ```bash
   pip install numpy pandas matplotlib seaborn
3. **Open** the notebook in Jupyter Notebook or Google Colab.
4. **Run** cells step-by-step to reproduce the analysis.

## Future Improvements
- Add interactive visualizations using Plotly or Dash
- Perform correlation analysis between audio features and popularity
- Build a predictive model for song popularity
