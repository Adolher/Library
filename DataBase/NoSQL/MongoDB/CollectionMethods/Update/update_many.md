# Update Many

`db.<collection>.updateMany( <query>, { <update_operator>: { field: <value> } }, { <option>: option_value> } )`

- updates all documents which matches the query

---

## \<options>

**upsert**

- `boolean`
- default: `false`
- updates the document which match the query
- creates new document if no document match the query

<sup>[MongoDB Docs .updateMany()](https://www.mongodb.com/docs/manual/reference/method/db.collection.updateMany/)</sup>

# Update Many

```mongoDB
db.collection.updateMany(
   <query>,
   <update>,
   {
     upsert: <boolean>,
     writeConcern: <document>,
     collation: <document>,
     arrayFilters: [ <filterdocument1>, ... ],
     hint:  <document|string>        // Available starting in MongoDB 4.2.1
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

- updates all documents that match the query
- update: document or pipeline: specifies th update criteria
- (optional) upsert: boolean:
  - default: false
  - true: create new document if no document match the query OR update a single document that match the query
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) [collation](https://www.mongodb.com/docs/manual/reference/collation/)
- (optional) arrayFilters: array: array of filter documents that determine which array elements to modify for an update operation on an array field
- (optional) hint : an index name or the index specification to use for the query

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.updateMany/#example)

---
