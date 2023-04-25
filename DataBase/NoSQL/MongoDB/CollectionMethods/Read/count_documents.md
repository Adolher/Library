<sup>[MongoDB Docs .countDocuments()](https://www.mongodb.com/docs/manual/reference/method/db.collection.countDocuments/)</sup>

# Count Documents

```mongoDB
db.<collection>.countDocuments(
   <query>,
   <options>
)
```

**return**: the count of documents that match the query

- (optional) options: options that affects the count behavior
  - `{ limit: <number> }` max number of documents to count
  - `{ skip: <number> }` number of documents to skip before counting
  - `{ hint: <string> }` an index name or the index specification to use for the query
  - `{ maxTimeMS: <number> }` max amount of time allow the count to run in ms

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.countDocuments/#example)

---
