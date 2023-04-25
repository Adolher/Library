<sup>[MongoDB Docs $search (aggregation)](https://www.mongodb.com/docs/manual/reference/operator/aggregation/search/)</sup>

# Search

```mongoDB
{
  $search:
  {
    "index": "<index-name>",
    "<operator-name>"|"<collector-name>": { <operator-specification>|<collector-specification> },
    "highlight": { <highlight-options> },
    "count": { <count-options> },
    "returnStoredSource": true | false
  }
}
```

**return**: results of the query

- must be the first stage in a pipeline
- performs a full-text search of the field or fields
- fields must be covered by an [Atlas Search Index](https://www.mongodb.com/docs/atlas/atlas-search/index-definitions/)

---

- Read [Atlas Search](https://www.mongodb.com/docs/atlas/atlas-search/)
