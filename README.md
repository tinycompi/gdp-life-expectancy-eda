# GDP & Life Expectancy - Exploratory Data Analysis

### Project Overview
This project explores the correlation between the economic output (GDP) of various nations and the life expectancy of their citizens from the years 2000 to 2015. 

Using data provided by the World Health Organization (WHO), this script utilizes Python's Data Science stack to clean, transform, and visualize the data. Because economic data is often heavily skewed, this project implements logarithmic transformations and custom axis formatting to generate accurate linear regression models and readable visualizations.

### 🛠️ Tech Stack
* **Language:** Python 3
* **Libraries:** `pandas`, `seaborn`, `matplotlib`, `numpy`
* **Concepts:** Data Visualization, Logarithmic Transformations, Linear Regression, Facet Grid Mapping, Custom Ticker Formatting

---

### 📊 Key Features & Visualizations
* **Data Wrangling:** Uses `pandas` to load, rename, and clean the raw WHO dataset.
* **Log-Transformation:** Applies a `numpy` log10 transformation to the GDP data to normalize the heavily skewed economic figures, allowing for accurate linear regression mapping.
* **Custom Matplotlib Formatting:** Implements a custom `FuncFormatter` to convert scientific notation (e.g., `1e12`) back into human-readable financial figures (Trillions, Billions, Millions) on the y-axis.
* **Faceted Scatter Plots:** Utilizes `seaborn.lmplot` to generate a dynamic grid of scatter plots with overlaid regression lines, separated by country, to easily compare disparate global economies.

---

### 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Ensure both the Python script and `all_data.csv` are in the same directory.
3. Run the script in your terminal to generate the Matplotlib visualization:
   `python script.py` *(Update this if you named your file something else!)*
