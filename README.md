# 🥫 Nutritional Profiling and Clustering of Food Products Using OpenFoodFacts

This project analyzes **nutritional data of food products** using the public **[OpenFoodFacts](https://world.openfoodfacts.org/)** API.  
A **SQLite database** is built, products are explored and classified based on their nutritional profiles, and **clustering (DBSCAN)** is applied to discover natural groupings.

---

## **Key Features**
-  **Data extraction** from the OpenFoodFacts API (e.g., canned vegetables sold in the U.S.).  
-  **Structured SQLite database** with three tables:
  - `products`: basic product details (name, brand, category, countries).
  - `nutrients`: nutritional values per 100 g.
  - `nutrient_levels`: qualitative indicators and nutrition grades.  
-  **Data cleaning and normalization** of JSON into tidy Pandas DataFrames.  
-  **SQL queries** for insights:
  - Top foods by protein, calories, or sugar content.
  - Classify products as *Healthy*, *Neutral*, or *Unhealthy*.  
  - Identify products with sugar ≥50% above the average.  
  - Create views for high-fiber, high-protein products.  
-  **Unsupervised clustering**:
  - Feature scaling with `StandardScaler`.  
  - Grouping with `DBSCAN` to detect patterns without predefined labels.  

---

## 🛠 **Technologies Used**
- [Python 3](https://www.python.org/)  
- [Pandas](https://pandas.pydata.org/)  
- [SQLite3](https://www.sqlite.org/index.html)  
- [scikit-learn](https://scikit-learn.org/stable/)  
- [Requests](https://requests.readthedocs.io/)  

---
