# Markdown Style

## Elements

### Headings: ATX

[![Rationale](https://img.shields.io/badge/GitHub-Headings-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#headings)

**ATX headings `#`, `##`, `###`, `####`, `#####`, and `######`** are preferred
over Setext headings. Setext headings are long and do not support over 2 levels
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

### Emphasis: Asterisk

[![Rationale](https://img.shields.io/badge/GitHub-Styling_text-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#styling-text)

**Use `*` and `**`** to highlight text. The optional symbols `_` and `__` can as
a subsequent highlighter.

**Before**

```md
***Lorem ipsum** dolor sit amet,* consectetur adipiscing elit.
```

**After**

```md
_**Lorem ipsum** dolor sit amet,_ consectetur adipiscing elit.
```

### Blockquote: Lazy

[![Rationale](https://img.shields.io/badge/Pandoc-Block_quotations-080808)](https://pandoc.org/chunkedhtml-demo/8.4-block-quotations.html)

**Use single `>`** to create blockquotes, not the subsequent lines. However,
list items and tables rows are exceptions.

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

### Fenced code: Backticks

[![Rationale](https://img.shields.io/badge/GitHub-Quoting_code-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#quoting-code)

**Use backticks ` ``` `** to create fenced code blocks, not the optional 4
spaces indentation.

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

### Lists

[![Rationale](https://img.shields.io/badge/GitHub-Lists-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#lists)

#### Unordered list: Hyphen

**Use hyphens `-`** to create unordered lists and nested lists. Asterisk is
already associated with highlights, and plus is not as common.

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

#### Ordered list: Period

**Use period `.`** and growing numbers to create ordered lists.

```md
1) Foo
1) Bar
```

**After**

```md
1. Foo
2. Bar
```

### Table

[![Rationale](https://img.shields.io/badge/GitHub-Creating_a_table-181717)](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables/#creating-a-table)

#### Table cell: Wrap

Always wrap the cell content and **pad with a space on each end**. Column
alignment line should be **3 dashes** and optional colon `:`.

**Before**

```md
| Column 1 | Column 2 |
| :------- | -------: |
| Foo      | Bar      |
```

**After**

```md
| Column 1 | Column 2 |
| :--- | ---: |
| Foo | Bar |
```

#### Table borders: Always

Use pipes `|` at each end of the cell for readability. When word wrapping is
enabled, it is difficult to see which cell belong to which row without the
pipes.

**Before**

```md
Column 1 | Column 2 | Column 3
--- | --- | ---
Foo | Bar | Baz
```

**After**

```md
| Column 1 | Column 2 | Column 3 |
| --- | --- | --- |
| Foo | Bar | Baz |
```

## Formatting

### Line length: 80

[![Rationale](https://img.shields.io/badge/Google-Links-4285F4)](https://github.com/google/styleguide/blob/gh-pages/docguide/style.md#links)

Keep characters in a line to a maximum of **80 characters.**

Separate a link to a new line **only if the text (not the link)** exceeds 80
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

[![Rationale](https://img.shields.io/badge/Commonmark-Spacing-fff)](https://github.com/style-guides/Markdown/#spacing)

Separate headings, paragraph, and everything in between with **1 blank line**.
Extra lines are ignored when rendered.

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

### Indentation: Variable

[![Rationale](https://img.shields.io/badge/GitHub-Nested_lists-181717)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax/#nested-lists)

Do not use fixed indentation, **align the content** with the previous line.

**Before**

```md
1. Foo
  - Bar

> Foo
>> Bar
```

**After**

```md
1. Foo
   - Bar

> Foo
> > Bar
```
