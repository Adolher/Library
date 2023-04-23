# Find Documents

---

**Find All**

`db.<collection>.find()`

---

**Find Document with query**

`db.<collection>.find( <query> )`

---

**Find Document with projection**

`db.<collection>.find( <query>, <projection> )`

---

**\<projection>**

```mongodb
{
    <field1>: <value>,
    "<field2>.<sub_field>": <value>,
    <field3>: <array_projection>,
    <field4>: <$meta expression>,
    <field5>: <aggregat expression>
}
```

- determines which fields are returned
- value == 0: specifies the exclusion of a field
- value != 0: specifies the inclusion of a field
- values needs to be all either 0 or not 0 except for _id-field

---
