# Case studies

Concrete examples of a vulnerability record traveling through the mesh,
documenting where and how the data degraded.
Each case study follows [TEMPLATE.md](TEMPLATE.md)
and cites commit-pinned permalinks
so the historical record states stay verifiable.

| Case study | Summary |
|---|---|
| [CVE-2026-50628 (Apache CXF)](cve-2026-50628-cxf.md) | A CVSS 9.8 issue in a single Maven artifact: correct at MITRE, over-broad CPE at NVD, empty stub at GitHub, missing at GitLab, diluted at OSV |
| [CVE-2026-109618/109619 (PHP2Shell)](cve-2026-109618-php2shell.md) | Twin KEV-listed PHP records followed field by field: NVD widens ranges, splits CVSS and adds uncited PAN-OS CPEs; no GitHub advisory; OSV inherits NVD's ranges |

To add a case study,
see [CONTRIBUTING.md](../CONTRIBUTING.md).
