# Footnotes

**Markdown**

    This is a Text with standard[^1] and longer[^2] footnotes.

    [^1]: This is a normal footnote
    [^2]: This is a long footnote  
        indent the line to include them to the footnote   
        and dont forget the colon!

**HTML**

    <p>This is a Text with standard<sup><a href=#fn1 id=fnref1>1</a></sup>
    and longer<sup><a href=#fn2 id=fnref2>2</a></sup> footnotes.</p>

    <footer>
        <ol>
            <li id=fn1> This is a normal footnote<sup><a href=#fnref1>1</a></sup> </li>
            <li is=fn2> This is a long footnote<br>indent the line to include them to the footnote<br>and dont forget the colon!<sup><a href=#fnref2>2</a></sup></li>
        </ol>
    </footer>

**Output**

This is a Text with standard[^1] and longer[^2] footnotes.

[^1]: This is a normal footnote
[^2]: This is a long footnote  
    indent the line to include them to the footnote   
    and dont forget the colon!