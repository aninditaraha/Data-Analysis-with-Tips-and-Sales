# Data Analysis Project: Tips and Sales Performance

## Project Overview

This project involves analyzing two datasets:

1. **Tips Dataset:** Contains information about tips and total bills.
2. **Sales Dataset:** Contains sales information, including quantities and values of products sold.

The goal of this analysis is to gain insights into tipping patterns, clean the sales data, and prepare it for further analysis. Visualizations are also provided to display trends.

## Datasets

- **`tips.xlsx`**: Dataset containing information about tips and bills.
- **`m35 (1).xlsx`**: Dataset containing sales data (SalesValue, SalesQty, and FocQty).

## Tools and Libraries Used

- **Python**: For data manipulation and analysis.
- **Pandas**: To load, clean, and process the data.
- **Matplotlib**: For data visualization.
- **NumPy**: Used for numerical operations.

## Data Cleaning and Processing

### Tips Dataset

1. Loaded the **tips** dataset.
2. Displayed basic information (first 10 rows, last 10 rows, columns, info, etc.).
3. Calculated a new column for tip percentage:  
   `Tip% = (tip / total_bill) * 100`
4. Summarized data using descriptive statistics.

### Sales Dataset

1. Loaded the **sales** dataset.
2. Cleaned columns by:
    - Removing extra characters (like 'AED', 'EA').
    - Handling missing values.
3. Converted numeric columns (e.g., `SalesValue(AED)`, `SalesQty(EA)`, and `FocQty(EA)`) to `float` for further analysis.
4. Dropped unnecessary columns to keep only the cleaned ones.

## Visualizations

Using **Matplotlib**, we created a simple plot as an example:

```python
import numpy as np
import matplotlib.pyplot as plt

# Sample plot for demo purposes
x = np.arange(1, 10)
y = x ** 2
plt.plot(x, y)
plt.title("Sample Plot")
plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.show()
