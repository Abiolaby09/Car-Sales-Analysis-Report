   # Car-Sales-Analysis-Report
This is a sales report of product by transmissions, countries, Gender and many more

---
##   Car_sales_analysis
_This report gives an insight about car sales data in the United States_

__This also contains dashboard__

---
## Project Overview
> This project bring to view the analytical report of car sales data to uncover insights on sales distribution by various attributes such as Gender, state, Transmission, color, price and many more using power bi, SQL, MS Excel, i explored metrics like all the details of all the car on the data and ,fetched all the name of customers who purchased cars, car companies , list of cars some particular amount and i explored metrics like car sold by region, transmission, company, dealer and gender. This analysis helps to understand the key factors driving cars in the United States nd identifies major patterns across different segments.

## Data source:
+ www.kaggle.com

## Tools used 
### Power Bi:
        1. For recreating interactive visualization
        2.For Dashboard Creation
        3. For visuals that present data insights in a user-friendly format
## Data Overview
_The dataset includes the following columns:_
> __ Car_ID: Unique identifier of the car__
> + Date: Date the car was purchased
> + Customer_Name: Name of the customer
> - Gender: Customer's Gender
> - Annual_Income: Customer's annual income
> - Delaer_Name:Name of the dealer
> - Company: Company the car was purchased from
> - Model:Model of the car
> - Engine: Type of engine
> - Transmission:Mode of transmisson of the car
> - Color: Color of the car
> - Price: The worthof the car
> - Dealer_No: Phone number of the dealer
> - Body_style: Type of car 
> - Phone: Customer's phone number
> - Dealer_Region: Geographic location where the car was sold
## Data Visualization
To view the data Bi dashboard , click here 

## Dashboard Visuals ![Uploading car sales dashboard.png…]()


## SQL
```sql
SELECT * FROM CarSales
```

```sql
SELECT Car_id FROM CarSales
```

```sql
SELECT DISTINCT [Customer Name] FROM CarSales;
```

```sql
SELECT DISTINCT Company FROM CarSales;
```

```sql
SELECT * FROM CarSales WHERE [Price ($)] > 400000;
```

```sql
SELECT * FROM CarSales WHERE Dealer_Region = 'Austin';
```

```sql
SELECT * FROM CarSales WHERE Transmission = 'Automatic';
```

```sql
SELECT Company, AVG([Price ($)]) AS AvgPrice FROM CarSales GROUP BY Company;
```

```sql
SELECT Dealer_Region, SUM([Price ($)]) AS TotalRevenue FROM CarSales GROUP BY Dealer_Region;
```

```sql
SELECT Gender, COUNT(Car_id) AS CarsSold FROM CarSales GROUP BY Gender;
``







