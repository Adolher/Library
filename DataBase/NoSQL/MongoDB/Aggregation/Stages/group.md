# Group

```mongoDB
db.<collection>.aggregate(
    [
        {
            $group:
            {
                _id: <expression>,
                <field>:
                {
                    <agg_acc_operator1>: <expression1>
                },
                <field2>:
                {
                    <agg_acc_operator1>: <expression1>
                }
            }
        }
    ]
)
```
