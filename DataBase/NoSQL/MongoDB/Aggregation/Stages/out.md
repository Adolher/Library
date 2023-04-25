<sup>[MongoDB Docs $out](https://www.mongodb.com/docs/manual/reference/operator/aggregation/out/)</sup>

# Out

```mongoDB
db.<collection>.aggregate([
    {
        $out:
        {
            db: <db>,
            coll: <collection>
        }
    }
])
```

**return**: documents

- must be the last in a pipeline
- writes the documents to collection in database
- collection and database will be created if not exists
- collection and database will be replaced if exists
- if db is not specified, the same db will be used

[Example](https://www.mongodb.com/docs/manual/reference/operator/aggregation/out/#example)

---
