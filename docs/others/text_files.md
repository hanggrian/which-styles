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

<a
  class="label label-posix"
  href="https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_206">
  POSIX: Line
</a>

**Always** end a file with a newline character, a common practice in Unix
systems.

{% highlight plaintext %}
Lorem ipsum.

{% endhighlight %}

## Trim trailing whitespace

<a
  class="label label-commonmark"
  href="https://spec.commonmark.org/0.20/#hard-line-breaks">
  CommonMark: Hard line breaks
</a>

**Never** put trailing whitespace at the end of a line.

{% highlight plaintext %}
Lorem ipsum.↵
{% endhighlight %}
