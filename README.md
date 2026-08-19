# 📊 Smart City Traffic & Retail Analytics
 
<p align="center">

<img src="https://img.shields.io/badge/Python-NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>

<img src="https://img.shields.io/badge/Project-Data%20Analytics-4CAF50?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Case%20Study-Smart%20City-blue?style=for-the-badge"/>

</p>

<p align="center">
  <b>A NumPy-based data analytics case study exploring traffic, retail sales, and weather data.</b>
</p>

---

## 📌 About the Project

This project is a **Smart City Traffic & Retail Analytics** case study developed using **Python and NumPy**.

The scenario represents a Smart City Analytics Project where different types of data are collected and analyzed:

* 🚦 Traffic data
* 🛍️ Retail sales data
* 🌦️ Weather data

The objective of this case study is to analyze these datasets using **NumPy only** and practice important array manipulation, slicing, aggregation, statistical analysis, masking, broadcasting, sorting, and trend-analysis techniques.

---

## 🎯 Objectives

The case study focuses on:

* Understanding NumPy arrays and their properties
* Working with 1D, 2D and 3D arrays
* Reshaping and flattening arrays
* Performing advanced indexing and slicing
* Calculating aggregations and statistics
* Applying Boolean masking
* Using conditional operations
* Understanding NumPy broadcasting
* Performing sorting and ranking
* Working with random sampling
* Performing sales and traffic trend analysis
* Calculating month-to-month growth rates

---

# 📂 Datasets

## 🚦 Traffic Dataset

The traffic dataset represents vehicle counts across:

* **4 regions**
* **7 days**
* **24 hours**

### Shape

```text
(4, 7, 24)
```

Each value represents the **number of vehicles per hour**.

The dataset is generated using NumPy random integers.

---

## 🛍️ Sales Dataset

The retail sales dataset represents:

* **12 months**
* **5 stores**
* **8 products**

### Shape

```text
(12, 5, 8)
```

The sales values are generated using NumPy random integers.

---

## 🌦️ Weather Dataset

The weather dataset contains temperature information for:

* **365 days**

### Shape

```text
(365,)
```

Temperature values are generated using a normal distribution with NumPy.

---

# 🧠 NumPy Concepts Covered

This case study provides practical experience with the following NumPy concepts.

## 📦 1. Array Properties

Explored:

```python
ndim
shape
size
dtype
```

Used to understand the structure and properties of the traffic and sales datasets.

---

## 🔄 2. Reshaping

Practiced reshaping datasets without changing their underlying data.

Examples:

```python
traffic.reshape(28, 24)

sales.reshape(60, 8)
```

---

## 📐 3. Flattening

Compared:

```python
flatten()
```

and

```python
ravel()
```

The notebook also includes explanations of the difference between returning a copy and a view.

---

## ✂️ 4. Array Slicing

Performed slicing operations on sales and traffic data.

Examples include:

* Store-specific data
* Product-specific data
* Selected months
* Selected products
* Selected regions
* Selected days
* Selected hours
* Last months
* Reverse-order data

---

## 🔁 5. Reverse Slicing

Practiced reversing:

* Sales months
* Traffic hours

Using NumPy slicing techniques.

---

# 📊 6. Aggregation

Performed aggregation operations on traffic and sales datasets.

### Traffic Analysis

Calculated:

* Total traffic per region
* Total traffic per day
* Total traffic per hour

### Sales Analysis

Calculated:

* Total yearly sales
* Sales per month
* Sales per store
* Sales per product

---

# 📈 7. Average Calculations

Calculated:

* Average hourly traffic
* Average monthly sales
* Average sales per product

using NumPy aggregation functions.

---

# 📉 8. Statistical Analysis

Calculated statistical measures for the datasets.

### Measures included:

```python
mean
median
standard deviation
variance
minimum
maximum
```

---

# 🎯 9. Conditional Operations

Practiced modifying data based on conditions.

Examples include:

* Increasing sales values by 15%
* Converting traffic values into thousands of vehicles
* Replacing traffic values below a threshold
* Capping sales values above a specified value

---

# 🔎 10. Boolean Masking

Used Boolean indexing to extract values based on conditions.

Examples:

```python
sales[sales > 800]
```

```python
traffic[traffic > 450]
```

```python
temperature[temperature < 25]
```

---

# 📡 11. Broadcasting

Practiced NumPy broadcasting using a product discount array.

Example:

```python
discount = np.array([10,20,30,40,50,60,70,80])

sales - discount
```

Also applied a 5% tax to sales values.

---

# 🤖 12. Masking with Conditional Operations

Worked with conditions involving:

* Temperature
* Sales
* Traffic

