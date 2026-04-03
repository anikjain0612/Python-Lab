# Experiment 12: Data Wrangling Using Python

## Aim

To carry out data wrangling using Python and the Pandas library by cleaning, transforming, and restructuring raw data into a well-organized format that is suitable for reliable analysis and informed decision-making.

---

## Tools Used

- Jupyter Notebook / Google Colab
- Python (Pandas library)

---

## Theory

### 1. Data Wrangling

Data wrangling is the practice of taking raw, unstructured, or inconsistent data and converting it into a clean and analysis-ready format. It encompasses a series of steps aimed at improving the overall quality and usability of a dataset.

This process is often the most time-intensive phase in any data pipeline, but it is also among the most critical. Core tasks include addressing missing values, correcting data types, eliminating duplicate records, and consolidating data from multiple sources into a single coherent structure.

---

### 2. Handling Missing Values

Missing data is a common challenge in real-world datasets and can arise from causes such as manual entry errors, system interruptions, or incomplete data collection processes. If left unaddressed, these gaps can skew analytical outcomes.

Pandas offers several utilities to manage missing values effectively:

- `isnull()` — detects missing entries in the dataset
- `dropna()` — removes rows or columns that contain missing values
- `fillna()` — substitutes missing values with a defined replacement such as 0, mean, or median

Properly handling missing data helps preserve the integrity of the dataset and minimizes the risk of introducing bias into the analysis.

---

### 3. Removing Duplicates

Duplicate entries can lead to misleading conclusions and inflated counts during analysis. They typically arise from repeated data entry or improperly managed dataset merges.

Pandas provides two key functions for this:

- `duplicated()` — flags rows that are repeated
- `drop_duplicates()` — eliminates those repeated rows

Removing duplicates guarantees that every record in the dataset is unique and contributes meaningfully to the results.

---

### 4. Data Transformation

Transformation involves reshaping or converting data into a format better suited for analysis. This can include changing column data types, deriving new columns from existing ones, or applying mathematical operations across the dataset.

For instance, converting a column from string to integer format, or computing a new `Total Cost` column from `Quantity` and `Price`, are typical transformation steps. Such operations enhance the analytical depth and usability of the dataset.

---

### 5. Renaming Columns

Column names in raw datasets are often cryptic, abbreviated, or inconsistent. Renaming them to more descriptive labels improves both readability and ease of use during analysis.

Pandas supports this through the `rename()` function, which allows selective or bulk renaming of columns — especially useful when working with large or merged datasets.

---

### 6. Filtering Data

Filtering allows analysts to isolate specific subsets of data that satisfy a given condition, enabling more focused and relevant analysis.

For example, extracting only the rows where a product category equals `'Electronics'` allows targeted insights without being distracted by unrelated records. This makes the analytical process more efficient and precise.

---

### 7. Sorting Data

Sorting arranges the dataset in a logical order — ascending or descending — based on one or more columns. It aids in spotting trends, identifying outliers, and improving overall data readability.

**Pandas method:**
```python
df.sort_values(by='Price')
```

---

### 8. Merging and Joining Data

Real-world data is often distributed across multiple tables or files. Merging and joining operations bring these separate datasets together into a unified structure for more comprehensive analysis.

**Pandas method:**
```python
df3 = pd.merge(df1, df2, on='ID')
```

This combines two DataFrames based on a shared column, enabling richer cross-dataset analysis.

---

## Code Snippets

```python
# Remove duplicate rows
df = df.drop_duplicates()

# Sort by a specific column
df = df.sort_values(by='Price')

# Merge two DataFrames on a common column
df3 = pd.merge(df1, df2, on='ID')
```

---

## Applications

- **Machine Learning** — Preprocessing raw data to improve model performance and accuracy
- **Business Intelligence** — Cleaning and structuring customer data for better segmentation
- **Finance** — Ensuring accurate data for reporting and forecasting purposes
- **Research** — Preparing survey or experimental data for statistical analysis

---

## Advantages

- Significantly improves data quality and reliability
- Reduces the likelihood of errors and inconsistencies in analysis
- Streamlines the overall data analysis workflow
- Enables seamless integration with advanced AI and ML pipelines

---

## Result

Data wrangling was successfully carried out using Python and the Pandas library. Operations including missing value treatment, duplicate removal, data type transformation, filtering, sorting, and dataset merging were all performed effectively. The resulting dataset was clean, well-structured, and ready for accurate downstream analysis and processing.
