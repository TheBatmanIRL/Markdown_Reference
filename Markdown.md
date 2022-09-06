# A GitHub Markdown Cheatsheet

This show usable Markdown features on GitHub as a side by side comparison. This focuses on Markdown _files_, while most of also works in comments etc., there are some differences, so keep that in mind.

### Table of Contents

[Headings](#headings)  
[Line Breaks](#line-breaks)  
[Inline text formatting](#inline-text-formatting)  
[Links](#links)  
[Horizontal Rule](#horizontal-rule)  
[Code and Syntax Highlighting](#code-and-syntax-highlighting)  
[Maths](#maths)  
[Blockquotes](#blockquotes)  
[Lists](#lists)  
[Definition lists](#definition-lists)  
[Tables](#tables)  
[Images](#images)  
[Sources and more information](#sources-and-more-information)  


<!-- -------------------------------------------- -->
## Headings

<table>
<td width="500px">

# h1

## h2

### h3

#### h4

##### h5

###### h6

</td>
<td width="500px">

```no-highlight
# h1

## h2

### h3

#### h4

##### h5

###### h6
```

</td>
</table>


<!-- -------------------------------------------- -->
## Line Breaks

<table>
<td width="500px">

Here's a line for us to start with.

Leave a blank line to start a *separate paragraph*.

This line is also a separate paragraph, but...
continuing on the next line puts in the *same paragraph*.

You can also put manual line-breaks  
with two spaces at the end of the line  
or with HTML <br>

</td>
<td width="500px">

```no-highlight
Here's a line for us to start with.

Leave a blank line to start a *separate paragraph*.

This line is also a separate paragraph, but...
continuing on the next line puts in the *same paragraph*.

You can also put manual line-breaks  
with two spaces at the end of the line  
or with HTML <br>
```

</td>
</table>


<!-- -------------------------------------------- -->
## Inline text formatting

<table>
<td width="500px">

*Emphasis*, aka *italics*, (*this* also works)

**Strong emphasis**, aka **bold**, (or **this**)

**Combined *both* in one context**

~~Strikethrough~~ uses two tildes

Inline code with `single backticks`.

Inline Math $a=1+2$ with LaTeX

*HTML Options:*

<kbd>User input</kbd> with `<kbd>`

<samp>Program output</samp> with `<samp>`

Mark <var>variables</var> with `<var>`

<ins>inserted</ins> Text with `<ins>`

<del>deleted Text</del> with `<del>`

<q>Quote</q> with `<q>` to get quotation marks

Subscript<sub>sub</sub> with `<sub>` and
Superscript<sup>sup</sup> with `<sup>`

</td>
<td width="500px">

```no-highlight
_Emphasis_, aka _italics_, (*this* also works)

**Strong emphasis**, aka **bold**, (or __this__)

**Combined _both_ in one context**

~~Strikethrough~~ uses two tildes

Inline code with `single backticks`.

Inline Math $a=1+2$ with LaTeX


_HTML Options:_

<kbd>User input</kbd> with `<kbd>`

<samp>Program output</samp> with `<samp>`

Mark <var>variables</var> with `<var>`

<ins>inserted</ins> Text with `<ins>`

<del>deleted Text</del> with `<del>`

<q>Quote</q> with `<q>` to get quotation marks

Subscript<sub>sub</sub> with `<sub>` and
Superscript<sup>sup</sup> with `<sup>`
```

</td>
</table>


<!-- -------------------------------------------- -->
## Links

<table>
<td width="500px">

[inline-style link](https://www.example.com)

[inline-style link with title](https://www.example.com "Hover Me")

[reference-style link][Arbitrary case-insensitive label]

[relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself]

URLs and URLs in angle brackets will automatically get turned
into links. <http://www.example.com> or <http://www.example.com>
and sometimes example.com (but not on Github, for example).

And HTML also works here: <a href="https://github.com">GitHub</a>

Some text to show that the reference links can follow later.

[Arbitrary case-insensitive label]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

</td>
<td width="500px">

```no-highlight
[inline-style link](https://www.example.com)

[inline-style link with title](https://www.example.com "Hover Me")

[reference-style link][Arbitrary case-insensitive label]

[relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself]

URLs and URLs in angle brackets will automatically get turned
into links. http://www.example.com or <http://www.example.com>
and sometimes example.com (but not on Github, for example).

And HTML also works here: <a href="https://github.com">GitHub</a>

Some text to show that the reference links can follow later.

[Arbitrary case-insensitive label]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com
```

</td>
</table>


<!-- -------------------------------------------- -->
## Horizontal Rule

<table>
<td width="500px">

Three or more...

---

Hyphens

***

Asterisks

___

Underscores

</td>
<td width="500px">

```no-highlight
Three or more...

---

Hyphens

***

Asterisks

___

Underscores
```

</td>
</table>


<!-- -------------------------------------------- -->
## Code and Syntax Highlighting

Code blocks are part of the Markdown spec, but syntax highlighting isn't. However, many renderers -- like GitHub's -- support any common programming language.
Here you can find a [list of supported languages](https://github.com/jincheng9/markdown_supported_languages).

<table>
<td width="500px">

We already know that inline code can be created with `single backticks`.
Alternatively you can use the <code>code</code> HTML-tag.

Blocks of code are fenced by lines with three backticks <code>```</code> or the <code>pre</code> HTML-tag.

You select the language to be used for highlighting as shown here:

```
No language indicated, so no syntax highlighting.
But you could explicitly use `no-highlight`
```

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

<pre lang="python">
# we can also use the HTML tag
import antigravity
print("hello world")
</pre>

```html
<title>HTML with syntax highlighting</title>
<p>
  But for HTML, we need to use ```
</p>
```

</td>
<td width="500px">

```
We already know that inline code can be created
with `single backticks`. Alternatively you can use
the <code>code</code> HTML-tag.

Blocks of code are fenced by lines with three
backticks <code>```</code> or the <code>pre</code>
HTML-tag.

You select the language to be used for highlighting
as shown here:
```

<pre>
```
No language indicated, so no syntax highlighting.
But you could explicitly use `no-highlight`
```

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
</pre>

```
<pre lang="python">
# we can also use the HTML tag
import antigravity
print("hello world")
</pre>
```

<pre>
```html
<title>HTML with syntax highlighting</title>
<p>
  But for HTML, we need to use ```
</p>
```
</pre>

</td>
</table>


<!-- -------------------------------------------- -->
## Maths

You can use LaTex syntax to write Maths and equations

<table>
<td width="500px">

You can use it inline with a single `$`: $a=1+2$

Or you can create an equation block with `$$`

$$ f(x) = \sum^\infty_{i=0} \frac{i}{a} + b^2 $$


</td>
<td width="500px">

```no-highlight
You can use it inline with a single `$`: $a=1+2$

Or you can create an equation block with `$$`

$$ f(x) = \sum^\infty_{i=0} \frac{i}{a} + b^2 $$
```

</td>
</table>


<!-- -------------------------------------------- -->
## Blockquotes

<table>
<td width="500px">

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

<blockquote>
  Or you can use HTML for this too
</blockquote>

You can also use this nice trick (but only on GitHub):

![image](https://user-images.githubusercontent.com/62838959/184722977-c6810a5c-f060-4adc-b8de-0716e25ff2a5.png)

</td>
<td width="500px">

```no-highlight
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

<blockquote>
  Or you can use HTML for this too
</blockquote>

You can also use this nice trick (but only on GitHub):

> **Note**
> this is something you should note

> **Warning**
> last warning, your really shouldn't do this!
```

</td>
</table>


<!-- -------------------------------------------- -->
## Lists

<table>
<td width="500px">

1. First ordered list item
2. Another item
    * Unordered sub-list
1. The exact numbers doesn't matter, just that it's a number
    1. Ordered sub-list
4. By the way, you can split you list items
    over multiple lines.
    Simply keep indenting.

* Unordered list can use asterisks
- Or minuses
+ Or pluses

</td>
<td width="500px">

```no-highlight
1. First ordered list item

2. Another item

    * Unordered sub-list

1. The exact numbers doesn't matter, just that it's a number

    1. Ordered sub-list

4. By the way, you can split you list items
    over multiple lines.
    simply keep indenting.


* Unordered list can use asterisks
- Or minuses
+ Or pluses
```

</td>
</table>


<!-- -------------------------------------------- -->
## Definition lists

This is a special type of list that originally comes from `.rst` documents. It's not part of Markdown, but you can use HTML to use them on GitHub.

<table>
<td width="500px">

Definition list are made up of three Tag:

<dl>
  <dt><code>&lt;dl&gt;</code></dt>
  <dd>it wraps the whole list</dd>

  <dt><code>&lt;dt&gt;</code></dt>
  <dd>text or word to define</dd>

  <dt><code>&lt;dd&gt;</code></dt>
  <dd>this containes the actuall definition</dd>

  <dt>Example</dt>
  <dd>This is the text defining it</dd>

</td>
<td width="500px">

```no-highlight
Definition list are made up of three Tag:

<dl>
  <dt><code><dl></code></dt>
  <dd>it wraps the whole list</dd>

  <dt><code><dt></code></dt>
  <dd>text or word to define</dd>

  <dt><code><dd></code></dt>
  <dd>this containes the actuall definition</dd>

  <dt>Example</dt>
  <dd>This is the text defining it</dd>
</dl>
```

</td>
</table>


<!-- -------------------------------------------- -->
## Tables

<table>
<td width="500px">

Colons can be used to align columns.

| Tables        | Are           | Cool |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up
prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
_Still_ | `renders` | **nicely**
1 | 2 | 3

</td>
<td width="500px">

```no-highlight
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make
the raw Markdown line up prettily.
You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
_Still_ | `renders` | **nicely**
1 | 2 | 3
```

</td>
</table>

<!-- -------------------------------------------- -->
## Images

<table>
<td width="500px">

Images are links that are prefixed with a `!` and use an image URL. By default, they use the images original size, but shrink it to fit the page. If you need more control over the size, use HTML.

Inline-style: ![alt text](https://badges.aleen42.com/src/github.svg "Hover Me")

Reference-style: ![alt text][github-badge]

Here HTML can actually benefit you, as it gives more control:

<img src="https://badges.aleen42.com/src/github.svg" width="200x" align="right">

Text next to image

<div align="center">
<img src="https://badges.aleen42.com/src/github.svg" width="60x" height="60px" >
</div>

[github-badge]: https://badges.aleen42.com/src/github.svg "also hover"
[logo]: https://simpleicons.org/icons/markdown.svg "also hover"

</td>
<td width="500px">

```no-highlight
Images are links that are prefixed with a `!` and use an image URL.
By default, they use the images original size, but shrink it to fit
the page. If you need more control over the size, use HTML.

Inline-style:
![alt text](https://badges.aleen42.com/src/github.svg "Hover Me")

Reference-style:
![alt text][github-badge]

Here HTML can actually benefit you, as it gives more control:

<img
  src="https://badges.aleen42.com/src/github.svg"
  width="200px"
  align="right"
/>

Text next to image

<div align="center">
  <img
    src="https://badges.aleen42.com/src/github.svg"
    width="60px"
    height="60px"
  />
</div>

[github-badge]: https://badges.aleen42.com/src/github.svg "also hover"
[logo]: https://simpleicons.org/icons/markdown.svg "also hover"
```

</td>
</table>

---

### Sources and more information

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) by Adam Pritchard  
[HTML Tags You Can Use on GitHub](https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2) by Sean Hammond  
[Guide to aligning images in github readme.md files](https://gist.github.com/DavidWells/7d2e0e1bc78f4ac59a123ddf8b74932d) by David Wells  
