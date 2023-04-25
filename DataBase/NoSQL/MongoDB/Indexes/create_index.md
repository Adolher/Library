# Create Index

`db.<collection>.createIndex( <key>, <option>, commitQuorum)` *( Single Field Index )*
`db.<collection>.createIndex( { <key1>, <key2>, <key3> }, <option>, commitQuorum)` *(Compound Indexes )*

[MongoDB Documents](https://www.mongodb.com/docs/manual/reference/method/db.collection.createIndex/)

---

**\<key>**

`{ <field>: <value> }`

- \<field> is the index-key
- if \<field> is an array, it will be an *Multikey Index*
- \<value> == 1: ascending
- \<value> == -1: descending

**\<options>**

- unique
- name
- partialFilterExpression
- sparse
- expireAfterSeconds
- hidden
- storageEngine
- collation
