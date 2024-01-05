# Experimenting with github as a knowledge base

Includes:

* Longer documentation as regular files
* Smaller bits of information as a wiki
* Issues to track IT support operation tasks
* Projects to plan longer tasks
* Documentation changes can be reviewed by pull requests

Consider using webhooks to get changes of the Github repo as a notification in Teams.

## How to find information
```mermaid
flowchart LR
    A[Use Github\nsearch function] -->B{Found\nsolution?}
    B -->|Yes|C(Consider improving\nthe documentation)
    B -->|No|D(Create Github issue\nrequesting documentation)
    D -->E{Solved with \n new doc?}
    E -->|Yes|C
    E -->|No|D
```

## How to contribute

```mermaid
flowchart TD
    A{Topic\nsize} -->|small| B(Wiki entry)
    A -->|medium| C(Markdown page)
    A -->|complex| D(AsciiDoc page)
```

Everything here is text-based to make everything easily searchable. Therefore, all documents are either Markdown (.md, preferred, simple) or AsciiDoc (.adoc, for special cases, more powerful) to let you focus on content rather than formatting.

Additionally, all wiki entries are (under the hood) just Markdown files, so the same source code formatting applies.

|                     | Wiki entry           | Markdown (.md) page | AsciiDoc (.adoc) page  |
|---------------------|----------------------|---------------------|------------------------|
| **power**           | very simple          | medium              | powerful               |
| **features**        | copy/paste pictures  | simple syntax       | create HTML/PDFs/Books |
| **github tooling**  | great                | none                | none                   |
| **PyCharm tooling** | n/a                  | ok                  | good                   |
| **version control** | only commit messages | version controlled  | version controlled     |


Irrespective of what you use to document your information, this has a couple of advantages:

* Everything is easily searchable
* Graphs can be included in text-based form (mermaid) making them searchable, version-controllable, and easily editable without special tools
* All changes are easily trackable and reversible with commits and pull requests. Old document versions can also be searched
* All text and even figure components can be referenced with permalinks in issues and other documents
* Since all IT support issues are also on Github, they can directly and easily reference to all documents and their specific lines




