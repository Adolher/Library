# Limit

`<curser>.limit( <value> )`

**\<value>**

- value must be numeric
- value == 0: no Limit
- value \< -2<sup>31</sup> OR value \> 2<sup>31</sup> : behavior undefined
- -value == value but closes the curser after returning a single batch of results
