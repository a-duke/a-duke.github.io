### Cartesian Products

---
## What is the Cartesian Product operation?
The cartesian product operation is a binary set operation, meaning it involves multiple relations. When the operation is applied, it will combine tuples together based on their entry row. This is also sometimes called a cross join.

What this means is, the operation will combine two tuples (relations) together and place them side-by-side into one, combned tuple. Still confused? See the animation below to see what I'm talking about:

[ANIMATION RENDER]

---
## How is Cartesian Products represented in relational algebra?
Cartesian Products are often denoted with the Greek letter chi (✕). An example operation can be found below:
-  R1✕R2
  - where R1 is the first relation/tuple
  - ✕ is the cartesian product operation
  - R2 s the second relation/tuple

What would this look like applied to a real table? Let's see!
- StudentPersonalInfo ✕ StudentFinancialInfo
  - This would combine student's personal information with their financial information.
  - It is important to note, that the DBMS (database management system) will NOT automatically sync the tables with the appropriate data, meaning that every student's information may not perfectly align with the correct data. To accomplish this, it is essentially to use the select operator to define matching parameters.

---
## When is a Cartesian Product useful?
Cartesian Products can be useful in a variety of situations, but should be used carefully. Used on larger databases, this gets significantly more expensive as the size and complexity of a database increases. The best use of this operation is in conjunction with other operations, such as selections- as it is rarely useful alone. For example, this could useful when multiple tables are needing referenced or leveraged in one way or another.

---
## So, what does this look like applied?
Cartesian products are performed by selecting multiple tables within one operation. So, the example below will select all of the information from the database for student's personal information and their financial information.

```sql
SELECT *
  FROM StudentPersonalInfo spi, StudentFinancialInfo sfi
 ;
```

---
## I’m still confused, do you have resources that might help me understand?
Sure, I do! Here are some of the resources that I used in research for this blog or that helped me during my time taking the course:
- GeeksForGeeks (Article) [https://www.geeksforgeeks.org/cartesian-product-operation-in-relational-algebra/#]
- TutorialsPoint (Article) [https://www.tutorialspoint.com/sql/sql-cartesian-joins.htm]
- Neso Academy (Video) [https://youtu.be/qvioqCvvMek]
