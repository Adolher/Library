# Count Documents

`db.<collection>.countDocuments( <query>, <options> )`

---

**\<options>**

1. `{ limit: <number> }`
   - max number of documents to count
2. `{ skip: <number> }`
   - number of documents to skip before counting
3. `{ hint: <string> }`
   - an index name or the index specification to use for the query
4. `{ maxTimeMS: <number> }`
   - max amount of time allow the count to run in ms

---
