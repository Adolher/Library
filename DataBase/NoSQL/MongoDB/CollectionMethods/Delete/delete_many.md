<sup>[MongoDB Docs .deleteMany()](https://www.mongodb.com/docs/manual/reference/method/db.collection.deleteMany/)</sup>

# Delete Many

```mongoDB
db.<collection>.deleteMany(
    <query>,
    {
        writeConcern: <document>,
        collation: <document>
    }
)
```

**return**:

```mongoDB
{
    "acknowledged" : <boolean>,
    "deletedCount" : <value>
}
```

- delete all documents that match the query
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) [collation](https://www.mongodb.com/docs/manual/reference/collation/)

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.deleteMany/#example)

---
