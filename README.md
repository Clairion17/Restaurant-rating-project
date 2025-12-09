# Restaurant-rating-project
✅ FINAL GITHUB README (Markdown Code — ready to paste)
# 🍽️ Restaurant Rating Analysis (Mexico 2012)

This project analyzes the **Restaurant Rating Dataset** collected from customer surveys across Mexico in 2012.  
The goal is to uncover insights that help **business owners and investors** make informed decisions about the food service market—covering cuisines, customer preferences, spending behaviour, satisfaction drivers, and location performance.

---

## 📊 Project Objectives

- Explore restaurant performance across Mexico  
- Identify top-rated cuisines and poorly performing ones  
- Understand customer demographics and preferences  
- Discover factors driving customer satisfaction  
- Segment customers into meaningful groups  
- Provide data-driven recommendations for entrepreneurs and investors  

---

## 📁 Dataset Description

The dataset includes:

- Restaurant details (name, location, type, cuisine, price range, etc.)  
- Customer demographic info (age, gender, frequency of visits)  
- Satisfaction ratings  
- Preferences and consumption patterns  
- Additional metadata collected during the 2012 Mexico restaurant survey  

---

## 🧹 Data Cleaning Steps

- Standardized cuisine and text fields  
- Handled missing values  
- Created derived variables (age groups, rating categories, price bins)  
- Converted appropriate columns to numeric or categorical  
- Removed duplicates and inconsistencies  

---

## 🔍 Exploratory Data Analysis (EDA)

The notebook includes:

- Rating distribution  
- Ratings by cuisine and price range  
- Ratings by location  
- Customer demographics distribution  
- Correlation analysis  
- Top factors influencing ratings  

Example plot:  

```python
import matplotlib.pyplot as plt

plt.hist(df['rating'])
plt.xlabel("Rating")
plt.ylabel("Frequency")
plt.title("Distribution of Restaurant Ratings")
plt.show()

🤖 Rating Prediction Model

A Random Forest model was built to identify key drivers of restaurant ratings.

from sklearn.ensemble import RandomForestRegressor

model = RandomForestRegressor(n_estimators=200, random_state=42)
model.fit(X_train, y_train)
importances = model.feature_importances_


Key insights from the model (example):

Food quality

Service speed

Price–value perception

Customer visit frequency

👥 Customer Segmentation

KMeans clustering was used to group customers based on behaviour and demographics.

from sklearn.cluster import KMeans

kmeans = KMeans(n_clusters=4, random_state=42)
df['segment'] = kmeans.fit_predict(X_scaled)


Result:

Budget diners

Premium customers

Frequent visitors

Young fast-casual lovers

🗺️ Geographic Insights

Maps show:

High-demand neighborhoods

Underserved areas

Clustering of high-rated restaurants

💡 Business Recommendations

Expand into underserved neighborhoods with high demand

Improve service speed and food quality

Align cuisine offerings with high-rating categories

Tailor pricing strategies to local demographics

Leverage data-backed customer personas

📝 Project Structure
project-folder/
│── data/
│── notebooks/
│   └── restaurant_rating_analysis.ipynb
│── src/
│── README.md
│── requirements.txt

▶️ How to Run the Project

Install dependencies:

pip install -r requirements.txt

📬 Contact

For questions or collaboration opportunities, feel free to reach out.
Amara Anagbor
Data Analyst
claribelonwu11@gmail.com

Run the Jupyter notebook:

jupyter notebook notebooks/restaurant_rating_analysis.ipynb
