---
title: "DNA-Protein Interactions"
subtitle: "Systematic classification of DNA-binding proteins"
summary: "Comprehensive overview of protein families that interact with DNA, organized by structure, enzymatic function, and regulatory roles"
date: 2025-01-24
type: widget_page
headless: false
---

{{< toc >}}

## Overview

DNA-protein interactions are fundamental to life processes, governing genome replication, repair, recombination, and transcriptional regulation. This resource systematically organizes major protein families that interact with DNA, providing a framework for understanding their coordinated roles in cellular functions.

---

## Classification Framework

This resource employs a **Structure-Enzyme-Regulation** framework that organizes DNA-binding proteins by their primary molecular roles:

<!-- - **Structural Proteins**: Establish and maintain the physical architecture of DNA/chromatin -->
  <!-- - *Includes*: Classical histones + 3D genome organizers (Cohesin, CTCF, Condensin)
  - *Rationale*: These proteins create physical structures, from nucleosomes to chromosomal loops -->

<!-- - **Enzymatic Proteins**: Catalyze chemical reactions on DNA -->
  <!-- - *Corresponds to*: Replication + Repair + Recombination factors in functional classifications
  - *Rationale*: Distinguished by their catalytic activity (e.g., polymerase, ligase, nuclease) -->

<!-- - **Regulatory Proteins**: Modulate gene expression without forming stable structures -->
  <!-- - *Includes*: Transcription factors + Chromatin modifiers + Epigenetic readers
  - *Rationale*: Control chromatin accessibility and transcriptional output -->

<!-- ### 💡 Connection to p53-Histone Competition Research

This classification directly supports the study of **transcription factor-nucleosome competition**:
- **Histones** (Structural) provide a stable, high-affinity DNA-packaging platform
- **p53** (Regulatory) must compete with histones for DNA access during stress responses
- Understanding their distinct roles clarifies the biophysical basis of this competition -->
---

<!-- ## Classification System

{{< figure src="/images/resource/DNA-Protein.png" caption="Overview of DNA-interacting protein classification" width="100%" >}} -->



<div class="taxonomy-container">

<!-- ========== Structural Proteins ========== -->
<div class="taxonomy-section structural">
  <h4>I. Structural Proteins</h4>
  <p class="category-description">Establish and maintain the physical architecture of DNA/chromatin.</p>
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA packaging proteins</span>
    <span class="taxonomy-proteins">
      <a href="structural/histones/">Histones</a> (H2A, H2B, H3, H4), Linker histone H1
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">3D genome organization</span>
    <span class="taxonomy-proteins">
      <a href="structural/cohesin/">Cohesin</a> (loop formation), 
      <a href="structural/ctcf/">CTCF</a> (boundary factor), 
      Condensin (mitotic condensation), 
      SMC5/6 (genome stability)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">Nuclear architecture</span>
    <span class="taxonomy-proteins">
      Lamin A/C, Nuclear matrix proteins (SAF-A)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">Architectural modulators</span>
    <span class="taxonomy-proteins">
      High-Mobility Group (HMG) proteins, DNA bending factors
    </span>
  </div>
</div>

<!-- ========== Enzymatic Proteins ========== -->
<div class="taxonomy-section enzymatic">
  <h4>II. Enzymatic Proteins</h4>
  <p class="category-description">Catalyze chemical reactions on DNA.</p>
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA replication enzymes</span>
    <span class="taxonomy-proteins">
      DNA polymerases (α, δ, ε), MCM complex (helicase), Primase
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA repair enzymes</span>
    <span class="taxonomy-proteins">
      DNA Ligase (I, III, IV), PARP1, Nucleases (XPF, FEN1), Rad50
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA recombination enzymes</span>
    <span class="taxonomy-proteins">
      <a href="enzymatic/reca">RecA</a><wbr>/Rad51/Dmc1<wbr> (homologous recombination)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA topoisomerases</span>
    <span class="taxonomy-proteins">
      Topoisomerase I, Topoisomerase II (relieve supercoiling)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA modification enzymes</span>
    <span class="taxonomy-proteins">
      DNA methyltransferases (DNMT1/3A/3B), TET enzymes (demethylation)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">DNA helicases</span>
    <span class="taxonomy-proteins">
      RecQ family (BLM, WRN), UvrD, Pif1
    </span>
  </div>
</div>

