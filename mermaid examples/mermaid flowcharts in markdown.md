# This documents something

See [this link](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/) for more information how to create mermaid graphs directly in markdown.

## Example mermaid figure

See source code of this document for the syntax.

```mermaid
flowchart TD
    A[Use Github\nsearch function] -->B{Found\nsolution?}
    B -->|Yes|C(Consider improving\nthe documentation)
    B -->|No|D(Create Github issue\nrequesting help)
    D -->E{Solved with new\ndocumentation?}
    E -->|Yes|C
    E -->|No|D
```