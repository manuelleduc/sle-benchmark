# Xbase Analysis


## Introduction
Xbase is an reusable expression language developed using Xtext.

It is developed modularly, it the goal to be embedded in heterogeneous
Domain Specific Languages.

![Xbase Hierarchy](./hierarchy.png)


Many languages have been developed using Xbase, among them, [seven demonstrating
language](https://github.com/xtext/seven-languages-xtext/) have been developed
by the Xtext development team:  **Scripting**, **Build**, **MongoDB**,
**Guice**, **Http Rounting**, **Template**, and **Tortoise**.

They offers a diversity of cases of reuse of xbase in application domains
described in the [documentation](https://github.com/xtext/seven-languages-xtext/tree/master/documentation).


## Observations

By applying a dead code analysis of the dependencies between the Xtext
languages hierarchy and the dependencies between the ecore files of the
languages syntax, similar to the
[dead feature detection](../challenges/dead-features-detection) challenge,
we found out that some parts of Xtype are never used when the production rule
`XImportSection` is not used in the language grammar.

![unused imports](./unused-imports.png)


Consequently, we see this as a missed opportunity to modularize the xbase
infrastructure even more.

## Experience: Extracting the import

### Technical details

Extracting the import means moving the following xtext and xbase entities out
of the xbase in their own xtext and ecore files.

- xtext
  - XImportSection
  - XImportDeclaration
  - QualifiedNameWithWildcard
  - QualifiedNameInStaticImport
- xbase
  - XImportSection
  - XImportDeclaration
