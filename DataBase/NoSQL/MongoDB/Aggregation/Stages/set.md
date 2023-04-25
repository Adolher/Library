<sup>[MongoDB Docs $set](https://www.mongodb.com/docs/manual/reference/operator/aggregation/set/)</sup>

# Set

```mongoDB
db.<collection>.aggregate([
    {
        $set:
        {
            <field>: <value>,
            <field>: <expression>
        }
    }
])
```

**return**: input documents with newly added fields

- appends new fields to existing documents

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/set/#example)

---
