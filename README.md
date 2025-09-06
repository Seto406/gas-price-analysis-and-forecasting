# US Gas Price Analysis & Forecasting 📊

This project demonstrates an end-to-end data science workflow using a time-series dataset of U.S. weekly retail gasoline prices from 1993 to the present. The entire analysis is conducted in a Jupyter Notebook.

---
## Project Workflow

1.  **Data Loading & Preparation:** The project begins by loading clean, historical data from a SQLite database (`gas_prices.db`). The dataset is prepared for time-series analysis by converting the 'date' column to a proper datetime format and setting it as the index.

2.  **Exploratory Data Analysis (EDA):** I performed visual analysis to uncover trends and patterns:
    * Plotted the complete time-series to show price fluctuations over 30+ years.
    * Aggregated the data by year and created a bar chart to visualize long-term trends and identify years with the highest/lowest average prices.

3.  **Predictive Modeling (Machine Learning):**
    * Developed a simple linear regression model using **Scikit-learn** to predict the next week's gas price based on the previous week's price.
    * The model was trained on 80% of the historical data and evaluated on the remaining 20% (the test set) to measure its accuracy. The results show a high correlation between the model's predictions and the actual prices, as visualized in the final plot.

---
## Technologies Used

* **Language:** Python
* **Libraries:**
    * Pandas (for data manipulation)
    * Matplotlib & Seaborn (for data visualization)
    * Scikit-learn (for machine learning)
* **Environment:** Jupyter Notebook
* **Database:** SQLite

---
## How to Run

1.  Clone this repository to your local machine.
2.  Ensure you have the required libraries installed (`pip install pandas jupyterlab matplotlib seaborn scikit-learn`).
3.  Launch JupyterLab (`jupyter lab`) and open the `analysis.ipynb` notebook.
4.  You can run the cells sequentially to reproduce the analysis and model training. The `gas_prices.db` file is included in the repository and must be in the same directory.
