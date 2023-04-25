<sup>[MongoDB Docs $sort](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sort/)</sup>

# Sort

```mongoDB
db.<collection>.aggregate([
    {
        $sort:
        {
            <field>: <value>
        }
    }
])
```

**return**: sorted documents

- you can sort max 32 \<field>
- \<value> == 1: ascending
- \<value> == -1: descending

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/sort/#example)

---
