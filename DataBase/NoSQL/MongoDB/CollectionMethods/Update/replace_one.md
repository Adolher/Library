<sup>[MongoDB Docs .replaceOne()](https://www.mongodb.com/docs/manual/reference/method/db.collection.replaceOne/)</sup>

# Replace One

```mongoDB
db.collection.replaceOne(
   <filter>,
   <replacement>,
   {
     upsert: <boolean>,
     writeConcern: <document>,
     collation: <document>,
     hint: <document|string>
   }
)
```

**return**:

```mongoDB
{
   "acknowledged" : true,
   "matchedCount" : <int>,
   "modifiedCount" : <int>,
   "upsertedId" : <int>         // if upsert == true
}
```

- replace the first document that match the filter
- keeps the _id
- if replaceOne() changes the Document size, the operation will fail
- (optional) upsert: boolean:
  - default: false
  - true: create new document if no document match the query OR update a single document that match the query
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) [collation](https://www.mongodb.com/docs/manual/reference/collation/)
- (optional) hint : an index name or the index specification to use for the query

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.replaceOne/#example)

---
