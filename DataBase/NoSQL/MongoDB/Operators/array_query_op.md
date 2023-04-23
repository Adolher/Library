# Array Query Operators

**$all**

`db.<collection>.find( { field_array: { $all: [ <value1>, <value2> ] } } )`

---

**$elemMatch**

`db.<collection>.find( { field_array: { $elemMatch: { field: <value>, field: <value> } } } )`

---

**$size**

`db.<collection>.find( { field_array: { $size: n } } )`

---
