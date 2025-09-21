# 🛍️ Customer Segmentation using K-Means Clustering

This project performs customer segmentation on the "Mall Customers" dataset using the K-Means clustering algorithm. The goal is to identify distinct customer groups based on their annual income and spending habits, enabling targeted marketing strategies.

## 📋 Project Overview

The analysis involves several key steps:

1.  **Exploratory Data Analysis (EDA):** Understanding the dataset's structure, distributions, and relationships between features like age, gender, income, and spending score.
2.  **Data Preprocessing:** Selecting the most relevant features for clustering ('Annual Income' and 'Spending Score').
3.  **Finding Optimal Clusters:** Using the Silhouette Method to determine the ideal number of clusters (`k`) for the dataset.
4.  **K-Means Clustering:** Applying the K-Means algorithm with the optimal `k` to segment the customers.
5.  **Cluster Interpretation:** Analyzing the resulting cluster centroids to create descriptive, human-readable labels for each customer segment.
6.  **Visualization:** Plotting the final clusters to visually represent the distinct customer groups.

-----

## 📊 The Customer Segments

The analysis successfully identified **five distinct customer segments**:

1.  **Affluent, Luxury Shopper:** High income and high spending. These are the prime targets for premium products and loyalty programs.
2.  **Affluent, Low Spender:** High income but low spending. Potential for targeted promotions to increase their spending.
3.  **Low Income, Luxury Shopper:** Low income but high spending. This is an interesting group that might be young, impulsive buyers.
4.  **Low Income, Low Spender:** Low income and low spending. Cautious buyers, likely responsive to discounts and value-oriented marketing.
5.  **Moderate Income, Moderate Spender:** The average customer group. They form the bulk of the customer base.

-----

## Dataset

This project uses the **Mall Customers** dataset, which can be found on platforms like Kaggle. The dataset contains the following features:

  * `CustomerID`
  * `Gender`
  * `Age`
  * `Annual Income (k$)`
  * `Spending Score (1-100)`

-----

## 🛠️ Technology Stack

  * **Python**
  * **Pandas:** For data manipulation and analysis.
  * **NumPy:** For numerical operations.
  * **Scikit-learn:** For implementing the K-Means algorithm and calculating silhouette scores.
  * **Matplotlib & Seaborn:** For data visualization.
  * **Jupyter Notebook:** As the development environment.

-----

## 🚀 How to Run This Project

To run this notebook on your local machine, follow these steps:

### 1\. Prerequisites

  * Python 3.8 or higher
  * Jupyter Notebook or Jupyter Lab installed

### 2\. Installation & Setup

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/AniketAish/PRODIGY_ML_02.git
    cd PRODIGY_ML_02
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required packages:**
    Create a file named `requirements.txt` in the project directory and add the following lines to it:

    ```
    pandas
    numpy
    scikit-learn
    matplotlib
    seaborn
    jupyter
    ```

    Now, install the packages using pip:

    ```bash
    pip install -r requirements.txt
    ```

4.  **Download the dataset:**
    Make sure you have the `Mall_Customers.csv` file. You may need to update the file path in the notebook to where you've saved the CSV.

    ```python
    # In the notebook, check this line:
    df = pd.read_csv(r"path/to/your/Mall_Customers.csv")
    ```

5.  **Launch Jupyter Notebook:**

    ```bash
    jupyter notebook
    ```

    This will open a new tab in your browser. Navigate to the cloned directory and open the `.ipynb` file to run the cells.

-----

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
