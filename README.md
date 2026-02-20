# Seoul Bike-Sharing: Demand Forecasting and Resource Optimization

This repository presents a data-driven framework for managing bicycle rental demand in Seoul. The project is divided into two comprehensive phases: **Demand Prediction** and **Strategic Allocation Optimization**. By utilizing historical hourly rental data, this project aims to minimize logistical costs and maximize user satisfaction through precise forecasting and mathematical optimization.

## Project Overview

To address the challenges of escalating bicycle rental demand, we developed a two-stage solution:
1. **Predictive Modeling:** Analyzing temporal patterns and employing machine learning to forecast demand.
2. **Strategic Optimization:** Using mathematical programming to allocate resources across the network based on those forecasts.

---

## Repository Structure

The project is implemented in two Jupyter Notebooks:

### 🚲 [Phase 1: Demand Prediction](Bike_Sharing_Problem_Phase1.ipynb)
The initial phase focuses on exploratory data analysis (EDA) and the development of robust forecasting models.
* **Temporal Analysis:** Exploration of rental variations by hour, season, and day of the week.
* **Statistical Modeling:** Parameter estimation and distribution fitting for rental data.
* **Machine Learning:** Comparison of multiple forecasting methods:
    * **ARIMA:** Capturing temporal patterns and magnitude.
    * **Linear Regression:** Establishing a baseline feature-dependent model.
    * **Random Forest:** Selected as the top performer for its high accuracy and ability to handle seasonal peaks.
* **Validation:** Implementation of cross-validation and hyperparameter tuning to ensure model reliability.

### ⚙️ [Phase 2: Strategic Allocation Optimization](Bike_Sharing_Problem_Phase2.ipynb)
In the second phase, the forecasts are integrated into an optimization framework to manage bike distribution across station pairs.
* **Demand Distribution Matrix:** Creating a detailed flow matrix between station pairs using statistical simulations (Normal and Exponential distributions).
* **Mathematical Framework:** Defining objectives and constraints to solve the bike allocation problem optimally.
* **Optimization with PuLP:** Implementing a flexible model to determine the optimal daily bike allocation for each station while minimizing operational costs.

---

## Technologies Used

* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning & Stats:** `scikit-learn`, `statsmodels` (ARIMA)
* **Optimization:** `PuLP`
* **Visualization:** `matplotlib`, `seaborn`, `mplcyberpunk`

---

## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn statsmodels pulp mplcyberpunk
    ```
3.  **Run the analysis:**
    * Execute `Bike_Sharing_Problem_Phase1.ipynb` to generate the demand forecasts.
    * Execute `Bike_Sharing_Problem_Phase2.ipynb` to apply the optimization model for station allocation.

---

## Authors

* **Mohammadarman Maghsoudi**
* **Ali Jahanshahi**
