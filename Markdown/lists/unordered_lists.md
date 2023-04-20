# Unordered Lists

**Markdown**

    - item
    - item
    - item

**HTML**

    <ul>
        <li> item </li>
        <li> item </li>
        <li> item </li>
    </ul>

**Output**
- item
- item
- item

---

**Markdown**  

    - item
    - item
        - intended item  
        - intended item  
    - item

**HTML**

    <ul>
        <li> item </li>
        <li> item </li>
            <ul>
                <li> item </li>
                <li> item </li>
            </ul>
        <li> item </li>
    </ul>

**Output**
- item
- item
   - intended item
   - intended item
- item

---
