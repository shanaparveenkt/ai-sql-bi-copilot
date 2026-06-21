# AI SQL BI Copilot 🚀

An AI-powered Business Intelligence and Forecasting platform that enables users to query business data using natural language, generate SQL automatically, visualize analytics, extract AI-driven insights, receive strategic recommendations, and forecast future revenue trends.

This project simulates an enterprise-level AI BI Copilot for e-commerce analytics using the ShopSphere dataset.

---

# Project Overview

ShopSphere AI Copilot allows business users to ask questions in natural language such as:

- Show total revenue
- Show top 5 products by revenue
- Show average rating by city
- Show monthly revenue trend

The system automatically:
- Converts natural language into SQL queries
- Executes SQL on MySQL database
- Displays results
- Generates KPI dashboards
- Creates visual charts
- Produces AI-powered business insights
- Recommends business strategies
- Forecasts future revenue trends

---

# Features

## Query Agent
- Converts natural language questions into SQL queries using LLM
- Supports raw SQL queries for advanced users

Examples:
- Show total revenue
- Show revenue by city
- Show top products by sales

---

## Query Validator
- Prevents unsafe SQL execution
- Blocks dangerous operations such as:
  - DROP
  - DELETE
  - UPDATE
  - ALTER

Ensures safe database access.

---

## BI Agent
Generates:
- KPI cards
- Business dashboards
- Interactive visualizations

Supported charts:
- Bar charts
- Pie charts
- Line charts

---

## Analysis Agent
Uses AI to generate:
- Key insights
- Business trends
- Anomaly detection
- Root cause analysis

---

## Recommendation Agent
Provides strategic recommendations such as:
- Revenue optimization strategies
- Sales improvement suggestions
- Customer growth strategies

---

## Forecast Agent
Predicts future business performance using historical data.

Currently supports:
- Revenue forecasting

---

# System Architecture

```text
User Query
   ↓
Query Agent
   ↓
Query Validator
   ↓
MySQL Database
   ↓
BI Agent
   ↓
Analysis Agent
   ↓
Recommendation Agent
   ↓
Forecast Agent
```

---

# Tech Stack

## Programming Language
- Python

## Database
- MySQL

## Frontend
- Streamlit

## Visualization
- Plotly

## ORM / Database Connectivity
- SQLAlchemy
- PyMySQL

## AI / LLM
- Groq API
- LLaMA 3.1

## Data Processing
- Pandas
- NumPy

## Forecasting
- Scikit-learn / Time-series logic

---

# Project Structure

```text
AI_SQL_BI_ASSISTANT/
│
├── data/
│   ├── customers.csv
│   ├── products.csv
│   ├── sellers.csv
│   ├── orders.csv
│   ├── order_items.csv
│   ├── payments.csv
│   ├── reviews.csv
│   ├── delivery.csv
│   └── fact_sales.csv
│
├── sql_agent.py
├── query_validator.py
├── bi_agent.py
├── insight_generator.py
├── recommendation_agent.py
├── forecast_agent.py
├── database.py
├── load_data.py
├── streamlit_app.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

# Dataset

This project uses a custom e-commerce dataset named **ShopSphere**.

Main tables:
- Customers
- Products
- Sellers
- Orders
- Order Items
- Payments
- Reviews
- Delivery
- Fact Sales

The dataset simulates real-world e-commerce business operations.

---

# Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/AI-SQL-BI-Copilot.git
cd AI-SQL-BI-Copilot
```

---

## Create Virtual Environment

```bash
python -m venv venv
```

Activate environment:

### Windows
```bash
venv\Scripts\activate
```

### Mac/Linux
```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Database Setup

Create MySQL database:

```sql
CREATE DATABASE shopsphere;
```

Load dataset into MySQL.

---

# Environment Variables

Create a `.env` file.

```env
GROQ_API_KEY=your_api_key_here
```

---

# Run Application

```bash
streamlit run streamlit_app.py
```

---

# Sample Questions

Try these queries:

- Show total revenue
- Show total customers
- Show total orders
- Show total revenue by city
- Show average rating by city
- Show top 5 products by revenue
- Show monthly revenue trend

---

# Sample Workflow

Example query:

```text
Show top 5 products by revenue
```

System output:
- Generated SQL
- Query result table
- KPI dashboard
- Interactive chart
- AI business insights
- Strategic recommendations

---

# Example Outputs

## Generated SQL
```sql
SELECT product_name, SUM(sales_amount) AS revenue
FROM fact_sales
GROUP BY product_name
ORDER BY revenue DESC
LIMIT 5;
```

---

## KPI Dashboard
- Total Revenue
- Average Revenue
- Maximum Revenue

---

## AI Business Insights
- Revenue performance analysis
- Product trend analysis
- Key business insights

---

## Strategic Recommendations
- Pricing optimization
- Inventory planning
- Revenue growth strategies

---

# Key Learning Outcomes

This project demonstrates practical knowledge in:

- Python development
- SQL and database management
- Business Intelligence
- Data visualization
- LLM integration
- AI agents
- Forecasting systems

---

# Future Enhancements

Potential improvements:
- Multi-page dashboard
- Advanced forecasting models
- Role-based access control
- Real-time analytics
- Cloud deployment
- Voice-based query support

---

# Use Cases

This platform can be used in:
- E-commerce analytics
- Retail business intelligence
- Sales analytics
- Customer analytics
- Revenue forecasting

---

# Author

Shana Parveen KT


---

# License

This project is for educational and portfolio purposes.
