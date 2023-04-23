# Aggregate

`db.<collection>.aggregate( <pipeline>, <options> )`  

[MongoDB Documents](https://www.mongodb.com/docs/manual/reference/method/db.collection.aggregate/)

---

**\<pipeline>**

`[ { <stage1> }, { <stage2> } ]`

```mongoDB
[
    {
        $stage1:
        {
            { <expression1> }
        }
        $stage2:
        {
            { <expression2> },
            { <expression3> }
        }
    }
]
```

```mongoDB
[
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
    }
]
```

---
