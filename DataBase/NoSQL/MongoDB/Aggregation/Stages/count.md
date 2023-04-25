<sup>[MongoDB Docs $count](https://www.mongodb.com/docs/manual/reference/operator/aggregation/count/)</sup>

# Count

```mongoDB
db.<collection>.aggregate([
    {
        <stage>:
        {
            <field>: <expression>
        }
    },
    {
        $count: <string>
    }
])
```

**return**: count documents in a aggregation pipeline and assigns the value to \<string>

- counts documents in a pipeline

[Examples](https://www.mongodb.com/docs/manual/reference/operator/aggregation/count/#example)

---
