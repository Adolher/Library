# Logical Operators

**$and**

`db.<collection>.find( { field: <value>, field: <value> } )`

`db.<collection>.find( { $and: [ { field: <value>}, { field: { <operator>: <value> } } ] } )`

---

**$not**

`db.<collection>.find( { field: { $not: <value> } } )`

`db.<collection>.find( { field: { $not: { <operator>: <value> } } } )`

---

**$nor**

`db.<collection>.find( { $nor: [ { field: <value> }, { field: { <operator>: <value> } } ] } )`

---

**$or**

`db.<collection>.find( { $or: [ { field: <value> }, { field: { <operator>: <value> } } ] } )`

---
