<sup>[MongoDB Docs .explain()](https://www.mongodb.com/docs/manual/reference/method/db.collection.explain/)</sup>

# Explain

```mongoDB
db.<collection>.explain(<mode>).<method>
```

**return**: explain results

- returns information on the query plan
- modes: queryPlannerMode (Default), executionStats, allPlansExecution
- methods: help(), \<method>.help(), aggregate(), find(), distinct(), count(), remove(), findAndModify()

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.explain/#example)

---
