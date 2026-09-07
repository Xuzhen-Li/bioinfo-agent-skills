---
name: grapevine-chip
description: >
  Design and QC a grapevine SNP / capture panel. Use when choosing sites,
  designing probes, or validating a capture chip. Canonical notes live in
  grapeancestry/chip — this stub only keeps old Cursor installs working.
---

# grapevine-chip (moved)

**Canonical home:** [grapeancestry/chip](https://github.com/Xuzhen-Li/grapeancestry/tree/main/chip)

Site choice is the science. Probe chemistry is secondary. Downstream ancestry
of called VCFs belongs to `grapeancestry` analysis, not a separate public grain.

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
  → hand the VCF to grapeancestry analysis /
    vitis-popgen
```

## Red lines

- Do not design a panel before the scientific job is one sentence.
- Do not dump a whole-genome VCF onto a chip without LD and windowing.
- Keep design (`grapeancestry/chip`) separate from sample calling (`grapeancestry/analysis`).
- No unpublished sample-level genotypes in the public repo.

## Split

| Path | Job |
|------|-----|
| `grapeancestry/chip` | pick sites and probes |
| `grapeancestry/analysis` | FASTQ → panel VCF → ancestry report |
| `grapevine-chip` repo | redirect shell for old links only |