<!-- ========== Regulatory Proteins ========== -->
<div class="taxonomy-section regulatory">
  <h4>III. Regulatory Proteins</h4>
  <p class="category-description">Modulate gene expression without forming stable structures.</p>
  <div class="taxonomy-item">
    <span class="taxonomy-label">Transcription factors</span>
    <span class="taxonomy-proteins">
      <a href="regulatory/p53/">p53</a> (tumor suppressor), 
      MYC (growth regulator), 
      NF-κB (inflammation master), 
      Nuclear receptors (ER, GR)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">Chromatin remodelers</span>
    <span class="taxonomy-proteins">
      <a href="regulatory/swi-snf/">SWI/SNF</a> (BAF complex), 
      INO80, ISWI, CHD family (ATP-dependent remodeling)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">Histone modifying enzymes</span>
    <span class="taxonomy-proteins">
      HATs (p300/CBP, GCN5), 
      HDACs (Class I/II/III/IV), 
      HMTs (EZH2, SUV39H1), 
      HDMs (LSD1, JMJD2)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label"> Epigenetic readers</span>
    <span class="taxonomy-proteins">
      BRD4 (acetyl-lysine reader), 
      HP1α/β/γ (methyl-lysine reader), 
      CBX proteins (Polycomb readers)
    </span>
  </div>
  
  <div class="taxonomy-item">
    <span class="taxonomy-label">Transcriptional co-regulators</span>
    <span class="taxonomy-proteins">
      Mediator complex (MED1/12/14), 
      p300/CBP (co-activators), 
      NCoR/SMRT (co-repressors)
    </span>
  </div>
</div>

</div>

---
<!-- 
## Research Methodologies

### Single-Molecule Techniques
- **TIRF Microscopy**: Total Internal Reflection Fluorescence for visualizing protein-DNA dynamics
- **FRET**: Förster Resonance Energy Transfer for measuring conformational changes
- **CoSMoS**: Co-localization Single-Molecule Spectroscopy for complex assembly
- **Optical Tweezers**: Force measurement for nucleosome unwrapping and protein binding
- **AFM**: Atomic Force Microscopy for chromatin fiber imaging

### Biochemical Analysis
- **EMSA**: Electrophoretic Mobility Shift Assay for DNA-binding affinity
- **ChIP-seq**: Chromatin Immunoprecipitation Sequencing for genome-wide localization
- **ATAC-seq**: Assay for Transposase-Accessible Chromatin for chromatin accessibility
- **Pull-down Assays**: Protein-protein interaction mapping
- **DNase I Footprinting**: DNA-binding site identification

### Structural Biology
- **X-ray Crystallography**: High-resolution protein-DNA complex structures
- **Cryo-EM**: Cryo-Electron Microscopy for large chromatin complexes
- **NMR**: Nuclear Magnetic Resonance for dynamics and intrinsically disordered regions
- **SAXS**: Small-Angle X-ray Scattering for solution structures

### Computational Approaches
- **Molecular Dynamics**: Simulation of protein-DNA interactions
- **AlphaFold**: Structure prediction for uncharacterized proteins
- **Motif Discovery**: Position Weight Matrices (PWMs) for binding site prediction
- **Network Analysis**: Mapping transcriptional regulatory networks -->

---
<!-- 
## Cross-References

### Biological Processes
For a process-oriented view of how these proteins coordinate in cellular contexts, see:
- [Chromatin Architecture Establishment](/resource/processes/chromatin/)
- [Transcriptional Activation](/resource/processes/transcription/) *(planned)*
- [DNA Damage Repair](/resource/processes/repair/) *(planned)*
- [DNA Replication](/resource/processes/replication/) *(planned)*

### Featured Proteins
Detailed mechanistic studies:
- [Histones - Nucleosome Core](/resource/interactions/structural/histones/) ✅
- [p53 - Guardian of the Genome](/resource/interactions/regulatory/p53/) ✅
- [RecA/Rad51 - Homologous Recombination](/resource/interactions/enzymatic/reca-rad51/) ✅
- [LLPS in Genome Regulation](/resource/llps/) ✅

--- -->

<!-- ## Key References -->

### Classification Frameworks
1. **Zheng Z, Wang Y (2011)** *Biomol Concepts* 2011 Aug 1;2(4):293-303. 
   [DNA binding proteins: outline of functional classification](https://doi.org/10.1515/bmc.2011.023)

2. **Luscombe NM et al. (2000)** *Genome Biology* 1:reviews001.
   [An overview of the structures of protein-DNA complexes](https://doi.org/10.1186/gb-2000-1-1-reviews001)

<!-- ### Chromatin Architecture
3. **Dekker J, Mirny L (2016)** *Cell* 164:1110-1121  
   [The 3D genome as moderator of chromosomal communication](https://doi.org/10.1016/j.cell.2016.02.007)

4. **Rao SSP et al. (2014)** *Cell* 159:1665-1680  
   [A 3D map of the human genome at kilobase resolution reveals cohesin loops](https://www.cell.com/fulltext/S0092-8674(14)01497-4)

### Transcription Factor Mechanisms
5. **Spitz F, Furlong EEM (2012)** *Nat Rev Genet* 13:613-626  
   [Transcription factors: from enhancer binding to developmental control](https://doi.org/10.1038/nrg3207) -->

---
<!-- 
## Database Resources

- **UniProt**: Protein sequences and functional annotations
- **PDB**: Protein Data Bank for 3D structures
- **ENCODE**: Encyclopedia of DNA Elements (ChIP-seq, ATAC-seq data)
- **JASPAR**: Transcription factor binding site profiles
- **4DN**: 4D Nucleome project for chromatin organization

--- -->

**Last Updated**: 2025-11-24  
**Status**: Active development | Feedback welcome at sun_yuting@icloud.com
