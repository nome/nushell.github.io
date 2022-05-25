---
title: str title-case
layout: command
version: 0.63.0
usage: |
  Convert a string to Title Case
---

# `{{ $frontmatter.title }}`

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> str title-case ...rest```

## Parameters

 -  `...rest`: optionally convert text to Title Case by column paths

## Examples

convert a string to Title Case
```shell
> 'nu-shell' | str title-case
```

convert a string to Title Case
```shell
> 'this is a test case' | str title-case
```

convert a column from a table to Title Case
```shell
> [[title, count]; ['nu test', 100]] | str title-case title
```