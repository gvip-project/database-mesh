# Contributing

This is a pure documentation repository:
Markdown files with Mermaid diagrams, rendered directly by GitHub.
There is no build step.

## Adding a database page

1. Copy [databases/TEMPLATE.md](databases/TEMPLATE.md) to `databases/<kebab-case-name>.md`.
2. Fill in every section.
   If a section genuinely does not apply,
   say so explicitly rather than deleting it,
   so pages stay comparable.
3. Add the database to the index table in [databases/README.md](databases/README.md)
   and to the master graph in the top-level [README.md](README.md).
4. Update the "Ingests from" / "Feeds into" sections of the neighboring database pages,
   and their local mesh diagrams.

## Adding a case study

1. Copy [case-studies/TEMPLATE.md](case-studies/TEMPLATE.md) to
   `case-studies/<identifier-short-slug>.md`
   (for example `cve-2026-50628-cxf.md`).
2. Cite primary sources:
   permalinks to specific commits in record mirrors
   (for example `CVEProject/cvelistV5`, `fkie-cad/nvd-json-data-feeds`,
   `github/advisory-database`)
   are strongly preferred over live URLs,
   because live records change.
3. Add the case study to the index in [case-studies/README.md](case-studies/README.md)
   and link it from the "Known data-quality issues" section
   of each database page it involves.

## Conventions

- Diagrams are Mermaid, kept inline in the Markdown.
  In flow diagrams, an arrow `A --> B` always means *data flows from A into B*;
  label edges with what is transferred, added, or lost.
  Use a dashed arrow (`A -.-> B`) for flows that are partial or unreliable in practice.
- Use [semantic line breaks](https://sembr.org) in Markdown prose:
  one sentence per line,
  with additional breaks at clause boundaries in long sentences.
- Use permalinked sources (commit-pinned URLs)
  for any claim about the historical state of a record.
- Dates are written in ISO format (`2026-06-15`) or spelled out (`June 15, 2026`),
  never ambiguous numeric forms.
