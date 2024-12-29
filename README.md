# Google Trends Analysis

This project analyzes Google Trends data for specific keywords ("Electric Cars," "Hybrid Cars," and "Gasoline Cars") using the Python pytrends library. The analysis includes search interest over time, regional interest, top charts, and related queries, with visualizations to help interpret the data.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Visualizations](#visualizations)
- [Code Overview](#code-overview)
- [Error Handling](#error-handling)
- [License](#license)
- [Author](#author)

## Installation

To run this project, you need Python 3.x installed. Install the required dependencies by running:

```bash
pip install pytrends pandas matplotlib seaborn
```

## Usage

1. Clone this repository:
```bash
git clone https://github.com/Neeraj-NN/Google-Search-Analysis.git
cd Google-Search-Analysis
```

2. Run the Python script:
```bash
python trends_analysis.py
```

3. The script will fetch Google Trends data, analyze it, and produce visualizations.

## Features

- **Interest Over Time**: Tracks search trends for the specified keywords over the last 5 years in India
- **Interest by Region**: Highlights the top regions for search interest in "Electric Cars"
- **Top Charts**: Fetches trending topics globally for the year 2023
- **Related Queries**: Identifies associated queries for the specified keywords
- **Data Visualization**: Creates clear and informative charts using matplotlib and seaborn

## Visualizations

### 1. Search Trends Over Time
A line graph showing the search trends for "Electric Cars," "Hybrid Cars," and "Gasoline Cars" over the past five years.

### 2. Regional Interest
A bar chart displaying the top 10 regions with the highest search interest for "Electric Cars."

## Code Overview

### Libraries Used
- `pandas`: For data manipulation
- `pytrends`: To interface with Google Trends
- `matplotlib` and `seaborn`: For creating visualizations

### Key Sections

1. **Interest Over Time**: Fetches and displays search interest trends over the past 5 years:
```python
data = pytrends.interest_over_time()
```

2. **Regional Interest**: Sorts and displays the top regions for a given keyword:
```python
region_data = pytrends.interest_by_region()
```

3. **Visualizations**:
   - Line plot for search trends
   - Bar chart for regional interest

## Error Handling

The script includes error handling for:
- Empty or missing data from the Google Trends API
- Network connectivity issues
- Invalid configurations or keyword inputs

## License

This project is licensed under the MIT License.

## Author

- **Neeraj Nair**
- Email: Neerajnsnair2000@gmail.com
