<sup>[MongoDB Docs .findAndModify()](https://www.mongodb.com/docs/manual/reference/method/db.collection.findAndModify/)</sup>

# Find And Modify

```mongoDB
db.collection.findAndModify(
{
    query: <query>,
    sort: <document>,
    remove: <boolean>,
    update: <document or aggregation pipeline>,
    new: <boolean>,
    fields: <document>,
    upsert: <boolean>,
    bypassDocumentValidation: <boolean>,
    writeConcern: <document>,
    collation: <document>,
    arrayFilters: [ <filterdocument1>, ... ],
    let: <document>
})
```

**return**: [Return Data](https://www.mongodb.com/docs/manual/reference/method/db.collection.findAndModify/#return-data)

```mongoDB

```

- modifies a single document
- (optional) query: a query document
- (optional) sort:
- remove OR update: boolean: remove or update the specified document
- (optional) new: boolean:
  - default: false: returns the original document
  - true: returns the modified document
- (optional) [fields](#fields-fields): document
  - specifies the fields to return
- (optional) upsert: boolean:
  - default: false
  - true: create new document if no document match the query OR update a single document that match the query
- (optional) bypassDocumentValidation: boolean:
  - default: false
  - true: bypass document validation during the operation
- (optional) [writeConcern](https://www.mongodb.com/docs/manual/reference/write-concern/)
- (optional) maxTimeMS: int: specifies a time limit in ms
- (optional) [collation](https://www.mongodb.com/docs/manual/reference/collation/)
- (optional) arrayFilters: array: array of filter documents that determine which array elements to modify for an update operation on an array field
- (optional) let: document: specifies a document with a list of variables

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.findAndModify/#example)

---

## Fields {#fields}

```mongoDB
{
    <field1>: <value>,
    "<field2>.<sub_field>": <value>,
    <field3>: <array_projection>,
    <field5>: <aggregat expression>
}
```

- determines which fields are returned
- value == 0: specifies the exclusion of a field
- value != 0: specifies the inclusion of a field
- values needs to be all either 0 or not 0 except for _id-field

---
