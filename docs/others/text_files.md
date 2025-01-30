---
title: Text files
parent: Others
nav_order: 3
---

# Text files
{: .no_toc }

&#8220;I always wanted to be somebody, but now I realize I should have been more
specific.&#8221; &mdash; *Lily Tomlin*
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Insert final newline

[![Rationale](https://img.shields.io/badge/POSIX-Line-fff)](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_206)

**Always** end a file with a newline character, a common practice in Unix
systems.

{% highlight plaintext %}
Lorem ipsum.

{% endhighlight %}

## Trim trailing whitespace

[![Rationale](https://img.shields.io/badge/Commonmark-Hard_line_breaks-fff)](https://spec.commonmark.org/0.20/#hard-line-breaks)

**Never** put trailing whitespace at the end of a line.

{% highlight plaintext %}
Lorem ipsum.↵
{% endhighlight %}
