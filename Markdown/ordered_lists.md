# Ordered Lists

**Markdown**

    1. item
    2. item
    3. item

**HTML**

    <ol>
        <li> item </li>
        <li> item </li>
        <li> item </li>
    </ol>

**Output**
1. item
2. item
3. item

---

**Markdown**  

    1. item
    2. item
        1. intended item  
        2. intended item  
    3. item

**HTML**

    <ol>
        <li> item </li>
        <li> item </li>
            <ol>
                <li> item </li>
                <li> item </li>
            </ol>
        <li> item </li>
    </ol>

**Output**
1. item
2. item
   1. intended item
   2. intended item
3. item

---
