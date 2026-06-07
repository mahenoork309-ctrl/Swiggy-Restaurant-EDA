# Swiggy Restaurant Data — Exploratory Data Analysis (EDA)

An end-to-end EDA project on Swiggy's restaurant dataset to uncover insights about ratings, delivery performance, offers, and customer satisfaction.

---

## Objective

The goal of this project is to analyze Swiggy restaurant data and answer key business questions:

1. How are restaurant ratings distributed on the platform?
2. What is the typical delivery time range?
3. Does delivery time affect customer ratings?
4. Do higher discounts lead to better ratings?
5. Which restaurants are the fastest in delivery?

---

## Dataset

**File:** `swiggy_cleaned.csv`

**Key Columns:**

| Column | Description |
|---|---|
| `hotel_name` | Restaurant name |
| `rating` | Customer rating (1.0 – 5.0) |
| `time_minutes` | Delivery time in minutes |
| `offer_percentage` | Discount offered (%) |
| `location` | Restaurant location |
| `food_type` | Type of cuisine |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly
- **Environment:** Jupyter Notebook

---

## Analysis Performed

### 1. Data Cleaning
- Handled missing values
- Removed duplicate records
- Type-casted columns to numeric where required

### 2. Univariate Analysis
- **Rating Distribution** — Most restaurants rated between 4.0–4.5; left-skewed distribution
- **Delivery Time Distribution** — Majority of deliveries complete in 20–50 minutes

### 3. Bivariate Analysis
- **Delivery Time vs Rating** — No clear correlation; customers rate based on food quality, not speed
- **Offer % vs Rating** — Higher discounts do not guarantee better ratings
- **Average Offer by Rating Group** — Lower-rated restaurants offer higher discounts to compensate

### 4. Other Insights
- **Top 10 Fastest Delivery Restaurants** — All deliver within ~12 minutes
- **Delivery Time Boxplot** — Median around 35–45 mins; outliers above 60–70 mins indicate peak-hour delays
- **Correlation Heatmap** — All numeric variables are weakly correlated with each other

---

## Key Findings

- ✅ Swiggy's delivery is **consistent** — most orders arrive in 20–50 minutes
- ✅ Customer ratings are generally **high across the platform** (4.0–4.5 range)
- ✅ **Delivery time does not significantly impact ratings** — food quality matters more
- ✅ **Discounts don't drive ratings** — highly rated restaurants maintain only moderate offers
- ✅ Lower-rated restaurants offer higher discounts but fail to improve their scores

---

## Project Structure

```
swiggy-eda/
│
├── EDA_Project_swiggy_dataset.ipynb   # Main analysis notebook
├── swiggy_cleaned.csv                 # Dataset
└── README.md
```

---

## How to Run

```bash
git clone https://github.com/your-username/swiggy-eda.git
cd swiggy-eda
pip install pandas numpy matplotlib seaborn plotly
jupyter notebook EDA_Project_swiggy_dataset.ipynb
```
