# Challenge: One Level Extension

## Description

Starting from a [Language Concern](../../benchmark/vocabulary.md#language-concern)
*A*, a language *B* is defined by extending *A*.


![One Level Extension Schema](./one-level-extension.svg)

### Concrete example

An expression language is reused to define a
[Logo](https://en.wikipedia.org/wiki/Logo_%28programming_language%29) language.

## Variants \#1

*B* is defined using *A*'s notation, but does not reuse it, consequently *A* is
only used as a facility to write implement the semantics of *B*.

![One Level Extension Schema - Variant 1](./one-level-extension-variant1.svg)

### Concrete example

An [Petri Net](https://en.wikipedia.org/wiki/Petri_net) language is used to
define the semantics of a
[Finite State Machine](https://en.wikipedia.org/wiki/Finite-state_machine)
language
