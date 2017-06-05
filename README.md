# markdown-tutorial

- markdown is intended to be as easy-to-read and easy-to-write is feasible.
- readability is emphasized above all else.
- markdown's syntax is comprised entirely of punctuation cahracters.

- markdwon's syntax is intended for one purpose: to be used as a format for writing for the web.

- for any markup that is not covered by markdwon's syntax, you simply use HTML itself. Not need to indicate.
 the only restrictions are that block-level HTML elements. e.g. 
 `<div>,<table>,<pre>,<p>,etc. must be seperated from surrounding content by
 blank lines, and the start and end tags of the block should not be indented wwith tabs or spaces.
 `

 --------
  This is a regular paragraph.

  <table>
    <tr>
        <td>Foo</td>
        <td>Bar</td>
        <td>&Bar</td>
    </tr>
  </table>

  This is another regular paragraph.

---------------------------------

- markdown formating syntax is not processed within block-level HTML tags.

- Span-level HTML tags - e.g. `<span>,<cite>,or <del> can be used anywhere in a markdown paragraph,list item,or header. If you want
 you can even use HTML tags instead of Markdown formatting;`

- unlike block-level HTML tags, Markdown syntax is processed within span-level tags.

## automatic excaping for special characters
- in html, there are two characters that demand special treatment: < and &
    left angle brackets are used to start tags;ampersands are used to denote HTML entities.
    need to escape them when use : \&lt;, and \&amp;
    But in markdown do this.

## block emements
- a paragraph is simply one or more consecutive lines of text, sepratated by one or more blank lines.
  Normal paragraphs should not be indented with spaces or tabs.

- when you do want to insert a \<br /> break tag usering markdown,end a line with two or more spaces, then type retrun

- Headers.
```
# H1
## H2
### H3
```

## blockquotes
- markdown use email-stype > characters to blockquoting.


> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.


- blockquotes can be nested.
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.


- Blockquotes can contain other Markdown elements, including headers, lists, and code blocks:

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> Here's some example code:
>
>      return shell_exec("echo $input | $markdown_script");


### Lists
- markdown support ordered and unordered lists

*   Red
*   Green
*   Blue

-   Red
-   Green
-   Blue


Ordered lists use numbers followed by periods:

1.  Bird
2.  McHale
3.  Parish


1.  Bird
1.  McHale
1.  Parish

<ol>
<li>Bird</li>
<li>McHale</li>
<li>Parish</li>
</ol>

- list markers typically start at the left margin,but may be indented by up to three spaces.
 list markers must followed by one or more spaces or a tab.

*   Bird
*   Magic

<ul>
<li>Bird</li>
<li>Magic</li>
</ul>


-----------------

*   Bird

*   Magic
--------------

<ul>
<li><p>Bird</p></li>
<li><p>Magic</p></li>
</ul>

- list items may consist of multiple paragraphs.Each subsequent paragraph in a
    list item must be idented by either 4 spaces or one tab:

- to put a code bolck within a list item, the code block needs to be indented twice - 8 spaces ro two tabs:

* A list itme with a code block:

        <code goes here>


### code blocks
- markdown wraps a code block in both <pre> and <code> tags.
to produce a code block in markdown,simply indent every line of th eblock by at least r spaces or 1 tab.

this is a normal paragraph:

    This is a code block.


### horizontal rules

* * *

### span elements

- markdown supports two style of links :inline and reference.
in both styles,the link text is delimited by [square brackets]

This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.

- use relative paths:

    See my [About](/about/) page for details. 

- reference-style links use a second set of square brackets, inside which you  place a label of your choosing to identify the link.

This is [an example][id] reference-style link.

[id]: http://example.com/  "Optional Title Here"


Use the `printf()` function

To include a literal backtick character within a code span, you can use multiple backticks as the opening and closing delimiters:

``There is a literal backtick (`) here.``
