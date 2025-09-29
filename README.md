# Northwind Dataset Analysis 📊🌍

This repository contains a series of SQL queries executed on the **Northwind dataset**, which simulates a trading company. The dataset includes information about customers, products, and orders, providing a rich environment for data analysis.

## Key Queries

1. **📘 Retrieve Full Customer Data**  
   Exported the full list of all customer details into a report.
   ```sql
   SELECT * FROM Customers;
2. 📘 Customer Names and Cities for Marketing
Retrieved customer names and their cities for targeted marketing campaigns.
   ```sql
   SELECT CustomerName, City FROM Customers;

3. 📘 Unique Cities for Delivery Network Expansion
Identified all distinct cities where customers are located to aid logistics planning.
   ```sql
   SELECT DISTINCT City FROM Customers;
   
4. 📘 High-Value Products Report
Analyzed products priced over £50 to focus on high-value items.
   ```sql   
   SELECT * FROM Products WHERE Price > 50;
   
5. 📘 International Customers Targeting (USA & UK)
Retrieved customer data for targeted marketing campaigns in the USA and UK.
   ```sql
   SELECT * FROM Customers WHERE Country = 'USA' OR Country = 'UK';
   
6. 📘 Recent Orders Report
Analyzed the latest orders by retrieving all columns from the Orders table, sorted by order date.
   ```sql
   SELECT * FROM Orders ORDER BY OrderDate DESC;
   
7. 📘 Mid-Range Products Listing
Prepared a product list for items priced between £20 and £50, ordered by descending price.
   ```sql
   SELECT * FROM Products WHERE Price BETWEEN 20 AND 50 ORDER BY Price DESC;
   
8. 📘 Local Marketing in the US (Portland & Kirkland)
Focused on customers from Portland and Kirkland in the USA for local marketing efforts.
   ```sql
   SELECT * FROM Customers WHERE Country = 'USA' AND City IN ('Portland', 'Kirkland') ORDER BY CustomerName ASC;
   
Conclusion
These queries demonstrate the versatility of SQL in extracting valuable insights from the Northwind dataset, aiding in marketing strategies, inventory management, and customer analysis. 🚀
