### Selections

---
## What is the selection operation?
The selection operational in relational algebra is a unary operator that selects (for lack of better terms) attributes from a relation that meets specified criteria. 

It is a pretty straightvforward operation, but to put it in readable English: selection is essentially an operation that picks certain rows within a database.
Still confused? Look at the animation below to see what I’m talking about:
![selection_1](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExM2NkMmUzOWIwMWI4ODJlMzVmYTMwZWE5ZjA3ZWU2MDdkM2JlZjVkNyZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PXM/qgSycr2SxBtUh5iPOh/giphy.gif)
---
## How is Selection represented in relational algebra?
Selection is often denoted with the Greek letter sigma (𝜎). Here’s an example of selection being written in relational algebra:
- 𝜎ₗ(R)
  - where 𝜎 is obviously the predicate (or the operation)
  - l is the logic being performed
  - R is the relation/the name of the table.

So... if we wanted to apply this format to a real-life example, we could!
- 𝜎ₛₜᵤₙᵤₘ₌₀₁₂₃₄₅₆₇₈₉(ONU)
  - This operation would select all of the rows within the ONU table that have the stuNum (student number) equal to 0123456789.

Another example of this can be seen through relational algebra and fancy symbols: σ(A > 5)(R) = {(a, b, c, d) | (a, b, c, d) ∈ R ∧ a > 5}
- I'm sure that looks complex, but don't freak out. This is simply saying to look at a relation containing ABCD and only take tuples where A is greater than 5. From there, everything else would be excluded and ignored for the operation.

[ANIMATION RENDER 2]

---
## When is Selection useful?
Selections are particularly useful when you need to simply filter entries in a database by a condition. Typically with selections, you will want to return the whole row (or tuple) from the table. However, in general, selection can be used to filter data, focus on specific subsets of a noted relation, and make queries more efficient- which can make it a very powerful tool to know.

---
## So, what does this look like applied?
This can be applied in any form of Database Management System, but for our sake, I am going to be displaying the same example above but in a SQL statement. The statement will be be selecting all students who have a student number of 0123456789 from the ONU table.

```sql
SELECT *
  FROM ONU
  WHERE stuNum = 0123456789
;
```

---
## I’m still confused, do you have resources that might help me understand?
Sure, I do! Here are some of the resources that I used in research for this blog or that helped me during my time taking the course:
- GeeksForGeeks (Article) [https://www.geeksforgeeks.org/select-operation-in-relational-algebra/]
- Guru99 (Article) [https://www.guru99.com/relational-algebra-dbms.html]
- Neso Academy (Video) [https://youtu.be/Givp56x6vbg]
- TutorialsPoint (Article) [https://www.tutorialspoint.com/explain-the-select-operation-in-relational-algebra-dbms]

