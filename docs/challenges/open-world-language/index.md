# Challenge: Open World Language


## Description

Given a set of properties, the a Language Concern offers an open world
assumption if some part of the specification are left voluntarily unspecified
and left to be specified by future Languages.

## Example

An expression language could be defined by only specifying the types of
supported operations (`+`, `-`, `sqrt`...) but not the type of the literals it
can be applied on.

### BNF

```
Plus extends Value: Value '+' Value
Minus extends Value: Value '-' Value
Sqrt extends Value: 'sqrt' '(' Value ')'
abstract Lit extends Value
```

At this point, Lit is left unspecified and must be specified later to form a
fully specified language.
