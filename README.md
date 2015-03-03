# govar
Go lang variable naming conventions.

No formatting or organization yet.

If you have a large team or contributing to open source, which the Go community strongly encourages, then use naming conventions that are widely accepted in the Go community.

http://doc.cat-v.org/bell_labs/pikestyle

List of common single character memory variables used in go.
<ul>
<li>i, n, k for/range.<li>
<li>v       value for range</li>
</ul>
<br>
not accepted:
<ul>
<li>m       mutex mu</li>
<li>e       error <b>err</b></li>
<li>t       type (t type)(t *type)receiver methods</li>
<li>p       parameter in a function/method func (t *type) fn(p param){}</li>

</ul>

<b>Variable naming rules.</b><br><br>
Use the shortest var name unless ambiguous or inconsistent with convention.<br><br>
Single letter memory variables are ambiguous unless:<br>
Usage is accepted by the Go community.<br>
An unambiguous initialization is close to all usage. (<b>less</b> than a screen)<br>
It is used in the majority of loc in a function/method. Used so often it disambiguates itself locally.<br><br>

Two letter memory variables are ambiguous:<br>
Too often these are needed because single letter names have been used in the same scope. Adding another letter just to avoid collision usually gains little while having multiple vars with the same starting letter. An acronym may help. Maybe try to build on accepted convention. If you are juggling more than error then e, er and err. Or make mu be RWMutex and m + the first letter of what it is covering be your rule. If you cannot achieve some clarity go to three or four letters.<br>

Three letter memory variables:<br>
acronyms: sql<br>
prefixes: max<br>

Four+ letter memory variables:<br>
Very few need to go to four. One that I find an exception is conn for connection. Others might find con or cn acceptable.<br>Unless the scope is global.<br>

Global vars and function naming<br>
I consider the naming needs of these to be similar. The further away from initialization it is called the increase in need of naming clarity.

Achieving max clarity with minimum length.
Prefix:<br>

How about password: pswrd or pw? (global local)



