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
