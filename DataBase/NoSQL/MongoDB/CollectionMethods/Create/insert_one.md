<sup>[MongoDB Docs .insertOne()](https://www.mongodb.com/docs/manual/reference/method/db.collection.insertOne/)</sup>

# Insert One

```mongoDB
db.<collection>.insertOne(
    <document>,
    {
        writeConcern: <document>
    }
)
```

**return**:

```mongoDB
{
    "acknowledged": <boolean>,
    "insertedId": <ObjectId>
}
```

- insert a single document
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.insertOne/#example)

---