and practiced combining masking with NumPy operations.

---

# 🏆 13. Important Values

Extracted values based on conditions such as:

* Sales greater than 800
* Traffic greater than 450
* Temperatures below 25

---

# 🔢 14. Sorting & Ranking

Practiced:

```python
np.sort()
np.argmax()
np.argmin()
```

The case study includes analysis related to:

* Monthly sales ranking
* Top-performing months
* Busiest region
* Least busy hour

---

# 🎲 15. Random Sampling

Used NumPy random functions to generate a random sample of sales values.

Example:

```python
np.random.choice()
```

---

# 📈 16. Trend Analysis

Compared:

* First 6 months of sales
* Last 6 months of sales

The notebook explores which half of the year performed better.

---

# 📊 17. Growth Rate Analysis

Calculated month-to-month sales growth using:

```python
monthly_sales = sales.sum(axis=(1,2))

growth_rate = (
    (monthly_sales[1:] - monthly_sales[:-1])
    / monthly_sales[:-1]
) * 100
```

This helps identify changes in monthly sales performance.

---

# 📝 Case Study Tasks

The notebook contains **25 NumPy-based tasks** covering:

| Task | Topic                                  |
| ---- | -------------------------------------- |
| 01   | Explore array properties               |
| 02   | Reshaping                              |
| 03   | Flattening & ravel                     |
| 04   | Sales slicing                          |
| 05   | Traffic slicing                        |
| 06   | Reverse slicing                        |
| 07   | Traffic aggregations                   |
| 08   | Sales aggregations                     |
| 09   | Average calculations                   |
| 10   | Statistical measures                   |
| 11   | Sales/traffic/temperature operations   |
| 12   | Masking operations                     |
| 13   | Product discount                       |
| 14   | City tax                               |
| 15   | Temperature effect                     |
| 16   | Important values                       |
| 17   | Traffic classification                 |
| 18   | High-sale transactions                 |
| 19   | Sales sorting & ranking                |
| 20   | `argmax()` / `argmin()`                |
| 21   | Random sampling                        |
| 22   | Temperature & sales relationship       |
| 23   | First-half vs second-half sales        |
| 24   | Sales growth rate                      |
| 25   | Highest average traffic hour by region |

---

# 📓 Jupyter Notebook

The complete case study is available here:

👉 **[Open the NumPy Case Study](./numpy_case_study.ipynb)**

The notebook contains the questions, NumPy code, outputs, and analysis performed for the case study.

---

# 📁 Project Structure

```text
numpy-smart-city-analytics/
│
├── numpy_case_study.ipynb
│
└── README.md
```

---

# 💡 Key Learning Outcomes

Through this case study, I practiced:

* NumPy array creation
* Multidimensional arrays
* Array properties
* Reshaping
* Flattening
* Ravel
* Indexing
* Slicing
* Reverse slicing
* Aggregation
* Statistical analysis
* Boolean masking
* Conditional operations
* Broadcasting
* Sorting
* Ranking
* Random sampling
* Trend analysis
* Growth-rate calculations

---

# 🚀 Future Improvements

The case study can be further improved by:

* Completing the remaining pending analysis tasks
* Adding deeper relationship analysis between datasets
* Using **Pandas** for more advanced data manipulation
* Using **Matplotlib** and **Seaborn** for visualization
* Performing more detailed Exploratory Data Analysis
* Creating a **Power BI dashboard**
* Combining traffic, sales and weather data for deeper business insights

---

# ⚠️ Project Status

This is a **learning and practice case study** created to strengthen practical NumPy and Data Analytics skills.

Some advanced tasks in the notebook are still being developed and can be improved in future versions.

---

# 🛠️ Technologies Used

| Technology          | Purpose                                  |
| ------------------- | ---------------------------------------- |
| 🐍 Python           | Programming                              |
| 🔢 NumPy            | Data generation, manipulation & analysis |
| 📓 Jupyter Notebook | Development & documentation              |

---

# 👨‍💻 Author

## Dharmana Lokesh

📊 **Aspiring Data Analyst**

🐍 Python • SQL • Power BI • Excel • Pandas • NumPy

🔗 **GitHub:** [DharmanaLokesh](https://github.com/DharmanaLokesh)

🔗 **LinkedIn:** [Dharmana Lokesh](https://www.linkedin.com/in/dharmana-lokesh-290396268)

📧 **Email:** [lokeshdarmana@gmail.com](mailto:lokeshdarmana@gmail.com)

---

<p align="center">

⭐ If you find this project useful, consider giving it a star!

</p>

<p align="center">

<b>Data → Analysis → Insights 📊</b>

</p>
