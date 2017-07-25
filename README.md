# Blockdown

Blockdown is an extension of [Markdown](https://help.github.com/articles/about-writing-and-formatting-on-github/) that enables the creation of feature-rich content with a powerful templating system.

- Lunr search
- Default Bootstrap template
- Highlight.js syntax highlighting
- Github Flavored Markdown
- Nunjucks tempting 

## Install

```
npm install -g
```

## Blockdown documents

A Blockdown document is a collection of blocks separated by three dashes `---`. The dash pattern must have its own line to separate blocks from each other.

```
first block
---
second block
---

third block

---


fourth block
... and so on ...
```

## Blocks

A block can begin with any number of `@key value` pairs. The key can be any valid JavaScript key, and the value must be a JSON formatted value like `42` or `"literal string"`. Since the value is consumed with `JSON.parse`, you can provide any valid JSON as the value for the key.

```
@title "Getting Started"
@template "get-started"
@length 10

This is how you get started, it should take around ten minutes.
- do this
- then this
- and finally this

---
@title "Write Something!"
@length 15
@standard ["CCSS.MATH.CONTENT.8.NS.A.1", "K12CS.K–2.Impacts of Computing.Social Interactions"]

This content aligns with standards, and the templating engine will help me link to them.

---

This is just *markdown with no key-value pairs*.

[link to something](https://anything.com)

> This is a block quote

```

## Layout



## Templates

Templates are rendered with nunjucks

## 
