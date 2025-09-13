# Bioinformatics Data & Workflow Links

## Data Repositories
| Tool | Domain | Data/Workflow | What You Get | Typical Use |
|------|--------|---------------|--------------|-------------|
| [**GEO (Gene Expression Omnibus)**](https://www.ncbi.nlm.nih.gov/geo/) | Functional Genomics | Data (processed + sometimes raw) | Gene expression matrices (genes × samples) | Reanalyze transcriptomics / microarray datasets |
| [**SRA (Sequence Read Archive)**](https://www.ncbi.nlm.nih.gov/sra) | Raw Sequencing | Data (raw reads) | Unprocessed NGS reads (A/T/G/C) | Run full pipelines (alignment → QC → variant calling) |
| [**PDB (Protein Data Bank)**](https://www.rcsb.org/) | Structural Bioinformatics | Data (3D structures) | Atomic coordinates of proteins (X-ray, cryo-EM, NMR) | Docking, folding, drug design |

---

## Workflow Registries & Pipelines
| Tool | Domain | Data/Workflow | What You Get | Typical Use |
|------|--------|---------------|--------------|-------------|
| [**WorkflowHub**](https://workflowhub.eu/) | General Bioinformatics | Workflow Registry | Catalog of workflows (Nextflow, Snakemake, CWL) | Browse, share, compare reproducible workflows |
| [**nf-core**](https://nf-co.re/) | Genomics & Beyond | Workflow Pipelines | Community-maintained, containerized Nextflow pipelines | Run production-ready pipelines out of the box |

---

## Workflow Frameworks
| Tool | Domain | Data/Workflow | What You Get | Typical Use |
|------|--------|---------------|--------------|-------------|
| [**Nextflow**](https://www.nextflow.io/) | Workflow Execution | Framework | DSL for building scalable, reproducible pipelines | HPC, cloud, nf-core backbone |
| [**Snakemake**](https://snakemake.readthedocs.io/) | Workflow Execution | Framework | Python-based “rule” system (input → output → command) | Lightweight workflows in academic labs |
| [**CWL (Common Workflow Language)**](https://www.commonwl.org/) | Workflow Standard | Framework (specification) | Portable, standardized workflow descriptions | Share workflows across platforms/engines |

---

**Quick Reference**:  
- **GEO / SRA / PDB** → *data you analyze*.  
- **WorkflowHub / nf-core** → *pipelines you run*.  
- **Nextflow / Snakemake / CWL** → *frameworks for building/running pipelines*.
