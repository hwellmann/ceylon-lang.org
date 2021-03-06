---
layout: reference
title_md: '`<` (less than) operator'
tab: documentation
unique_id: docspage
author: Tom Bentley
doc_root: ../../..
---

# #{page.title_md}

The non-associating, binary infix `<` operator is used to test whether its left-hand 
operand is *less than* its right-hand operand.

## Usage 

<!-- try: -->
    void m<T>(T x, T y) 
      given T satisfies Comparable<T> {
        Boolean less = x < y;
    }

## Description

### Definition

The `<` operator is defined as follows:

<!-- check:none -->
<!-- try: -->
    lhs.compare(rhs)==smaller;

See the [language specification](#{site.urls.spec_current}#equalitycomparison) for more details.

### Polymorphism

The `<` operator is [polymorphic](#{page.doc_root}/reference/operator/operator-polymorphism). 
The meaning of `<` depends on the 
[`Comparable`](#{site.urls.apidoc_current}/Comparable.type.html) interface. 

### Type

The result type of the `<` operator is [`Boolean`](#{site.urls.apidoc_current}/Boolean.type.html).

## See also

* API documentation for [`Comparable`](#{site.urls.apidoc_current}/Comparable.type.html)
* [`<` in the language specification](#{site.urls.spec_current}#equalitycomparison)
* [operator precedence](#{site.urls.spec_current}#operatorprecedence) in the 
  language specification
* [Operator polymorphism](#{page.doc_root}/tour/language-module/#operator_polymorphism) 
  in the Tour of Ceylon

