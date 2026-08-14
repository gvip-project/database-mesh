# Databases

One page per database,
all following [TEMPLATE.md](TEMPLATE.md) so they stay comparable.
See the top-level [README](../README.md)
for the master graph of how they interact.

| Database | Operator | Identifier | Format | Role in the mesh | Page |
|---|---|---|---|---|---|
| MITRE CVE List | MITRE (CVE Program) | `CVE-YYYY-NNNNN` | CVE JSON 5.x | Canonical record registry | [mitre-cve.md](mitre-cve.md) |
| NVD | NIST | CVE IDs | NVD API 2.0 JSON, CPE 2.3 | Enrichment (CPE, CWE) | [nvd.md](nvd.md) |
| GitHub Advisory Database | GitHub | `GHSA-xxxx-xxxx-xxxx` | OSV schema | Enrichment (reviewed) and NVD mirror (unreviewed); also a CNA | [github-advisories.md](github-advisories.md) |
| OSV.dev | Google / OpenSSF | source-native + CVE | OSV schema | Package-first aggregator | [osv.md](osv.md) |
| GitLab Advisory Database | GitLab | per-package paths | custom YAML | Curated aggregator for GitLab scanning | [gitlab-advisory-database.md](gitlab-advisory-database.md) |
| CISA KEV | CISA | CVE IDs | fixed JSON/CSV schema | Curated exploited-in-the-wild subset | [cisa-kev.md](cisa-kev.md) |
| ENISA EUVD | ENISA | `EUVD-YYYY-NNNNN` | custom JSON | EU aggregator and disclosure channel; also a CNA | [euvd.md](euvd.md) |
| VulnerableCode | AboutCode / nexB | `VCID`, PURL-keyed | relational / REST | Open cross-source aggregator | [vulnerablecode.md](vulnerablecode.md) |

Not yet covered by dedicated pages, but referenced:
the CISA ADP ("Vulnrichment", the SSVC/KEV/CVSS enrichment container on CVE records),
ecosystem databases feeding OSV.dev
(PyPA advisory-db, RustSec, Go vulnerability database),
Linux distribution trackers
(Debian, Red Hat, SUSE, Alpine),
and national databases such as JVN or CNNVD.
Contributions welcome,
see [CONTRIBUTING.md](../CONTRIBUTING.md).
