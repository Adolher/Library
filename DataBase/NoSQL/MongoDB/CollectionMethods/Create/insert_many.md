<sup>[MongoDB Docs .insertMany()](https://www.mongodb.com/docs/manual/reference/method/db.collection.insertMany/)</sup>

# Insert Many

```mongoDB
db.<collection>.insertMany(
    [
        <document1>,
        <document2>,
        <document3>
    ],
    {
        writeConcern: <document>,
        ordered: <boolean>
    }
)
```

**return**:

```mongoDB
{
    "acknowledged": <boolean>,
    "insertedIds": [ <ObjectId>, <ObjectId> ]
}
```

- insert multiple documents into a collection
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) ordered: default: true
  - specifies if an ordered or unordered insert will be performed

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.insertMany/#example)

---
