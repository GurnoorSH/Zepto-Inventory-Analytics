# 🛒 Zepto Inventory Analytics: SQL Data Analysis Project

## 📊 Project Overview

This project presents a comprehensive SQL-based analysis of Zepto's inventory management system, demonstrating advanced data analysis techniques applied to real-world e-commerce data. Through systematic data exploration, cleaning, and strategic business intelligence queries, this analysis provides actionable insights for inventory optimization and revenue enhancement.

**Dataset Source**: [Zepto Inventory Dataset](https://www.kaggle.com/datasets/palvinder2006/zepto-inventory-dataset/data?select=zepto_v2.csv)

## 🎯 Business Context

Zepto, a leading quick-commerce platform, manages thousands of products across multiple categories with complex pricing structures, discount strategies, and inventory levels. This analysis addresses critical business questions around pricing optimization, inventory management, and category performance that directly impact profitability and customer satisfaction.

## 🔧 Technical Implementation

### Database Schema Design
```sql
CREATE TABLE zepto (
    sku_id SERIAL PRIMARY KEY,
    category VARCHAR(120),
    name VARCHAR(150) NOT NULL,
    mrp NUMERIC(8,2),
    discountPercent NUMERIC(5,2),
    availableQuantity INTEGER,
    discountedSellingPrice NUMERIC(8,2),
    weightInGms INTEGER,
    outOfStock BOOLEAN,
    quantity INTEGER
);
```

### Data Quality Assurance Process

The analysis begins with rigorous data validation and cleaning procedures:

**1. Completeness Assessment**
- Systematic null value detection across all critical fields
- Data integrity verification for business-critical columns

**2. Data Standardization**
- Currency conversion from paise to rupees for accurate financial calculations
- Removal of invalid records (products with zero pricing)

**3. Consistency Validation**
- Identification of duplicate product entries
- Stock status verification against availability metrics

## 📈 Key Business Intelligence Queries

### 1. **Strategic Discount Analysis**
Identifies the most attractive deals for customers, enabling marketing teams to promote high-value offerings and understand competitive positioning.

### 2. **Inventory Risk Assessment**
Highlights premium products that are out of stock, revealing potential revenue loss and helping prioritize restocking decisions for high-margin items.

### 3. **Revenue Optimization by Category**
Calculates potential revenue streams across product categories, providing insights for resource allocation and category management strategies.

### 4. **Premium Product Portfolio Analysis**
Examines high-value, low-discount products to understand luxury market positioning and identify opportunities for margin improvement.

### 5. **Category Performance Benchmarking**
Ranks categories by average discount percentage, revealing promotional strategies and helping identify categories that may need pricing adjustments.

### 6. **Value Engineering Analysis**
Calculates price-per-gram metrics for products, enabling cost-effectiveness comparisons and helping customers find the best value propositions.

### 7. **Product Segmentation Strategy**
Implements intelligent categorization based on product weight, facilitating targeted marketing campaigns and logistics optimization.

### 8. **Supply Chain Weight Analytics**
Analyzes total inventory weight by category, supporting warehouse planning and logistics cost management decisions.

## 💼 Business Impact & Insights

### Key Findings:
- **Pricing Strategy Optimization**: Identified products with suboptimal discount structures
- **Inventory Management**: Highlighted critical stock-outs in high-value segments
- **Category Performance**: Revealed top-performing categories by revenue potential
- **Value Proposition**: Established price-per-unit metrics for competitive analysis

### Strategic Recommendations:
- Implement dynamic pricing for high-discount products to maximize margins
- Prioritize restocking of premium out-of-stock items
- Develop category-specific promotional strategies based on discount patterns
- Optimize warehouse space allocation using weight-based analytics

## 🚀 Technical Skills Demonstrated

**Advanced SQL Techniques:**
- Complex aggregations with GROUP BY and HAVING clauses
- Conditional logic implementation using CASE statements
- Data transformation and cleaning procedures
- Statistical analysis with AVG, SUM, and ROUND functions
- Sorting and ranking with ORDER BY and LIMIT

**Data Analysis Methodology:**
- Systematic data exploration and profiling
- Data quality assessment and remediation
- Business-focused query design
- Performance-oriented SQL optimization

**Business Intelligence:**
- KPI development and measurement
- Category analysis and benchmarking
- Revenue forecasting and analysis
- Inventory optimization strategies

## 📋 Project Structure

```
zepto-inventory-analytics/
│
├── Zepto_SQL_data_analysis.sql    # Complete analysis script
├── README.md                      # Project documentation
└── data/                         # Dataset reference
    └── zepto_v2.csv              # Source data (Kaggle)
```

## 🔄 Reproducibility

To reproduce this analysis:

1. **Database Setup**: Execute the table creation script
2. **Data Import**: Load the Zepto dataset from Kaggle
3. **Analysis Execution**: Run the complete SQL script in sequence
4. **Results Validation**: Verify outputs against business logic

## 🎯 Future Enhancements

- **Predictive Analytics**: Implement demand forecasting models
- **Customer Segmentation**: Analyze purchasing patterns by customer demographics
- **Seasonal Analysis**: Examine inventory trends across different time periods
- **Competitive Benchmarking**: Compare pricing strategies with market competitors

## 🛠️ Technologies Used

- **Database**: PostgreSQL
- **Language**: SQL
- **Data Source**: Kaggle Datasets
- **Analysis Type**: Descriptive and Diagnostic Analytics

## 📞 Connect With Me

This project showcases my ability to transform raw e-commerce data into actionable business insights using advanced SQL techniques. I'm passionate about leveraging data analytics to drive strategic decision-making in retail and technology environments.

---

*This project demonstrates practical application of SQL skills in real-world business scenarios, emphasizing both technical proficiency and business acumen essential for data analyst and business intelligence roles.*