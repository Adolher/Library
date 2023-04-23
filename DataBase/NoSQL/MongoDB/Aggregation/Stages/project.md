# Project

`{ $project: <projection> }`

---

**\<projection>**

```mongodb
{
    <field1>: <value>,
    <field2>: <expression>
}
```

- `<field>: <expression>` adds a new field or resets the value of an existing one
- determines which fields are returned
- value == 0: specifies the exclusion of a field
- value != 0: specifies the inclusion of a field
- values needs to be all either 0 or not 0 except for _id-field

---
