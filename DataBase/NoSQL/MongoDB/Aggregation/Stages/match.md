<sup>[MongoDB Docs $match](https://www.mongodb.com/docs/manual/reference/operator/aggregation/match/)</sup>

# Match

```mongoDB
db.<collection>.aggregate([
    {
        $match: <query>
    }
])
```

**return**: documents which pass the query

- filters the documents according the query

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/match/#examples)
