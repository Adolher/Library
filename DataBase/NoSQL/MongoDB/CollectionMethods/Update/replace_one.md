# Replace One

`db.<collection>.replaceOne( <query>, <document>, {options})`

- replaces the first document which matches the query
- keeps the _id
- if replaceOne() changes the Document size, the operation will fail
