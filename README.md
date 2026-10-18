# E-Commerce Sales & Operations Analytics

An end-to-end Business Intelligence project built using PostgreSQL, SQL, and Power BI to analyze the Brazilian Olist e-commerce dataset.

The project transforms raw transactional data into an analytics-ready data model and provides interactive dashboards for analyzing sales, customers, products, logistics, reviews, payments, and seller performance.

---

## Project Overview

E-commerce businesses generate large volumes of data across orders, customers, products, sellers, payments, deliveries, and customer reviews.

This project integrates these datasets into PostgreSQL, creates SQL-based BI views, and connects the transformed data to Power BI for business analysis and reporting.

### Objectives

- Analyze revenue and order trends over time
- Identify high-performing product categories
- Analyze customer and geographic sales patterns
- Measure delivery and logistics performance
- Analyze customer reviews and satisfaction
- Understand payment methods and installment behavior
- Evaluate seller performance
- Build an executive-level business intelligence dashboard

---

## Tech Stack

- PostgreSQL
- SQL
- Power BI
- DAX
- Data Modeling
- Business Intelligence
- Data Analytics

---

## Dataset

The project uses the Brazilian Olist E-commerce dataset.

The raw dataset contains the following tables:

| Dataset | Description |
|---|---|
| Customers | Customer information and location |
| Orders | Order status and order lifecycle dates |
| Order Items | Products purchased within each order |
| Products | Product details and dimensions |
| Sellers | Seller information and location |
| Payments | Payment methods, values, and installments |
| Reviews | Customer ratings and review information |
| Geolocation | ZIP code, latitude, longitude, city, and state |
| Category Translation | Portuguese-to-English product category mapping |

The dataset contains approximately 100K orders and multiple related transactional tables.

---

## Data Architecture

```text
Olist CSV Dataset
        |
        v
PostgreSQL Raw Tables
        |
        v
SQL Transformation Layer
        |
        +-------------------+
        |                   |
        v                   v
BI Fact Views          BI Dimension Views
        |                   |
        +---------+---------+
                  |
                  v
             Power BI
                  |
                  v
          DAX Measures
                  |
                  v
        Interactive Dashboard
