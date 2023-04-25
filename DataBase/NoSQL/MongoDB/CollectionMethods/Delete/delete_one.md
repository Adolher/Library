<sup>[MongoDB Docs .deleteOne()](https://www.mongodb.com/docs/manual/reference/method/db.collection.deleteOne/)</sup>

# Delete One

```mongoDB
db.<collection>.deleteOne(
    <query>,
    {
        writeConcern: <document>,
        collation: <document>,
        hint: <document|string>
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

- delete the firs document that match the query
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) [collation](https://www.mongodb.com/docs/manual/reference/collation/)
- (optional) hint: specifies the index to use

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.deleteOne/#example)

---
