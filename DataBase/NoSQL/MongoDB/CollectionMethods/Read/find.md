<sup>[MongoDB Docs .find()](https://www.mongodb.com/docs/manual/reference/method/db.collection.find/)</sup>

# Find

```mongoDB
db.<collection>.find(
    <query>,
    <projection>,
    <options>
)
```

**return**: a curser to the documents that match the query

- find documents
- (optional) projection: specifies the fields to return
- (optional) options: specifies options for the query
  - [Find Options](https://mongodb.github.io/node-mongodb-native/4.0//interfaces/findoptions.html)

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.find/#example)

---

## Projection

```mongoDB
{
    <field1>: <value>,
    "<field2>.<sub_field>": <value>,
    <field3>: <array_projection>,
    <field4>: <$meta expression>,
    <field5>: <aggregat expression>
}
```

- determines which fields are returned
- value == 0: specifies the exclusion of a field
- value != 0: specifies the inclusion of a field
- values needs to be all either 0 or not 0 except for _id-field

---
