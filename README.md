# bioinfo-agent-skills

Agent skills for plant genomics — one folder per line of work.

Copy a folder from `skills/` into `~/.claude/skills/` or `~/.cursor/skills/`.

| Skill | Line |
|-------|------|
| [plant-omics-db](skills/plant-omics-db/SKILL.md) | Journal-ready plant multi-omics database |
| [grapevine-adna](skills/grapevine-adna/SKILL.md) | Plant aDNA FASTQ→BAM, damage, projection |
| [vitis-te](skills/vitis-te/SKILL.md) | EDTA → curated TE library |
| [vitis-pangenome](skills/vitis-pangenome/SKILL.md) | Graph vs linear ref; PAV; when not to rebuild |
| [vitis-popgen](skills/vitis-popgen/SKILL.md) | Clones, PCA, ADMIXTURE, gene flow |
| [grapevine-chip](skills/grapevine-chip/SKILL.md) | Capture / SNP panel design |
| [drawio-source-redraw](skills/drawio-source-redraw/SKILL.md) | Paper figure → editable draw.io |
| [bioinfo-pitfalls](skills/bioinfo-pitfalls/SKILL.md) | HWE, VCF, aDNA, Slurm traps |

Sister stub repos on the same account (`grapeancestry`, `grapevine-adna`, …) are where code will live. This repo is the agent playbook.

## Install

```bash
git clone https://github.com/Xuzhen-Li/bioinfo-agent-skills.git
cp -R bioinfo-agent-skills/skills/plant-omics-db ~/.cursor/skills/
```

## Topics

`bioinformatics` `plant-genomics` `agent-skills` `ancient-dna` `pangenome` `grapevine`

## License

MIT. Unpublished genotypes and private coordinates do not belong here.

## Author

Xuzhen Li — [ORCID 0000-0003-3670-6657](https://orcid.org/0000-0003-3670-6657)
