<sup>[MongoDB Docs $limit](https://www.mongodb.com/docs/manual/reference/operator/aggregation/limit/)</sup>

# Limit

```mongoDB
db.<collectio>.aggregate([
    {
        $limit: <value>
    }
])
```

**return**: documents

- value must be positive 64-bit integer
- limits the number of documents

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/limit/#example)

---
