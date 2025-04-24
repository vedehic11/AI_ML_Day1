# Titanic Dataset Analysis

This project demonstrates data preprocessing, cleaning, and exploratory data analysis (EDA) on the Titanic dataset using Python. The notebook includes steps for handling missing data, scaling numerical features, detecting and removing outliers, and encoding categorical features.

## Project Structure

- **`Day1.ipynb`**

## Steps in the Notebook

1. **Import Libraries**:
   - Libraries such as `pandas`, `seaborn`, and `matplotlib` are used for data manipulation and visualization.

2. **Load Dataset**:
   - The Titanic dataset is loaded using `seaborn`'s `load_dataset` function.

3. **Data Cleaning**:
   - Dropped unnecessary columns like `alive`, `who`, `adult_male`, `alone`, and `deck`. ( these were causing me error , due to my previous attempt)
     
   - Filled missing values in columns like `age`, `embarked`, and `embark_town` using median or mode.

4. **Scaling and Standardization**:
   - Used `StandardScaler` from `sklearn` to scale numerical columns (`age`, `fare`, `parch`, `sibsp`).

5. **Outlier Detection and Removal**:
   - Detected outliers using the Interquartile Range (IQR) method.
   - Removed rows containing outliers.

6. **Encoding Categorical Features**:
   - Encoded the `sex` column using `LabelEncoder`.
   - Applied one-hot encoding to the `embarked` column and dropped the original column.

7. **Correlation Heatmap**:
   - Visualized the correlation between numerical features using a heatmap.

## Prerequisites

- Python 3.7 or higher
- Libraries:
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `scikit-learn`



1. Clone the repository or download the notebook file.
2. Install the required libraries:
   ```bash
   pip install pandas seaborn matplotlib scikit-learn
