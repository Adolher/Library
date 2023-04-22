# Update Operators

---

## Field Update Operators

**$set**

- replaces the value of a field
- if the field does not exists, it will be added

```mongodb
{
    $set:
    {
        <field>: <value>,
        <field>: [ <value1>, <value2> ],
        <field>: { <field1>: <value1>, <field2>: <value2> }
    }
}
```

---

## Array Update Operators

**$push**

- appends a value to an array
- if the array does not exists, it will be added with value as its element
- if \<value> is an array, it will be appended as an array as single element
- if the field is not an array, the operation will fail

```mongodb
{
    $push:
    {
        <field>: <value>,
        <field>: [ <value1>, <value2> ],
        <field>: { <modifier>: [ <value1>, <value2> ] }
    }
}
```

---
