# Exp-8-Implement-the-keyword-Case-Cross-Join-full-outer-join
## AIM:
To implement CASE,CROSS,JOIN,FULL OURT JOIN in SQL.
## ALGORITHM:
STEP 1: Create a sample table in SQL using CREATE TABLE syntax
STEP 2: Insert all the values and Titles respectively using INSERT INTO syntax
STEP 3: Now check whether all the rows are affected or not by fetching the table
STEP 4: After checking, now use SELECT for choosing the column name that we want and use FROM to choose the table
STEP 5: Then use CASE,CROSS,JOIN,FULL OURT JOIN syntax to implement its functionality.
STEP 6: After compiling and running the program, the results will be displayed.
## PROGRAM:
### TABLE:
~~~
CREATE TABLE EMPLOYEE(
 	SNO int,
	FNAME varchar(50),
  	LNAME varchar(50),
	SALARY int
);
INSERT INTO EMPLOYEE VALUES (1,'John','MCFlury',8000);
INSERT INTO EMPLOYEE VALUES (2,'Vols','Vegan',4000);
INSERT INTO EMPLOYEE VALUES (3,'Amilia','Doofenshmirt',5000);
INSERT INTO EMPLOYEE VALUES (4,'Camilia','Jordan',3000);
INSERT INTO EMPLOYEE VALUES (5,'Max','Zeus',4500);
INSERT INTO EMPLOYEE VALUES (6,'Jacob','Norway',6700);
INSERT INTO EMPLOYEE VALUES (7,'Becky','Rodgerd',10000);
SELECT *FROM EMPLOYEE;
~~~
### CASE:
~~~
SELECT SALARY ,
CASE
	WHEN SALARY <= 3000 THEN 'LOW'
    WHEN SALARY > 3000 AND SALARY <= 5000 THEN 'AVG'
    ELSE 'HIGH'
END AS PREDICT
FROM EMPLOYEE
~~~
### FULL OUTER JOIN:
~~~
SELECT FRUITS.basket_id, BASKET.basket_id
FROM FRUITS
FULL OUTER JOIN BASKET ON FRUITS.basket_id=BASKET.basket_id
ORDER BY FRUITS.basket_id;
~~~
### CROSS JOIN:
~~~
SELECT SalesOrg.sales_org , Channel.channel
FROM SalesOrg
CROSS JOIN Channel;
~~~
### JOIN:
~~~
SELECT SalesOrg.sales_id , Channel.channel_id
FROM SalesOrg
JOIN Channel;
~~~
## OUTPUT:
### CASE:
![image](https://github.com/SdMdZahi7/Exp-8-Implement-the-keyword-Case-Cross-Join-full-outer-join/assets/94187572/e5dcc9fe-a504-463d-b4e5-70e3185e5ae1)

### FULL OUTER JOIN:
![image](https://github.com/SdMdZahi7/Exp-8-Implement-the-keyword-Case-Cross-Join-full-outer-join/assets/94187572/5e2b4fb5-40a4-4d0a-abeb-eaab4defad98)
### CROSS JOIN:
![image](https://github.com/SdMdZahi7/Exp-8-Implement-the-keyword-Case-Cross-Join-full-outer-join/assets/94187572/eb4af97b-2b12-436e-b9a5-399a6b48aaff)
### JOIN:
![image](https://github.com/SdMdZahi7/Exp-8-Implement-the-keyword-Case-Cross-Join-full-outer-join/assets/94187572/ccf6d6c7-3f05-4ee5-8f51-6717eef10375)

## RESULT:
Thus we have successfully obtained the required result using the above-given code.
