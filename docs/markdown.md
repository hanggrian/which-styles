---
title: Markdown
nav_order: 3
---

# Markdown
{: .no_toc }

&#8220;Easy reading is damn hard writing.&#8221; &mdash; *Nathaniel Hawthorne*
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Blockquote style

[![Rationale](https://img.shields.io/badge/Pandoc-Block_quotations-080808)](https://pandoc.org/chunkedhtml-demo/8.4-block-quotations.html)

Use **lazy** form, where only the first line is prefixed with a blockquote
character, subsequent lines are prefixed with indentation.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
> Lorem ipsum dolor sit amet,
> consectetur adipiscing elit.
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
> Lorem ipsum dolor sit amet,
  consectetur adipiscing elit.
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Emphasis style

[![Rationale](https://img.shields.io/badge/GitHub-Styling_text-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#styling-text)

Stylize text with **asterisks** while *underscores* act as subsequent
highlights.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
***Lorem ipsum** dolor sit amet,*
consectetur adipiscing elit.
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
_**Lorem ipsum** dolor sit amet,_
consectetur adipiscing elit.
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Fenced code style

[![Rationale](https://img.shields.io/badge/GitHub-Quoting_code-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#quoting-code)

Use **backticks** to create fenced code blocks, not the optional 4 spaces
indentation.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
    git status
    git add
    git commit
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
```
git status
git add
git commit
```
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Header style

[![Rationale](https://img.shields.io/badge/GitHub-Headings-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#headings)

**ATX headings** are preferred over Setext headings. Setext headings are long
and do not support over 2 levels of headings.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
Lorem ipsum
===========
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
# Lorem Ipsum
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Lists

### Unordered list style

[![Rationale](https://img.shields.io/badge/GitHub-Lists-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#lists)

Use **hyphens** to create unordered lists and nested lists. Asterisk is already
associated with highlights, and plus is not as common.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
* Foo
+ Bar
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
- Foo
- Bar
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

### Ordered list style

[![Rationale](https://img.shields.io/badge/Google-Use_lazy_numbering_for_long_lists-4285f4)](https://google.github.io/styleguide/docguide/style.html#use-lazy-numbering-for-long-lists)

Use **fixed numbers** for ordered lists to avoid confusion with nested lists.
There should be four spaces after the period to better align with nested list
items.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
1) Foo
2) Bar
   - Baz
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
1.  Foo
1.  Bar
    - Baz
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Table

### Optional table pipe

[![Rationale](https://img.shields.io/badge/Google-Prefer_lists_to_tables-4285f4)](https://google.github.io/styleguide/docguide/style.html#prefer-lists-to-tables)

**Never** use the optional pipe at each side of the table.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
| Column 1 | Column 2 | Column 3 |
| --- | --- | --- |
| Foo | Bar | Baz |
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
Column 1 | Column 2 | Column 3
--- | --- | ---
Foo | Bar | Baz
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

### Wrap table cell

[![Rationale](https://img.shields.io/badge/GitHub-Creating_a_table-181717)](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables/#creating-a-table)

**Always** wrap the cell content and pad with a space on each end. Column
alignment line should be 3 dashes and optional colon.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
Column 1 | Column 2
:------- | -------:
Foo      | Bar
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
Column 1 | Column 2
:--- | ---:
Foo | Bar
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

## Formatting

### Max line length

[![Rationale](https://img.shields.io/badge/Google-Links-4285f4)](https://github.com/google/styleguide/blob/gh-pages/docguide/style.md#links)

Keep characters in a line to a maximum of **80 characters.**

Separate a link to a new line only if the text (not the link) exceeds 80
characters. In the example below, a paragraph is not split because `[hyperlink]`
can still fit in the first column even though the link is more than 80
characters.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[hyperlink](path/to/hyperlink/).
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. [hyperlink](path/to/hyperlink/).
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>

### Vertical spacing

[![Rationale](https://img.shields.io/badge/Commonmark-Spacing-fff)](https://github.com/style-guides/Markdown/#spacing)

Separate headings, paragraph, and everything in between with **1 blank line.**
Extra lines are ignored when rendered.

<div class="code-example" markdown="1">
  <table>
    <thead>
      <tr>
        <th>Before</th>
        <th>After</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
{% highlight markdown %}
# Heading
Lorem ipsum dolor sit amet.
{% endhighlight %}
        </td>
        <td>
{% highlight markdown %}
# Heading

Lorem ipsum dolor sit amet.
{% endhighlight %}
        </td>
      </tr>
    </tbody>
  </table>
</div>
