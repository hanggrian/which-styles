---
title: File names
parent: Others
nav_order: 1
---

# File names
{: .no_toc }

&#8220;If you think your boss is stupid, remember: You wouldn&#8217;t have a job
if he was any smarter.&#8221; &mdash; *John Gotti*
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Extension letter

[![Rationale](https://img.shields.io/badge/Google-Extensions-4285f4)](https://developers.google.com/style/filenames/#file-type-names)

Refer to file type names as *uppercase,* but use **lowercase** for file
extensions.

Use full form file extensions (e.g.: `.jpeg` over `.jpg`), unless modified by a
specific platform or tool.

{% highlight plaintext %}
Check out our company profile in the attached PDF file.

Attachment: company_profile.pdf
{% endhighlight %}

## Separate indices

![Rationale](https://img.shields.io/badge/Personal-gray)

When referencing a series of files, use a combination of the filename and index
**without a separator.**

{% highlight plaintext %}
├ links
│ ├ graph1_1.svg
│ ├ graph1_2.svg
│ └ graph1_1_1.svg
├ blog1.md
└ blog1_1.md
{% endhighlight %}

## Whitespace symbol

[![Rationale](https://img.shields.io/badge/Google-Filenames-4285f4)](https://developers.google.com/style/filenames/#exceptions-for-consistency)

Use an **underscore** to separate words in a file name. Although hypens are more
common, it is sometimes used to denote a range of values in a file name.

This rule can be ignored if a specific platform or tool already has a naming
convention.

{% highlight plaintext %}
├ avoiding_cliches.jd
└ quick_lesson1-4.md
{% endhighlight %}
