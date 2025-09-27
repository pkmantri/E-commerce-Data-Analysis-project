# E-commerce Data Analysis

This project analyzes **E-commerce sales data** using Python, Pandas,
NumPy, and data visualization libraries.\
It explores customer behavior, sales trends, and relationships between
different variables such as order count, price, and product categories.

## 📌 Features

-   Load and clean E-commerce dataset
-   Perform **exploratory data analysis (EDA)**
-   Handle missing values and data preprocessing
-   Generate descriptive statistics
-   Visualize sales trends using **Matplotlib & Seaborn**
-   Correlation analysis between numerical features (`order_count` vs
    `price`)

## 🛠️ Tech Stack

-   Python 3
-   Jupyter Notebook
-   Libraries:
    -   `pandas`
    -   `numpy`
    -   `matplotlib`
    -   `seaborn`

## 📂 Project Structure

    ecommerce.ipynb   # Main Jupyter Notebook with code & analysis
    README.md         # Project Documentation
    data/             # (Optional) Folder containing dataset

## ⚙️ Installation

1.  Clone this repository:

    ``` bash
    git clone https://github.com/pkmantri/ecommerce-analysis.git
    cd ecommerce-analysis
    ```

2.  Install dependencies:

    ``` bash
    pip install pandas numpy matplotlib seaborn jupyter
    ```

3.  Launch Jupyter Notebook:

    ``` bash
    jupyter notebook ecommerce.ipynb
    ```

## 📊 Key Analysis

-   **Sales Trends**: Analyzed sales data across products and
    categories.
-   **Correlation**: Used `numpy.corrcoef()` and `pandas.corr()` to
    measure correlation between:
    -   `order_count`
    -   `price`
-   **Visualization**: Created bar charts, histograms, and scatter plots
    to understand patterns.

Example correlation calculation:

``` python
import numpy as np
a = np.corrcoef(df["order_count"], df["price"])
print("The correlation is", a[0,1])
```

Or using Pandas:

``` python
df["order_count"].corr(df["price"])
```

## 📈 Insights

-   Products with higher prices may not always have higher order counts.
-   Seasonal or category-specific patterns influence sales.
-   Correlation values help identify **positive/negative relationships**
    between variables.

## 🚀 Future Work

-   Add predictive modeling (sales forecasting)
-   Build an interactive dashboard (Streamlit / Power BI)
-   Apply clustering for customer segmentation

## 👨‍💻 Author

Developed by **\[Pankaj Kumar Mantri\]**\
BSc IST, Ravenshaw University
