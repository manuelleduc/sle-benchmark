# Vocabulary

## Language

A Language is a specific kind of language concern where there is no more
variability and no more customization to be done.
For instance, if the Expression language concern is configured by selecting
Literal and Arithmetic Operation (but not Variable and Comparison Operation) and
customized by defining the Literal as Double values, and nothing is left in the
variation interface and customization interface, then the result is a specific
Expression Language, i.e, one among all the potential Expression Languages
derivable from the Expression Language Concern.

## Language Concern

A Language Concern is a configurable unit of reuse that encapsulates a specific
user-visible set of constructs of a language (such as support for expressions,
support for exceptions, units, uncertainty management, etc.).
A Language Concern may reuse other Language Concerns.
A Language Concern encompasses the definition of the expected constituents among
abstract syntax, concrete syntax and behavioral semantics.
Those constituents are concretized in various artifacts (e.g., Ecore metamodels,
BNF grammars, OCL constraints, ATL model transformations, Java visitors,etc.).
Artifacts are organized in facets that correspond to the perspectives (e.g.,
domain model, graphical concrete syntax, context conditions, interpreter,
compiler, etc.) of a specific language workbench.
Language Concern reuse is achieved thanks to three interfaces: A variation
interface expressing variabilities in the Language Concern in terms of features
from which a user, i.e., a language engineer, can select his desired
configuration; a customization interface allowing to integrate a Language
Concern into another language or Language Concern; and a usage interface
exposing the relevant information needed to use the functionality that a concern
provides to a language or another Language Concern. Section 2.3 introduced two
examples of Language Concerns (Expression and Unit).


## Artifact

## Facet
