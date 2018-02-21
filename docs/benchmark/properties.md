# Properties

## Functional Properties

- **reusability:** can we quantify how much a define Language is reusable as a building block of future languages?
- **model compatibility:** does it exist a notion of language typing. Does the model produced defined using a Language *A* be executable using a Language *B* with a children type relationship to *A*.
- **independent compilation:** does the compilation of a language requires the compilation of its dependencies.
- **interface isolation/information hidding:** can the compilation of a language be done by consulting only the interfaces informations of its dependencies.
- **anticipation:** does the specification of a language concern be done without have to adapt the implementation specifically to address implementation concerns of the languages that depends on it?

## Non Functional Properties

All of the following properties can be asked in term of comparison to a
functionally equivalent language developed monolithically instead of modularly.

- **compilation speed:** how long does it takes to compile a language. Does it vary according to the size of its own specification. Of the size of the specification of its dependencies? This property is linked to the **independent compilation** functional property.
- **execution speed:** What is the cost of the modularity in term of execution speed. Does it vary according to the number of transitive dependencies?


## Reusability scope

What is the scope covered by the reuse operations of the language workbench?
The set of minimal identified feature of a language workbench are listed in
the [workbenches](../index/workbenches#identified-language-workbenches-features) page.

It is neither realistic nor required to let every aspect of a Language definition
be defined modularly with reuse in mind. Yet, it is important for the language
designer to know what is expected to be reusable when choosing a language
concern to address part of the implementation of a language.


# To be defined

- Can the language concern be distributed as an well identified set of black-box software artifacts (e.g. maven artifacts)?
