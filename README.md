# Awesome-Proteomics-Informatics

## Top Proteomics Informatics Platforms

A curated list of leading software tools for proteomics informatics — covering peptide/protein identification, quantification (DDA, DIA, labeled, label-free), PTM analysis, spectral library search, de novo sequencing, and targeted/untargeted workflows from mass spectrometry data.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[Proteome Discoverer](https://www.thermofisher.com/)** (Thermo Fisher) | Comprehensive, extensible platform for protein identification, quantification (LFQ, isobaric tags), PTM analysis, DIA/DDA, glycoproteomics, cross-linking, and top-down. Integrates multiple search engines (Sequest HT, Mascot, etc.) and advanced rescoring (INFERYS, CHIMERYS). | Full-featured commercial proteomics suite (especially Thermo instruments) |
| **[Spectronaut](https://biognosys.com/)** (Biognosys) | Gold-standard vendor-independent DIA analysis software. Supports library-based and library-free (directDIA) workflows, AI-augmented models, high-throughput quantification, and deep proteome coverage. | DIA proteomics analysis & quantification |
| **[PEAKS Studio](https://www.bioinfor.com/)** (Bioinformatics Solutions) | Complete bottom-up proteomics solution with powerful *de novo* sequencing (DeepNovo), database search, PTM/SPIDER homology, DDA & DIA support, sequence variant analysis, and quantification. Vendor-neutral. | *De novo* + database search & DIA/DDA |
| **[Scaffold](https://www.proteomesoftware.com/)** (Proteome Software) | Industry-standard tools for DDA and DIA validation, visualization, quantitative analysis (labeled/label-free), PTM analysis, and result comparison across search engines. Includes Scaffold DDA, DIA, Q+S, and PTM modules. | Results validation, visualization & quantitation |
| **[ProteinPilot](https://sciex.com/)** (SCIEX) | Protein identification and relative quantification software featuring the Paragon algorithm for extensive PTM and variant searching, plus Pro Group for protein inference. Optimized for SCIEX instruments. | Peptide/protein ID with broad PTM coverage |
| **[MaxQuant](https://www.maxquant.org/)** | Widely used integrated suite for high-resolution quantitative proteomics (free for academic/non-profit). Includes Andromeda search engine, MaxLFQ, SILAC/TMT/iTRAQ support, and MaxDIA. Developed by the Cox lab (Max Planck). | Discovery proteomics quantification (DDA + DIA) |
| **[Byonic](https://www.proteinmetrics.com/)** (Protein Metrics) | Highly sensitive full MS/MS search engine for peptide and protein identification. Strong for glycoproteomics, phosphoproteomics, wide modification searches, and high-throughput workflows. Vendor-neutral. | Sensitive search engine (especially PTMs/glycans) |
| **[Skyline](https://skyline.ms/)** | Freely available, open-source Windows application for targeted quantitative proteomics (SRM/MRM, PRM, DIA/SWATH, MS1 filtering). Excellent method development, visualization, and multi-vendor support. | Targeted & quantitative method development |
| **[Omics Discovery Index (OmicsDI)](https://www.omicsdi.org/)** | Public data discovery portal/index that aggregates proteomics (and other omics) datasets from multiple repositories for search and discovery. | Omics data discovery & indexing |
| **[MS-DIAL](https://prime.psc.riken.jp/compms/msdial/main.html)** | Open-source software originally for metabolomics/lipidomics DIA deconvolution; also used in broader MS data mining including multimodal and lipidome analysis. Supports multiple vendors and advanced structural elucidation. | DIA deconvolution & untargeted MS analysis |

---

## Open-Source Softwares

Proteomics has one of the strongest open-source ecosystems in bioinformatics. Many widely adopted tools are free or fully open-source and often match or exceed commercial performance in specific workflows.

### Core Frameworks & Search / Quantification Engines

| Project | Description | License / Availability | Notes |
|---------|-------------|------------------------|-------|
| **[MaxQuant](https://www.maxquant.org/)** + Andromeda | Integrated suite for peak detection, identification, and quantification (MaxLFQ, SILAC, TMT, label-free, MaxDIA). Extremely popular for high-resolution Orbitrap data. | Free for academic/non-profit use | De facto standard for many discovery workflows |
| **[Skyline](https://skyline.ms/)** | Open-source targeted proteomics platform for method building, data extraction, visualization, and quantification across SRM, PRM, DIA, and MS1. Multi-vendor support. | Apache 2.0 (open source) | Essential for targeted quantitation |
| **[OpenMS](https://www.openms.de/)** | Comprehensive open-source C++ framework and TOPP tools for LC-MS data processing, identification, quantification (label-free, labeled, DIA/SWATH), visualization, and workflow building. | BSD-3-Clause | Full modular pipeline + TOPPView |
| **[FragPipe](https://fragpipe.nesvilab.org/)** + **[MSFragger](https://github.com/Nesvilab/MSFragger)** | Ultra-fast search engine (fragment ion indexing) + complete pipeline for DDA/DIA, open modification searches, quantification (IonQuant), and PTM analysis. | Academic free / open components | Exceptional speed for large datasets & open searches |
| **[DIA-NN](https://github.com/vdemichev/DiaNN)** | High-performance neural network-based DIA analysis tool. Library-free and library-based quantification with excellent depth and accuracy. | Free / open-source components | Leading open DIA competitor to Spectronaut |
| **[MS-DIAL](https://prime.psc.riken.jp/compms/msdial/main.html)** | Open-source DIA MS/MS deconvolution and untargeted analysis platform (strong in metabolomics/lipidomics; also used for broader MS). Multi-vendor support. | Open source | Excellent for DIA deconvolution |
| **[Comet](https://github.com/UWPR/Comet)** | Open-source fork of the classic SEQUEST database search engine. Fast and widely integrated into other pipelines. | Apache 2.0 | Reliable open database search |
| **[X!Tandem](https://www.thegpm.org/tandem/)** | Open-source probabilistic search engine with expectation value scoring. | Open source | Classic community search engine |

### Specialized Libraries & Related Tools

| Project | Description | Focus Area |
|---------|-------------|------------|
| **[ProteoWizard](https://proteowizard.sourceforge.io/)** | Open-source libraries and tools (msconvert, etc.) for reading/writing MS data formats and basic processing. Foundation for many other tools. | Data conversion & access |
| **[Percolator](https://github.com/percolator/percolator)** | Machine-learning post-processor for improving peptide/protein identification confidence (widely integrated). | FDR control & rescoring |
| **[Trans-Proteomic Pipeline (TPP)](http://tools.proteomecenter.org/wiki/index.php?title=Software:TPP)** | Modular open-source pipeline for peptide/protein identification, validation, and quantification. | Standardized open workflow |
| **[PeptideShaker](https://github.com/compomics/peptide-shaker)** | Open-source tool for interpretation and visualization of proteomics identification results. | Results interpretation |
| **[EncyclopeDIA](https://bitbucket.org/searleb/encyclopedia)** | Open-source DIA analysis and spectral library tools. | DIA library search |
| **[AlphaPept / AlphaX ecosystem](https://github.com/MannLabs)** | Modern open-source Python-based proteomics tools from the Mann lab for search, quantification, and downstream analysis. | Next-gen open pipelines |
| **[MZmine](https://github.com/mzmine/mzmine)** | Open-source framework for LC-MS data processing (strong in metabolomics; usable for proteomics feature detection). | Feature detection & processing |

### Additional Notable Open-Source Tools

- **Search engines & adapters** — Sage, Tide/Crux, MS-GF+, MetaMorpheus, and others.
- **Quantification helpers** — MSstats, IonQuant, MaxLFQ implementations, and Python/R packages for downstream stats.
- **Visualization & downstream** — TOPPView (OpenMS), SeeMS, various R/Bioconductor packages (e.g., MSnbase, Proteomics notebooks).
- **Spectral libraries & prediction** — Prosit, MS2PIP, and community library tools.
- **Cross-linking & special workflows** — OpenMS crosslinking tools, xiSEARCH community options, and specialized open packages.
- **Data repositories & discovery** — PRIDE, MassIVE, PeptideAtlas, and OmicsDI (public indexes).

**Note:** Many commercial tools (Proteome Discoverer, Scaffold, Spectronaut) offer excellent usability and vendor-optimized performance. Open-source alternatives (MaxQuant, FragPipe, DIA-NN, OpenMS, Skyline) are production-grade, highly cited, and frequently preferred in academic research for transparency, cost, and cutting-edge algorithms. Hybrid workflows (open search engines + commercial validation/visualization) are very common.

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| High-quality DDA discovery + quantification | **MaxQuant** or **FragPipe/MSFragger** |
| Targeted quantitation (SRM/PRM/DIA) & method building | **Skyline** |
| Fast, deep DIA analysis | **DIA-NN** or **Spectronaut** (commercial) |
| Full modular open pipeline | **OpenMS** |
| *De novo* sequencing + variants | **PEAKS Studio** (commercial) or open *de novo* tools |
| Results validation & visualization | **Scaffold** (commercial) or PeptideShaker + OpenMS |
| Sensitive PTM / glycan searches | **Byonic** (commercial) or FragPipe open searches |
| Multi-vendor data conversion | **ProteoWizard** (msconvert) |
| Untargeted DIA deconvolution | **MS-DIAL** |
| Enterprise Thermo-centric workflows | **Proteome Discoverer** |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context. Proteomics benefits from an exceptionally mature open-source ecosystem (MaxQuant, Skyline, OpenMS, FragPipe, DIA-NN, and others) that powers a large fraction of published research.