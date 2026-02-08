<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Retail Sales Performance Analysis</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f5f5f5;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            font-size: 2.5em;
            color: #2c3e50;
            margin-bottom: 30px;
            border-bottom: 4px solid #3498db;
            padding-bottom: 15px;
            text-align: center;
        }
        
        h2 {
            font-size: 1.8em;
            color: #34495e;
            margin-top: 30px;
            margin-bottom: 15px;
            border-left: 5px solid #3498db;
            padding-left: 15px;
        }
        
        h3 {
            font-size: 1.3em;
            color: #5d6d7b;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        
        p {
            font-size: 1em;
            margin-bottom: 15px;
            text-align: justify;
        }
        
        ul {
            margin-left: 30px;
            margin-bottom: 15px;
        }
        
        li {
            margin-bottom: 8px;
            font-size: 0.95em;
        }
        
        a {
            color: #3498db;
            text-decoration: none;
        }
        
        a:hover {
            text-decoration: underline;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            font-size: 0.95em;
        }
        
        th {
            background-color: #3498db;
            color: white;
            padding: 12px;
            text-align: left;
            font-weight: 600;
        }
        
        td {
            padding: 10px 12px;
            border-bottom: 1px solid #ddd;
        }
        
        tr:hover {
            background-color: #f8f9fa;
        }
        
        .tech-stack {
            background-color: #ecf0f1;
            padding: 20px;
            border-radius: 5px;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Retail Sales Performance Analysis</h1>
        
        <h2>Overview</h2>
        <p>This project analyses a Retail Sales dataset sourced from Kaggle to evaluate business performance across revenue trends, product performance, customer behaviour, and profitability.</p>
        <p>The objective is to simulate a real-world retail analytics workflow using Python, SQL, and Power BI to generate actionable business insights.</p>
        
        <div class="tech-stack">
            <h2>Tech Stack</h2>
            <ul>
                <li><strong>Python (Pandas)</strong> – Data cleaning & feature engineering</li>
                <li><strong>SQL (MySQL / BigQuery syntax)</strong> – Business-driven data analysis</li>
                <li><strong>Power BI</strong> – Interactive dashboard development</li>
            </ul>
        </div>
        
        <h2>Dataset Source</h2>
        <h3>Retail Sales Dataset (Kaggle)</h3>
        <p><a href="https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset" target="_blank">https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset</a></p>
        
        <h2>Repository Structure</h2>
        
        <h3>Dashboard</h3>
        <p>Contains Power BI dashboard screenshots highlighting revenue, customer, and profitability insights.</p>
        
        <h3>Dataset</h3>
        <p>Includes:</p>
        <ul>
            <li>Raw dataset</li>
            <li>Cleaned dataset used for SQL and visualization</li>
        </ul>
        
        <h3>Python</h3>
        <p>Contains the data cleaning and preprocessing script used to:</p>
        <ul>
            <li>Create derived time variables</li>
            <li>Calculate profit and margin</li>
            <li>Engineer analytical features</li>
        </ul>
        
        <h3>SQL Query</h3>
        <p>Business-oriented SQL queries designed to answer key analytical questions such as revenue trends, customer segmentation, and seasonal performance.</p>
        
        <h3>SQL Query Results</h3>
        <p>Outputs from executed queries used to validate KPIs and dashboard metrics.</p>
        
        <h2>Cleaned Dataset – Data Dictionary</h2>
        <table>
            <thead>
                <tr>
                    <th>Column Name</th>
                    <th>Description</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>transaction_id</td>
                    <td>Unique transaction identifier</td>
                </tr>
                <tr>
                    <td>date</td>
                    <td>Transaction date</td>
                </tr>
                <tr>
                    <td>customer_id</td>
                    <td>Unique customer identifier</td>
                </tr>
                <tr>
                    <td>gender</td>
                    <td>Customer gender</td>
                </tr>
                <tr>
                    <td>age</td>
                    <td>Customer age (numeric)</td>
                </tr>
                <tr>
                    <td>age_group</td>
                    <td>Categorized age segment</td>
                </tr>
                <tr>
                    <td>product_category</td>
                    <td>Product category (Beauty, Clothing, Electronics)</td>
                </tr>
                <tr>
                    <td>quantity</td>
                    <td>Units purchased</td>
                </tr>
                <tr>
                    <td>price_per_unit</td>
                    <td>Selling price per unit</td>
                </tr>
                <tr>
                    <td>unit_cost</td>
                    <td>Cost per unit</td>
                </tr>
                <tr>
                    <td>total_amount</td>
                    <td>quantity × price_per_unit</td>
                </tr>
                <tr>
                    <td>revenue</td>
                    <td>Transaction revenue</td>
                </tr>
                <tr>
                    <td>total_cost</td>
                    <td>quantity × unit_cost</td>
                </tr>
                <tr>
                    <td>profit</td>
                    <td>revenue − total_cost</td>
                </tr>
                <tr>
                    <td>profit_margin</td>
                    <td>profit ÷ revenue</td>
                </tr>
                <tr>
                    <td>year</td>
                    <td>Extracted year</td>
                </tr>
                <tr>
                    <td>quarter</td>
                    <td>Extracted quarter</td>
                </tr>
                <tr>
                    <td>month</td>
                    <td>Numeric month</td>
                </tr>
                <tr>
                    <td>month_name</td>
                    <td>Month name</td>
                </tr>
                <tr>
                    <td>day_of_week</td>
                    <td>Day of week</td>
                </tr>
                <tr>
                    <td>is_weekend</td>
                    <td>Weekend indicator</td>
                </tr>
            </tbody>
        </table>
        
        <h2>Analytical Scope</h2>
        <p>This project includes:</p>
        <ul>
            <li>Monthly and quarterly revenue analysis</li>
            <li>Year-over-Year growth calculation</li>
            <li>Profitability by category</li>
            <li>Weekend vs Weekday performance</li>
            <li>RFM-based customer segmentation</li>
            <li>Seasonal performance index</li>
            <li>Top-performing products by quarter</li>
        </ul>
        
        <h3>Advanced SQL Techniques Applied</h3>
        <ul>
            <li>Common Table Expressions (CTEs)</li>
            <li>Window functions (RANK, LAG, NTILE)</li>
            <li>Moving averages</li>
            <li>Revenue contribution percentage</li>
        </ul>
    </div>
</body>
</html>
