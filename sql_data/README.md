# **Employee Analysis**

This projec was accomplished using SQL for data analysis, feature enegineering and data preprocessing.

### **Techniques used:**
- SQL funtions
- Views
- Subqueries
- Foreign keys
- Joins

### **Steps involved:**
- Create the tables
- Data preprocessing
	- Rename columns
	- Change datatypes
	- Rename values in columns; gender and marital_status
	- Drop rows with null type values in each column
- Perform eda 
- Feature engineering
	- Creating new columns (salary_after_tax, years_of_service) and re-arranging columns

## **Observations**
- There are 8 genders
	- Males have the highest count present in the data; 358
	- Males have the highest maximum salary after taxing; 396,498.00
	- Males have the highest number of employees in terms of positions
	- Genderfluid has the highest average and minimum salary after taxing; 327,876.00 and 230,787.00
	- Agender in position cto has the highest average salary after tax; 396,348.00

- There are 4 types of marital_status
	- Algeria has the highest number of married employees
	- Bahrain, Denmark, New Zealand, Ukraine and Cyprus has the highest number of single employees
	- Morocco has the highest number of widowed employees

- There are 12 positions present
	- cto and ceo have salaries above 350000 after taxing
	- cto's in male, female, agender, polygender, bigender, genderqueer and genderfluid have maximum salaries above 380000
	- An intern in male and female suffers loss after taxing their salary
	- ctos highest number of years of service with 16 ctos present
	- Position of vp, director, cto, cmo, cfo and ceo with a salary above 200,000, live in houses that ranked above 20

- Employees are from 99 countries
	- The country Bahrain has the highest number of employees present; 16
	- Indonesia, Thailand and Croatia have lowest number of employees present; 2
	- It seems Bahrain average salary after taxing is pretty low; 188,554.31. They could be of a lower position? Panama has the highest average salary after taxing
	- Apparently, not much employees are of high position from this country. So which country has the most number of employees in high positions; namely cto, ceo, cmo, cfo and vp? Panama only has employees in ceo, cto and vp position. Hence, their average salary will be high (less spread in data points)
	- Italy & Guatemala has the highest number of ceo's; 3
	- Germany has the highest number of cfo's; 3
	- Tunisia & Uruguay has the highest number of cmo's;  3
	- Poland and Algeria has the highest number of cto's; 4
	- Myanmar (Burma) has the highest number of vp; 4

- Looking the branches
	- Bahrain has the highest number of branches; 20
	- One of Democratic Republic of the Congo's branches amongst other countries has the highest maximum revenue generated; 9,992,041
	- One of Chile's branches  amongst other countries has the lowest revenue generated 
	- Kuwait has the highest average revenue generated


*NB:* Currency is in dollars and use the code format below to insert values for each table using SQL Shell (psql);

```\copy employee_details (employee_id, FIRStname, Lst_namE, EmaIL, gender,placeOFBirTH, "PositiON",salArY,Date_hired, "Material Status", CAr_owned, HOuse_owneDD) FROM 'C:\\file_path\\employee_details_salary_added.csv' WITH CSV HEADER DELIMITER ',';```