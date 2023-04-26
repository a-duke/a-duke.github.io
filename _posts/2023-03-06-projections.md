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

Another example of this could look like: П(A, C)(R) = {(a, c) | ∃b, d (a, b, c, d) ∈ R}.
- If you're anything like me, that probably looks like another language! I promise it's not that bad and is simply explaining that is is selecting ONLY columns A and C from the relation ABCD and then will project only those two.

[ANIMATION RENDER 2?]

---
## When is Projection useful?
Projection can be useful in many different scenarios. One use-case for this operation is when you need to limit the amount of data shown (or need to see only specific data). For example, if I wanted to only select the age and majors of every student at Ohio Northern but hide the rest of the student information, I would be able to use the projection operation to do so successfully!

Additionally, we can also leverage something called Extended Projection to make the result contain arbitrary expressions involving attriutes; such as arithmetic functions and duplicate occurences. I like to think of it as a mix between selections and projections (although it's not necessarily the correct idea, but you can use functions within the projection to achieve different results).

All-in-all, projection is a very useful operation, as it allows us to extract specific information from a relation without having to manipulate the entire relation. We can also use to reduce the size of a relation, focus on specific attributes of interest, and make queries more efficient. So used wisely, this operation can come in very handy!

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
- Wikipedia (Article) [https://en.wikipedia.org/wiki/Projection_(relational_algebra)]
- TutorialsPoint (Article) [https://www.tutorialspoint.com/explain-project-operation-in-relational-algebra-dbms]
- Swati Chawla (Video) [https://youtu.be/VBzU0n-8DeE]
