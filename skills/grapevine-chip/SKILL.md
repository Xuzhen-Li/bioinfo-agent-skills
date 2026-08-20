---
name: grapevine-chip
description: >
  Design and QC a grapevine SNP / capture panel. Use when choosing sites,
  designing probes, or validating a capture chip. Downstream ancestry
  of called VCFs belongs to grapeancestry, not this skill.
---

# grapevine-chip

Site choice is the science. Probe chemistry is secondary.

## Order

```
Question (ancestry / GWAS / ID)
  → VCF QC
  → LD prune
  → windows
  → MAF / informativeness rank inside each window
  → pick sites
  → probe design (flank, Tm, off-target)
  → wet QC
  → call and validate vs WGS
  → hand the VCF to grapeancestry / vitis-popgen
```

## Red lines

- Do not design a panel before the scientific job is one sentence.
- Do not dump a whole-genome VCF onto a chip without LD and windowing.
- Keep design (this skill) separate from sample calling (`grapeancestry`).
- No unpublished sample-level genotypes in the public repo.

## Split

| Repo / skill | Job |
|--------------|-----|
| `grapevine-chip` | pick sites and probes |
| `grapeancestry` | FASTQ → panel VCF → ancestry report |

Related: `vitis-popgen`, `vitis-pangenome`.
