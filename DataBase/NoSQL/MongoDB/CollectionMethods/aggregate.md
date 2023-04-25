<sup>[MongoDB Docs .aggregate()](https://www.mongodb.com/docs/manual/reference/method/db.collection.aggregate/)</sup>

# Aggregate

```mongoDB
db.<collection>.aggregate([
    {
        $stage1:
        {
            { <agg_operator1>: <argument1> }
        }
        $stage2:
        {
            { <agg_operator1>: <argument1> },
            { <agg_operator2>: [ <argument1>, <argument2> ] }
        }
    },
    <options>
])
```

**return**: a corser for resulting documents or, if the pipeline includes $out or $merge, an empty curser

- calculates aggregate values
- (optional) options: [Options](https://www.mongodb.com/docs/manual/reference/method/db.collection.aggregate/#definition)

[Example](https://www.mongodb.com/docs/manual/reference/method/db.collection.aggregate/#example)

---
