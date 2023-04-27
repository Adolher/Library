<sup>[MongoDB Docs .limit()](https://www.mongodb.com/docs/manual/reference/method/cursor.limit/)</sup>

# Limit

```mongoDB
db.<collection>.<method>(<query>).limit(<value>)
```

- specifies the max number of documents, the curser will return
- value must be numeric
- value == 0: no Limit
- value \< -2<sup>31</sup> OR value \> 2<sup>31</sup> : behavior undefined
- -value == value but closes the curser after returning a single batch of results

---
