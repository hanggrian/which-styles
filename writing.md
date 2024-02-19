# Writing Style

## Capitalization

[![Rationale](https://img.shields.io/badge/APA-Title_case_capitalization-000)](https://github.com/style-guides/Markdown/#spelling)

### Title-case: Document title & figure title

Capitalize **first letter of each word** for titles of documents, tables, and
figures.

**Before**

```md
# Lorem ipsum

![Figure 1](path/to/figure)<br><small>Figure 1 &ndash; use-case diagram</small>
```

**After**

```md
# Lorem Ipsum

![Figure 1](path/to/figure)<br><small>Figure 1 &ndash; Use-case Diagram</small>
```

### Sentence-case: Subtitle & table headings

Capitalize **first letter of the first word** for everything else.

**Before**

```md
lorem ipsum dolor sit amet, consectetur adipiscing elit.

| Foo Bar | Baz Qux |
| --- | --- |
| ... | ... |
```

**After**

```md
Lorem ipsum dolor sit amet, consectetur adipiscing elit.

| Foo bar | Baz qux |
| --- | --- |
| ... | ... |
```

## Punctuation

[![Rationale](https://img.shields.io/badge/AP-Punctuation-eb483b)](https://libguides.csusb.edu/APstylebook/punctuation/)

### Serial comma: Never

Serial comma **is not placed** after the penultimate term. Exceptionally, comma
can be placed when combining two separate contexts.

**Before**

```md
Science, math, and reading, and writing.

I was breastfed but my family members were fed formula.
```

**After**

```md
Science, math, and reading and writing.

I was breastfed, but my family members were fed formula.
```

### Emphasize punctuation: Always

When highlighting a word or phrase with adjacent punctuations, **also highlight
the punctuations.**

**Before**

```md
**Lorem ipsum**, dolor sit amet.
```

**After**

```md
**Lorem ipsum,** dolor sit amet.
```

### Punctuate list item: Sentence-only

Punctuate list items with a period **only if** they are complete sentences.

**Before**

```md
- Lorem ipsum, dolor sit amet
- Consectetur adipiscing elit

1. Foo.
2. Bar.
```

**After**

```md
- Lorem ipsum, dolor sit amet.
- Consectetur adipiscing elit.

1. Foo
2. Bar
```
