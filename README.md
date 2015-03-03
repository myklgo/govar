# govar
Go lang variable naming conventions.

No formatting or organization yet.

If you have a large team or contributing to open source, which the Go community strongly encourages, then use naming conventions that are widely accepted in the Go community.

http://doc.cat-v.org/bell_labs/pikestyle

List of common single character memory variables used in go.
<ul>
<li>i, n, k integers used in range. k is used as any key type because of mnemonic</li>
<li>v       value used in range</li>
</ul>
<br>
not accepted:
<ul>
<li>m       mutex</li>
<li>e       error should be used instead of err</li>
<li>t       type for receiver methods</li>
<li>p       parameter in afunction/method func (t *type) fn(p param){}</li>
</ul>

List of variable naming rules in order of importance.

<b>Consistency</b> Being more important than disambiguous may seem counter intuitive. However consistency shrinks ambiguity over time, therefore more powerful.
<b>Disambiguous</b>
<b>Length</b>

Single letter memory variables.

It is consistently used by the Go community.
An unambiguous initialization is close to all usage. (less than a screen, preferrably much less)
It is used in the majority of loc in a function/method. Used so often it disambiguates itself. 

Two letter memory variables.


