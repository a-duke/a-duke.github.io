### Projections

---
## What is the Cartesian Product operation?
The cartesian product operation is a binary set operation, meaning it involves multiple relations. When the operation is applied, it will combine tuples together based on their entry row. 

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
## When is Projection useful?
Projection can be useful in many different scenarios. One use-case for this operation is when you need to limit the amount of data shown (or need to see only specific data). For example, if I wanted to only select the age and majors of every student at Ohio Northern but hide the rest of the student information, I would be able to use the projection operation to do so successfully!

Additionally, we can also leverage something called Extended Projection to make the result contain arbitrary expressions involving attriutes; such as arithmetic functions and duplicate occurences. I like to think of it as a mix between selections and projections (although it's not necessarily the correct idea, but you can use functions within the projection to achieve different results).

---
## So, what does this look like applied?
Projection is available in pretty much any Data Management System, including SQL. As shown in the example below (and described above), the SQL statement is selecting only the age and majors of Ohio Northern students from the ONU database table.

```sql
SELECT age a, major m 
  FROM ONU
 ;
```

---
## I’m still confused, do you have resources that might help me understand?
Sure, I do! Here are some of the resources that I used in research for this blog or that helped me during my time taking the course:
-
