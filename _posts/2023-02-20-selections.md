### Selections

---
## What is the selection operation?
The selection operational in relational algebra is a unary operator that selects (for lack of better terms) attributes from a relation that meets specified criteria. 

It is a pretty straightforward operation, but to put it in readable English: selection is essentially an operation that picks certain rows within a database.
Still confused? Look at the animation below to see what I’m talking about:
[ANIMATION RENDER]

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

---
## When is Selection useful?

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

