##  Job Market Analysis & Forecasting with Prophet

This project explores job listings data to uncover hiring patterns, top job roles, skills demand, and hiring activity over time. It also uses time series forecasting to predict the volume of job postings for the coming weeks using Facebook's Prophet model.

---

## Objectives

- Perform **exploratory data analysis (EDA)** on job listings
- Identify **most in-demand roles, companies, cities, and skills**
- Visualize **hiring trends over time**
- Build a **forecasting model** to predict future job postings
- Share insights in a clear, visual, and impactful way

---

##  Dataset Overview

- The dataset contains job listings scraped from online platforms.
- Key features include:
  - `job_title`: Name of the advertised position
  - `location`: City where the job is based
  - `company`: Hiring organization
  - `skills`: Key skills required for the job
  - `posted_date`: Date the job was posted

---

## Exploratory Data Analysis (EDA)

### 1.Most Common Job Titles

We identified the top 10 job titles, such as:
- **Data Analyst**
- **Software Engineer**
- **Business Analyst**

> **Insight**: These roles indicate high demand in the tech and data-driven fields.

---

### 2.  Most Active Hiring Cities

The top locations included:
- **Nairobi**
- **Mombasa**
- **Kisumu**

> Insight: Major urban centers show the highest job activity, consistent with economic hubs in Kenya.

---

### 3.  Top Hiring Companies

Some of the top companies (simulated in the dataset) included:
- Safaricom
- Andela
- IBM
- Google

> Insight: Larger tech and multinational companies drive a significant portion of the hiring.

---

### 4. Most Requested Skills

We tokenized the `skills` column to reveal the most in-demand skills:
- **Python**
- **SQL**
- **Excel**
- **Power BI**
- **Machine Learning**

> Insight: Core data analytics and visualization tools dominate the market demand.

---

### 5.  Job Posting Trends Over Time

By aggregating job postings weekly, we visualized hiring trends over time. The data showed:
- Periodic spikes and dips in hiring
- Some seasonality or fluctuations over months

> Insight: These trends are valuable for planning job applications or understanding market slowdowns.

---

## Forecasting Job Postings with Prophet

We used **Facebook Prophet**, a time series model designed for business data.

### Steps:
- Grouped job listings by week (`W` frequency)
- Renamed columns to fit Prophet's format: `ds` for dates, `y` for values
- Trained the model on historical weekly posting data
- Forecasted job postings for the **next 12 weeks**

### Forecast Results

The Prophet model output revealed:
- An **upward trend**, suggesting that job postings may increase
- A **weekly seasonality pattern**, with regular dips and spikes
- The forecast curve was smooth and realistic

 **Interpretation**: Assuming historical patterns continue, job listings will grow moderately in the near future — helpful insight for job seekers and hiring teams.

---

## project structure
job-market-analysis/
│
├── job_listings.csv # Dataset used for the analysis
├── job_analysis.ipynb # Jupyter Notebook with full code
├── README.md # Project documentation (this file)

---

## Tools & Technologies

- **Python 3.10+**
- **Pandas** – data manipulation
- **Matplotlib & Seaborn** – data visualization
- **Prophet** – time series modeling
- **Jupyter Notebook / Google Colab** – development environment

---

## ✍️ Author

**Valentine Njeri**  
Aspiring Data Analyst | Passionate about solving real-world problems through data insights

---

## Future Work

- Add job description text mining using NLP
- Analyze salary ranges if data is available
- Deploy visualizations in a dashboard (e.g., Streamlit or Power BI)
- Compare forecasts using other models like LSTM or ARIMA

---

## Final Note

This project demonstrates the full cycle of a data analytics workflow — from cleaning and visualizing raw data to forecasting future patterns. It showcases essential skills for entry-level data roles including:

- EDA
- Data wrangling
- Visualization
- Forecasting
- Reporting




