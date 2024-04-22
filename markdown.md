# Markdown style

### Blockquote style: Lazy

Use single greater-than `>` to create blockquotes, not the subsequent lines.
However, list items and tables rows are exceptions.

**Before**

```md
> Lorem ipsum dolor sit amet,
> consectetur adipiscing elit.
```

**After**

```md
> Lorem ipsum dolor sit amet,
  consectetur adipiscing elit.
```

### Emphasis style: Asterisk

Stylize text with asterisks `*` and `**`. The underscores `_` and `__` can as a
subsequent highlighter.

**Before**

```md
***Lorem ipsum** dolor sit amet,* consectetur adipiscing elit.
```

**After**

```md
_**Lorem ipsum** dolor sit amet,_ consectetur adipiscing elit.
```

### Fenced code style: Backticks

Use backticks ` ``` ` to create fenced code blocks, not the optional 4 spaces
indentation.

**Before**

```md
    git status
    git add
    git commit
```

**After**

```md
´´´
git status
git add
git commit
´´´
```

### Header style: ATX

ATX headings `#`, `##`, `###`, `####`, `#####`, and `######` are preferred over
Setext headings. Setext headings are long and do not support over 2 levels
of headings.

**Before**

```md
Lorem ipsum
===========
```

**After**

```md
# Lorem Ipsum
```

## Lists

### Unordered list style: Hyphen

Use hyphens `-` to create unordered lists and nested lists. Asterisk is already
associated with highlights, and plus is not as common.

**Before**

```md
* Foo
+ Bar
```

**After**

```md
- Foo
- Bar
```

### Ordered list style: Lazy

Use fixed `1.` instead of growing numbers to create ordered lists. There should
be two spaces after the period to better align with nested list items.

```md
1) Foo
2) Bar
   - Baz
```

**After**

```md
1.  Foo
1.  Bar
    - Baz
```

## Table

### Optional table pipe: Never

Do not use the optional pipe `|` at the beginning and end of the table.

**Before**

```md
| Column 1 | Column 2 | Column 3 |
| --- | --- | --- |
| Foo | Bar | Baz |
```

**After**

```md
Column 1 | Column 2 | Column 3
--- | --- | ---
Foo | Bar | Baz
```

### Wrap table cell: Always

Always wrap the cell content and pad with a space on each end. Column alignment
line should be 3 dashes and optional colon `:`.

**Before**

```md
Column 1 | Column 2
:------- | -------:
Foo      | Bar
```

**After**

```md
Column 1 | Column 2
:--- | ---:
Foo | Bar
```

## Formatting

### Max line length: 80

Keep characters in a line to a maximum of 80 characters.

Separate a link to a new line only if the text (not the link) exceeds 80
characters. In the example below, a paragraph is not split because `[hyperlink]`
can still fit in the first column even though the link is more than 80
characters.

**Before**

```md
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[hyperlink](path/to/hyperlink/).
```

**After**

```md
Lorem ipsum dolor sit amet, consectetur adipiscing elit. [hyperlink](path/to/hyperlink/).
```

### Vertical spacing: 1

Separate headings, paragraph, and everything in between with 1 blank line. Extra
lines are ignored when rendered.

**Before**

```md
# Heading
Lorem ipsum dolor sit amet.
```

**After**

```md
# Heading

Lorem ipsum dolor sit amet.
```
