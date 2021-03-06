---
title: "Scheme Interpreter"
date: 2019-11-19T10:07:47+06:00
draft: false

# post thumb
image: "images/scheme.jpeg"

# meta description
description: "CS61A Scheme Project"
summary: "Python interpreter for the Scheme programming language."
author: "Jeffrey Sung"

# taxonomies
categories: 
  - "Structure and Interpretation of Computer Programs"
tags:
  - "Python"

# post type
type: "post"
---

### Interpreter Features
**Read-Eval-Print.** The interpreter reads Scheme expressions, evaluates them, and displays the results.
```
scm> 2
2
scm> (+ 2 3)
5
scm> (((lambda (f) (lambda (x) (f f x)))
       (lambda (f k) (if (zero? k) 1 (* k (f f (- k 1)))))) 5)
120
```
{{< rawhtml >}}<br/><br/>{{< /rawhtml >}}
**Load.** The load procedure differs from standard Scheme in that it uses a symbol for the file name. For example, to load tests.scm, evaluate the following call expression.
```
scm> (load 'tests)
```
{{< rawhtml >}}<br/><br/>{{< /rawhtml >}}
**Symbols.** Rule for identifiers:
{{< rawhtml >}}
<p><blockquote>An identifier is a sequence of letters (a-z and A-Z), digits, and characters in <code>!$%&*/:<=>?@^_~-+.</code> that do not form a valid integer or floating-point numeral.</blockquote></p>
{{< /rawhtml >}}
The version of Scheme used is case-insensitive: two identifiers are considered identical if they match except possibly in the capitalization of letters. They are internally represented and printed in lower case:
```
scm> 'Hello
hello
```