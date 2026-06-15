# ✈️ Flight Booking Data Analysis Project

## 📖 About the Project

Have you ever wondered why flight ticket prices change so frequently? Why does the same route cost different amounts on different days or airlines?

This project explores these questions through a complete Exploratory Data Analysis (EDA) workflow on real flight booking data. Using Python and popular data analysis libraries, we uncover hidden patterns in airline pricing, travel routes, departure schedules, flight duration, and booking behavior.

The goal is to transform raw flight booking data into meaningful business insights that can help airlines optimize pricing strategies, improve customer experience, and understand travel demand trends.

---

## 🎯 Project Objectives

* Analyze airline ticket pricing patterns.
* Compare fare structures across airlines.
* Understand how flight duration affects ticket prices.
* Identify the impact of departure and arrival timings.
* Explore route popularity and pricing trends.
* Study the influence of cabin class and number of stops.
* Generate actionable business insights through visualization.

---

## 📂 Project Structure

```text
Flight_Booking_Project/
├── README.md                      # Project Documentation
├── Flight_Booking_Project.ipynb   # Jupyter Notebook containing analysis
└── Flight_Booking.csv             # Dataset
```

---

## 📊 Dataset Information

The dataset contains **10,683 flight booking records** with information such as:

| Feature          | Description                     |
| ---------------- | ------------------------------- |
| airline          | Airline name                    |
| flight           | Flight code                     |
| source_city      | Departure city                  |
| departure_time   | Flight departure slot           |
| stops            | Number of stops                 |
| arrival_time     | Arrival slot                    |
| destination_city | Destination city                |
| class            | Economy or Business             |
| duration         | Flight duration (hours)         |
| days_left        | Days remaining before departure |
| price            | Ticket price                    |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🔄 Project Workflow

### 1️⃣ Data Collection

* Import dataset
* Load CSV file into Pandas DataFrame

### 2️⃣ Data Cleaning

* Remove duplicates
* Handle missing values
* Verify data types
* Eliminate unnecessary columns

### 3️⃣ Exploratory Data Analysis (EDA)

* Dataset overview
* Statistical summaries
* Feature analysis
* Price trend analysis

### 4️⃣ Data Visualization

* Histograms
* Count plots
* Box plots
* Heatmaps
* Correlation analysis
* Comparative airline charts

### 5️⃣ Business Insights

* Airline pricing behavior
* Route performance analysis
* Impact of booking time on ticket prices
* Duration vs Price relationship

---

## 📈 Key Visualizations

The notebook includes:

### Airline-wise Price Comparison

Understand which airlines offer premium or budget pricing.

### Cabin Class Analysis

Compare Economy and Business class fares.

### Route Analysis

Identify expensive and affordable travel routes.

### Departure Time Trends

Analyze how departure schedules affect pricing.

### Correlation Heatmap

Visualize relationships between numerical features.

### Flight Duration vs Ticket Price

Study whether longer flights cost significantly more.

---

## 🔍 Major Insights

✔️ Business-class tickets are significantly more expensive than Economy tickets.

✔️ Flights booked closer to departure dates generally have higher prices.

✔️ Certain airlines consistently maintain premium pricing strategies.

✔️ Flight duration has a positive correlation with ticket price.

✔️ Routes connecting major metropolitan cities tend to exhibit higher fare fluctuations.

---

## 💡 Tips & Tricks for Better Analysis

### 1. Always Clean Data First

Even the best machine learning models fail when data quality is poor.

```python
df.drop_duplicates(inplace=True)
df.isnull().sum()
```

---

### 2. Understand the Distribution Before Modeling

Use histograms and boxplots to detect:

* Outliers
* Skewness
* Abnormal values

```python
sns.histplot(df['price'])
```

---

### 3. Correlation Does Not Mean Causation

A strong correlation between duration and price doesn't necessarily mean duration alone determines cost.

Always validate findings using domain knowledge.

---

### 4. Look Beyond Averages

Instead of only checking mean prices:

```python
df.groupby('airline')['price'].describe()
```

This reveals variability, quartiles, and outliers.

---

### 5. Use Visualizations to Tell a Story

Good data analysis is not about creating charts.

It is about answering questions such as:

* Why are some airlines more expensive?
* Which routes generate higher revenue?
* When should customers book tickets?

---

### 6. Think Like a Business Analyst

Ask:

* Which airline earns the highest revenue?
* Which route should be promoted?
* How can ticket pricing be optimized?

These questions convert data analysis into business value.

---

## 🚀 Future Enhancements

* Flight Price Prediction using Machine Learning
* Customer Segmentation
* Interactive Dashboard using Streamlit
* Real-Time Flight Data Integration
* Demand Forecasting Models
* Revenue Optimization Analysis

---

## ▶️ How to Run

### Clone Repository

```bash
git clone <repository-url>
```

### Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn
```

### Launch Jupyter Notebook

```bash
jupyter notebook Flight_Booking_Project.ipynb
```

Make sure `Flight_Booking.csv` is present in the same directory as the notebook.

---

## 🎓 Learning Outcomes

By completing this project, you will gain practical experience in:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Data Visualization
* Statistical Interpretation
* Business Analytics
* Insight Generation
* Python for Data Science

---

## 👩‍💻 Author

**Prathibha D**

B.E. Computer Science & Engineering
Aspiring AI/ML Engineer | Data Science Enthusiast

---

## 📜 License

This project is open-source and intended for educational, research, and learning purposes.

⭐ If you found this project useful, consider giving the repository a star!

