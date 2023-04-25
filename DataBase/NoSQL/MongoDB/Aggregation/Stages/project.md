<sup>[MongoDB Docs $project](https://www.mongodb.com/docs/manual/reference/operator/aggregation/project/)</sup>

# Project

```mongoDB
db.<collection>.aggregate([
    {
        $project:
        {
            <field>: <value>,
            <field>: <expression>
        }
    }
])
```

**return**: documents with the requested fields

- `<field>: <expression>` adds a new field or resets the value of an existing one
- determines which fields are returned
- value == 0: specifies the exclusion of a field
- value != 0: specifies the inclusion of a field
- values needs to be all either 0 or not 0 except for _id-field

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/project/#example)

---
