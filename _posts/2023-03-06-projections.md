### Projections

---
## What is the projection operation?
The projection opertion in relational algebra is a unary operator that selects an entire vertical subset of values from a relation. Projections are similar to the select operator, but instead it extracts values of a specified attribute and eliminates duplicates.

In other words, this operation selects an entire column and projects it with specific attributes only and without duplicates. Still confused? Look at the animation below to see what I'm talking about:

[ANIMATION RENDER]

---
## How is Projection represented in relational algebra?
Projection is often denoted with the Greek letter pi (П). An example operation can be found below:
-  Пc(R)
  - where П is the projection operation
  - c is the column(s) being selected
    - Yes, you can select multiple columns from one operation!
  - R is the relation/the name of the table

What would this look like applied to a real table? Let's see!
- Пₛₜᵤₙᵤₘ, ₘₐⱼₒᵣ, ᵤₚₘ(ONU)
  - This would project the column stuNum, major, and upm from the ONU table. This scenario would then only show ONU student numbers, majors, and upperclassman status.

---
## When is Projection useful?
Projection can be useful in many different scenarios. One use-case for this operation is when you need to limit the amount of data shown (or need to see only specific data). For example, if I wanted to only select the age and majors of every student at Ohio Northern but hide the rest of the student information, I would be able to use the projection operation to do so successfully!

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
