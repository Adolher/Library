# Update One

`db.<collection>.updateOne( <query>, { <update_operator>: { field: <value> } }, { <option>: option_value> } )`

- updates the first document which matches the query

---

## \<options>

**upsert**

- `boolean`
- default: `false`
- updates the document which match the query
- creates new document if no document match the query
