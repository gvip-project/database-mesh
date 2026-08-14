# <Database name>

<One-paragraph description: what this database is, who runs it, and its role in the mesh.>

## At a glance

|                       |                                                   |
|-----------------------|---------------------------------------------------|
| **Operator**          | <organization>                                    |
| **URL**               | <main website>                                    |
| **Identifier scheme** | <CVE-YYYY-NNNNN, GHSA-xxxx-xxxx-xxxx, ...>        |
| **Data format**       | <CVE JSON 5.x, OSV schema, custom YAML, ...>      |
| **Data license**      | <license of the published data>                   |
| **Access**            | <API endpoints, git repositories, bulk downloads> |

## Scope

<What the database covers: all software, open-source packages only, a curated subset,
a specific ecosystem, a jurisdiction, ...>

## Ingests from

- [<Database>](<page>.md): <what is ingested and how (API pull, git sync, manual)>

## Feeds into

- [<Database>](<page>.md): <what is consumed downstream>

## Local mesh

```mermaid
flowchart LR
    UP["<upstream>"] -- "<what flows>" --> THIS["<this database>"]
    THIS -- "<what flows>" --> DOWN["<downstream>"]
```

## Enrichment performed

<What this database adds to records beyond what it ingests: scores, product identifiers,
affected ranges, exploitation status, review, ...>

## Known data-quality issues

<Systematic problems observed in this database's data:
staleness, over-broad or missing product identifiers, empty stubs,
propagation of upstream errors, ...
Link case studies.>

- <issue>. See [case study](../case-studies/<file>.md).
