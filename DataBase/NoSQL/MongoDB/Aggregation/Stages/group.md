<sup>[MongoDB Docs $group](https://www.mongodb.com/docs/manual/reference/operator/aggregation/group/)</sup>

# Group

```mongoDB
db.<collection>.aggregate(
    [
        {
            $group:
            {
                _id: <expression>,
                <field>:
                {
                    <agg_operator1>: <expression1>
                },
                <field2>:
                {
                    <agg_acc_operator1>: <expression1>
                }
            }
        }
    ]
)
```

**return**: one document for each unique group key (_id: \<expression>)

- separates documents into groups according a group key

[Examples](https://www.mongodb.com/docs/manual/reference/operator/aggregation/group/#example)

---
