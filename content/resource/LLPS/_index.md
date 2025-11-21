---
title: "Liquid-Liquid Phase Separation (LLPS)"
subtitle: "液-液相分離 - 生物分子凝聚體的形成與功能"
summary: "LLPS是細胞通過多價相互作用組織生化反應的普遍機制，在轉錄調控、染色質組織和DNA修復中發揮關鍵作用"
date: 2025-11-20
authors: ["Yu-Ting Sun"]
tags: ["LLPS", "Phase Separation", "Condensates", "Transcription", "Chromatin", "p53"]
categories: ["Molecular Mechanisms", "Nuclear Biology"]
type: page
toc: true
weight: 3
featured: true

image:
  caption: 'Cellular biomolecular condensates formed by LLPS (Banani et al. 2017)'
  focal_point: "Smart"
  preview_only: false
---

{{< toc >}}

<!-- 語言切換按鈕 -->
<div class="lang-toggle">
  <button onclick="toggleLanguage('both')" class="active">中英並排 Both</button>
  <button onclick="toggleLanguage('zh')">僅中文 Chinese Only</button>
  <button onclick="toggleLanguage('en')">僅英文 English Only</button>
</div>

<div class="bilingual-section">

<!-- ========== 概述部分 ========== -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

## 概述

液-液相分離（Liquid-Liquid Phase Separation, LLPS）是細胞內生物大分子通過**多價相互作用**自發形成**無膜細胞器**（membraneless organelles）的物理化學過程。這些動態的生物分子凝聚體（biomolecular condensates）在時空上組織生化反應，實現快速、可逆的功能調控。

在核生物學中，LLPS驅動形成：
- **轉錄凝聚體**：濃縮轉錄因子和共激活因子，增強基因激活
- **異染色質區域**：通過HP1α等蛋白相分離維持基因沉默
- **DNA修復病灶**：招募修復蛋白，加速損傷響應

**與本項目的關聯**：p53通過其固有無序區（IDR）驅動相分離，形成轉錄凝聚體，在與組蛋白的競爭中局部增強濃度，克服核小體屏障。

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

## Overview

Liquid-Liquid Phase Separation (LLPS) is a physicochemical process by which cellular biomacromolecules spontaneously form **membraneless organelles** through **multivalent interactions**. These dynamic biomolecular condensates spatiotemporally organize biochemical reactions, enabling rapid and reversible functional regulation.

In nuclear biology, LLPS drives the formation of:
- **Transcriptional condensates**: Concentrating transcription factors and coactivators to enhance gene activation
- **Heterochromatin domains**: Maintaining gene silencing through phase separation of proteins like HP1α
- **DNA repair foci**: Recruiting repair proteins to accelerate damage response

**Connection to this project**: p53 drives phase separation through its intrinsically disordered regions (IDRs), forming transcriptional condensates that locally enhance its concentration to overcome nucleosome barriers in competition with histones.

  </div>
</div>

<!-- 細胞內凝聚體全景圖 -->
<div style="text-align: center; margin: 2rem 0;">
  <img src="/images/resource/llps-overview.png" alt="Cellular LLPS-driven condensates" style="max-width: 100%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
  <p style="font-size: 0.9rem; color: #64748b; margin-top: 0.5rem;">
    <strong>Figure:</strong> Major LLPS-driven biomolecular condensates in cells<br>
    <em>Source: Banani et al. (2017) Nat Rev Mol Cell Biol 18:285-298</em>
  </p>
</div>

---

<!-- ========== Section 1: LLPS基礎概念 ========== -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

## Section 1: LLPS基礎概念

### 1.1 定義與核心驅動力

**什麼是LLPS？**

LLPS是指均一溶液在特定條件下（濃度、溫度、離子強度）分離成兩相：
- **稀相（dilute phase）**：蛋白濃度低，類似體相
- **緻密相（dense phase）**：蛋白濃度高，形成液滴狀凝聚體

**核心驅動力**：
1. **多價相互作用（Multivalent interactions）**
   - 多個弱相互作用位點的協同效應
   - 通過降低體系自由能驅動相分離 ([Flory-Huggins理論](https://doi.org/10.1038/nrm.2017.7))

2. **固有無序區（IDRs）**
   - 缺乏固定三維結構
   - 富含帶電、芳香族或極性氨基酸
   - 提供多個可逆結合位點

3. **特異性相互作用類型**：
   - **π-π堆積**：芳香族殘基（Phe, Tyr, Trp）
   - **靜電相互作用**：正負電荷吸引
   - **疏水作用**：疏水殘基聚集
   - **氫鍵網絡**：極性殘基介導

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

## Section 1: LLPS Fundamentals

### 1.1 Definition and Core Driving Forces

**What is LLPS?**

LLPS refers to the separation of a homogeneous solution into two phases under specific conditions (concentration, temperature, ionic strength):
- **Dilute phase**: Low protein concentration, similar to bulk
- **Dense phase**: High protein concentration, forming droplet-like condensates

**Core Driving Forces**:
1. **Multivalent interactions**
   - Synergistic effects of multiple weak interaction sites
   - Drive phase separation by reducing system free energy ([Flory-Huggins theory](https://doi.org/10.1038/nrm.2017.7))

2. **Intrinsically Disordered Regions (IDRs)**
   - Lack fixed 3D structure
   - Enriched in charged, aromatic, or polar amino acids
   - Provide multiple reversible binding sites

3. **Specific Interaction Types**:
   - **π-π stacking**: Aromatic residues (Phe, Tyr, Trp)
   - **Electrostatic interactions**: Attraction between opposite charges
   - **Hydrophobic effect**: Clustering of hydrophobic residues
   - **Hydrogen bond networks**: Mediated by polar residues

  </div>
</div>

<!-- 1.2 分子基礎 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 1.2 分子基礎

**IDR的特徵**：
- **序列組成**：
  - 低複雜度序列（LCD）：重複的短氨基酸motif
  - Prion-like domains（PrLDs）：類朊病毒結構域（Gln/Asn富集）
  - RGG/FG重複：RNA結合蛋白常見

- **結構特性**：
  - 無固定二級/三級結構
  - 構象高度靈活（ensemble of states）
  - 響應環境快速變化

**關鍵氨基酸類型**：

| 類型 | 代表氨基酸 | 作用機制 |
|------|-----------|---------|
| **芳香族** | Phe, Tyr, Trp | π-π堆積，疏水作用 |
| **帶正電** | Arg, Lys | 靜電相互作用，結合DNA/RNA |
| **帶負電** | Glu, Asp | 靜電相互作用，調控相分離閾值 |
| **極性** | Ser, Thr, Gln, Asn | 氫鍵網絡，穩定液滴 |
| **小分子** | Gly, Ala | 提供構象靈活性 |

**實例**：
- **p53的TAD（1-67）**：富含Phe/Trp（π-π）+ 酸性殘基（靜電）
- **HP1α的Hinge**：帶正電IDR，結合H3K9me3並驅動相分離
- **FUS的LCD**：Gly/Ser/Gln/Tyr富集，形成水凝膠狀液滴

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

### 1.2 Molecular Basis

**IDR Characteristics**:
- **Sequence Composition**:
  - Low Complexity Domains (LCDs): Repetitive short amino acid motifs
  - Prion-like Domains (PrLDs): Enriched in Gln/Asn
  - RGG/FG repeats: Common in RNA-binding proteins

- **Structural Properties**:
  - No fixed secondary/tertiary structure
  - Highly flexible conformation (ensemble of states)
  - Rapid response to environmental changes

**Key Amino Acid Types**:

| Type | Representative AAs | Mechanism |
|------|-------------------|-----------|
| **Aromatic** | Phe, Tyr, Trp | π-π stacking, hydrophobic effect |
| **Positively charged** | Arg, Lys | Electrostatic interactions, DNA/RNA binding |
| **Negatively charged** | Glu, Asp | Electrostatic interactions, regulate phase separation threshold |
| **Polar** | Ser, Thr, Gln, Asn | Hydrogen bond networks, stabilize droplets |
| **Small** | Gly, Ala | Provide conformational flexibility |

**Examples**:
- **p53 TAD (1-67)**: Rich in Phe/Trp (π-π) + acidic residues (electrostatic)
- **HP1α Hinge**: Positively charged IDR, binds H3K9me3 and drives phase separation
- **FUS LCD**: Enriched in Gly/Ser/Gln/Tyr, forms hydrogel-like droplets

  </div>
</div>

<!-- 1.3 物理特性 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 1.3 關鍵物理特性

**濃度閾值（Saturation concentration, Csat）**：
- 超過此濃度時發生相分離
- 受溫度、鹽濃度、pH、分子擁擠等影響
- 細胞通過調控濃度控制凝聚體形成

**動態流動性**：
- 凝聚體內分子快速交換（秒-分鐘級）
- FRAP實驗：螢光恢復半衰期 t₁/₂ ~ 10-100 s
- 不同於固體聚集體（如澱粉樣蛋白）

**環境因素影響**：

| 因素 | 效應 | 機制 |
|------|------|------|
| **溫度↑** | 相分離減弱 | 增加熵，破壞弱相互作用 |
| **鹽濃度↑** | 雙向調節 | 低鹽促進（屏蔽同種電荷），高鹽抑制（競爭結合） |
| **分子擁擠** | 促進相分離 | 排除體積效應，降低Csat |
| **翻譯後修飾** | 精細調節 | 磷酸化通常抑制，甲基化/乙醯化促進 |

**相圖示例**：

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

### 1.3 Key Physical Properties

**Saturation Concentration (Csat)**:
- Phase separation occurs above this concentration
- Influenced by temperature, salt, pH, molecular crowding
- Cells control condensate formation by regulating concentration

**Dynamic Fluidity**:
- Rapid molecular exchange within condensates (seconds-minutes)
- FRAP experiments: Fluorescence recovery half-time t₁/₂ ~ 10-100 s
- Distinct from solid aggregates (e.g., amyloid)

**Environmental Factors**:

| Factor | Effect | Mechanism |
|--------|--------|-----------|
| **Temperature↑** | Weaken phase separation | Increase entropy, disrupt weak interactions |
| **Salt↑** | Biphasic regulation | Low salt promotes (screen like charges), high salt inhibits (compete for binding) |
| **Molecular crowding** | Promote phase separation | Excluded volume effect, lower Csat |
| **Post-translational modifications** | Fine-tuning | Phosphorylation usually inhibits, methylation/acetylation promote |

**Phase Diagram Example**:

  </div>
</div>

<!-- 相圖插圖 -->
<div style="text-align: center; margin: 2rem 0;">
  <img src="/images/resource/llps-phase-diagram.png" alt="LLPS phase diagram" style="max-width: 80%; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
  <p style="font-size: 0.9rem; color: #64748b; margin-top: 0.5rem;">
    <strong>Figure:</strong> Phase diagram showing nucleation and spinodal decomposition mechanisms<br>
    <em>Source: Alberti et al. (2019) Cell 176:419-434</em>
  </p>
</div>

<div class="bilingual-pair">
  <div class="lang-zh-block">

**兩種形成機制**：
- **成核（Nucleation）**：濃度略超閾值時，小液滴逐漸長大
- **旋節分解（Spinodal decomposition）**：濃度遠超閾值時，快速形成網絡狀凝聚體

*詳細物理原理見 [Alberti et al. 2019](https://doi.org/10.1016/j.cell.2018.12.035)*

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

**Two Formation Mechanisms**:
- **Nucleation**: Small droplets gradually grow when concentration slightly exceeds threshold
- **Spinodal decomposition**: Rapid network formation when concentration far exceeds threshold

*For detailed physical principles, see [Alberti et al. 2019](https://doi.org/10.1016/j.cell.2018.12.035)*

  </div>
</div>

---

<!-- ========== Section 2: LLPS在核生物學中的作用 ========== -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

## Section 2: LLPS在核生物學中的作用

### 2.1 轉錄調控中的LLPS

#### 轉錄凝聚體的形成

轉錄激活需要轉錄因子（TFs）、共激活因子、Mediator複合體和RNA Pol II在特定基因位點的協同作用。LLPS提供了一種**時空濃縮機制**：

**超級增強子（Super-enhancers）的相分離**：
- 多個增強子簇集形成高濃度TF結合位點
- Mediator的MED1亞基（含IDR）驅動相分離
- 形成轉錄工廠（transcription factories）
- 排除抑制因子，選擇性富集激活因子

**關鍵轉錄凝聚體**：

| 凝聚體類型 | 核心蛋白 | 驅動區域 | 功能 |
|-----------|---------|---------|------|
| **p53凝聚體** ⭐ | p53 | TAD (1-67) | 應激響應，細胞週期阻滯 |
| **MYC凝聚體** | MYC, MAX | N-terminal LCD | 生長調控，代謝重編程 |
| **ER凝聚體** | ER, Mediator | IDR + AF2 | 雌激素響應 |
| **GCN4凝聚體** | GCN4, Mediator | Acidic AD | 營養缺乏響應 |

#### p53凝聚體與組蛋白競爭 ⭐⭐⭐

**p53如何通過相分離克服核小體屏障**：

1. **基礎狀態**（無應激）：
   - p53濃度低（~10 nM）
   - 組蛋白佔據優勢（~10 μM）
   - 核小體緊密包裝DNA，p53結合位點被遮蔽

2. **應激激活**（DNA損傷）：
   - ATM/ATR磷酸化 → p53穩定化
   - p53濃度劇增（~1 μM）
   - **TAD驅動相分離形成凝聚體**

3. **局部濃度增強**：
   - 凝聚體內p53濃度：**~100 μM**
   - 遠超體相濃度，改變競爭平衡
   - 利用核小體呼吸窗口（50-250 ms）結合DNA

4. **招募染色質重塑酶**：
   - p53凝聚體招募p300/CBP（HAT活性）
   - 組蛋白乙醯化 → 核小體不穩定
   - SWI/SNF複合體移除核小體

5. **維持開放染色質**：
   - 相分離持續存在（分鐘-小時）
   - 防止核小體快速重新組裝
   - 持續轉錄激活

**實驗證據**：
- Chong et al. (2018): 體外重構p53液滴
- Guo et al. (2019): 活細胞成像觀察p53病灶

**MYC-p53 Sequential Remodeling假說**：
- 增殖期：MYC凝聚體主導 → 增殖基因激活
- 複製壓力：R-loop形成 → DNA損傷
- 狀態轉換：MYC凝聚體解體，p53凝聚體形成
- 修復狀態：p53凝聚體主導 → 修復基因激活

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

## Section 2: LLPS Roles in Nuclear Biology

### 2.1 LLPS in Transcriptional Regulation

#### Formation of Transcriptional Condensates

Transcriptional activation requires cooperative action of transcription factors (TFs), coactivators, Mediator complex, and RNA Pol II at specific gene loci. LLPS provides a **spatiotemporal concentration mechanism**:

**Super-enhancer Phase Separation**:
- Multiple enhancer clusters form high-density TF binding sites
- Mediator's MED1 subunit (containing IDR) drives phase separation
- Form transcription factories
- Exclude repressors, selectively enrich activators

**Key Transcriptional Condensates**:

| Condensate Type | Core Proteins | Driving Region | Function |
|----------------|---------------|----------------|----------|
| **p53 condensate** ⭐ | p53 | TAD (1-67) | Stress response, cell cycle arrest |
| **MYC condensate** | MYC, MAX | N-terminal LCD | Growth control, metabolic reprogramming |
| **ER condensate** | ER, Mediator | IDR + AF2 | Estrogen response |
| **GCN4 condensate** | GCN4, Mediator | Acidic AD | Nutrient starvation response |

#### p53 Condensates and Histone Competition ⭐⭐⭐

**How p53 Overcomes Nucleosome Barriers via Phase Separation**:

1. **Basal State** (No Stress):
   - Low p53 concentration (~10 nM)
   - Histones dominate (~10 μM)
   - Nucleosomes tightly package DNA, p53 binding sites occluded

2. **Stress Activation** (DNA Damage):
   - ATM/ATR phosphorylation → p53 stabilization
   - p53 concentration surges (~1 μM)
   - **TAD-driven phase separation forms condensates**

3. **Local Concentration Enhancement**:
   - p53 concentration inside condensates: **~100 μM**
   - Far exceeds bulk concentration, shifts competitive equilibrium
   - Exploit nucleosome breathing windows (50-250 ms) to bind DNA

4. **Recruit Chromatin Remodelers**:
   - p53 condensates recruit p300/CBP (HAT activity)
   - Histone acetylation → nucleosome destabilization
   - SWI/SNF complex removes nucleosomes

5. **Maintain Open Chromatin**:
   - Phase separation persists (minutes-hours)
   - Prevent rapid nucleosome reassembly
   - Sustain transcriptional activation

**Experimental Evidence**:
- Chong et al. (2018): In vitro reconstitution of p53 droplets
- Guo et al. (2019): Live-cell imaging of p53 foci


**MYC-p53 Sequential Remodeling Hypothesis**:
- Proliferation phase: MYC condensate dominates → proliferation gene activation
- Replication stress: R-loop formation → DNA damage
- State transition: MYC condensate dissolves, p53 condensate forms
- Repair state: p53 condensate dominates → repair gene activation

  </div>
</div>

<!-- 2.2 染色質組織 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 2.2 染色質組織中的LLPS

#### HP1α驅動的異染色質形成

**機制**：
1. **識別**：HP1α的Chromodomain識別H3K9me3
2. **二聚化**：HP1α同源二聚體形成
3. **相分離**：Hinge區（IDR）介導多價相互作用
4. **擴散**：HP1α液滴招募更多HP1α和HMT（如SUV39H）
5. **正反饋**：新甲基化的H3K9me3進一步招募HP1α

**特性**：
- 液滴直徑：0.2-2 μm
- FRAP恢復時間：~30 s
- 排除RNA Pol II和轉錄激活因子
- 維持基因沉默狀態

#### Polycomb body形成

**核心成分**：
- PRC1/PRC2複合體
- CBX蛋白（識別H3K27me3）
- EZH2（催化H3K27me3）

**功能**：
- Polycomb靶基因共定位
- 形成抑制性核區域
- 發育基因的長程沉默

#### 其他核凝聚體

| 凝聚體 | 核心蛋白 | 功能 |
|--------|---------|------|
| **核仁** | Nucleolin, Fibrillarin | rRNA轉錄與加工 |
| **核斑點** | SRSF2, SON | mRNA剪接因子儲存 |
| **PML body** | PML, SUMO | 應激響應，腫瘤抑制 |
| **Cajal body** | Coilin | snRNA成熟 |

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

### 2.2 LLPS in Chromatin Organization

#### HP1α-Driven Heterochromatin Formation

**Mechanism**:
1. **Recognition**: HP1α Chromodomain recognizes H3K9me3
2. **Dimerization**: HP1α homodimer formation
3. **Phase Separation**: Hinge region (IDR) mediates multivalent interactions
4. **Spreading**: HP1α droplets recruit more HP1α and HMTs (e.g., SUV39H)
5. **Positive Feedback**: Newly methylated H3K9me3 further recruits HP1α

**Properties**:
- Droplet diameter: 0.2-2 μm
- FRAP recovery time: ~30 s
- Exclude RNA Pol II and transcriptional activators
- Maintain gene silencing state

#### Polycomb Body Formation

**Core Components**:
- PRC1/PRC2 complexes
- CBX proteins (recognize H3K27me3)
- EZH2 (catalyzes H3K27me3)

**Functions**:
- Co-localization of Polycomb target genes
- Form repressive nuclear domains
- Long-range silencing of developmental genes

#### Other Nuclear Condensates

| Condensate | Core Proteins | Function |
|-----------|--------------|----------|
| **Nucleolus** | Nucleolin, Fibrillarin | rRNA transcription & processing |
| **Nuclear speckles** | SRSF2, SON | mRNA splicing factor storage |
| **PML body** | PML, SUMO | Stress response, tumor suppression |
| **Cajal body** | Coilin | snRNA maturation |

  </div>
</div>

<!-- 2.3 DNA損傷修復 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 2.3 DNA損傷修復中的LLPS

#### 修復病灶的液滴性質

**雙鏈斷裂（DSB）響應**：
1. **初始信號**：γH2AX標記損傷位點
2. **53BP1招募**：
   - 53BP1低複雜度區域驅動相分離
   - 形成微米級病灶（修復工廠）
   - 濃縮BRCA1, Rad51等修復蛋白

3. **動態流動性**：
   - FRAP實驗證實液滴特性
   - 允許修復蛋白快速交換
   - 根據修復進程動態重組

**功能優勢**：
- **濃縮效應**：提高局部酶濃度，加速修復
- **選擇性分配**：排除不相關蛋白，避免干擾
- **可逆性**：修復完成後快速解散

**病理意義**：
- 過度穩定的液滴 → 修復延遲
- 相分離缺陷 → 基因組不穩定性
- 靶向液滴動態 → 潛在治療策略

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

### 2.3 LLPS in DNA Damage Repair

#### Liquid Droplet Properties of Repair Foci

**Double-Strand Break (DSB) Response**:
1. **Initial Signal**: γH2AX marks damage site
2. **53BP1 Recruitment**:
   - 53BP1 low-complexity region drives phase separation
   - Forms micrometer-scale foci (repair factories)
   - Concentrates BRCA1, Rad51, and other repair proteins

3. **Dynamic Fluidity**:
   - FRAP experiments confirm droplet properties
   - Allow rapid exchange of repair proteins
   - Dynamically reorganize according to repair progress

**Functional Advantages**:
- **Concentration Effect**: Increase local enzyme concentration, accelerate repair
- **Selective Partitioning**: Exclude irrelevant proteins, avoid interference
- **Reversibility**: Rapidly disassemble after repair completion

**Pathological Significance**:
- Overly stable droplets → repair delay
- Phase separation defects → genomic instability
- Targeting droplet dynamics → potential therapeutic strategies

  </div>
</div>

---

<!-- ========== Section 3: 關鍵LLPS驅動蛋白 ========== -->
<div class="bilingual-pair">

  <div class="lang-zh-block">

## Section 3: 關鍵LLPS驅動蛋白

下表列出了主要的LLPS驅動蛋白及其特徵。⭐ 標記的蛋白與本項目研究重點相關。

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

## Section 3: Key LLPS-Driving Proteins

The table lists major LLPS-driving proteins and their characteristics. ⭐ marks proteins related to project research focus.

  </div>

</div>

<div style="overflow-x: auto; margin: 1.5rem 0;">
<table class="table table-hover table-bordered">
  <thead class="thead-light">
    <tr>
      <th width="12%">Category</th>
      <th width="15%">Protein</th>
      <th width="23%">LLPS-Driving Region</th>
      <th width="30%">Function</th>
      <th width="20%">Details</th>
    </tr>
  </thead>
  <tbody>
    <!-- 轉錄因子類 -->
    <tr style="background: #e0f2fe;">
      <td rowspan="4" style="vertical-align: middle; font-weight: 600; color: #0369a1;">
        <strong>轉錄因子<br>Transcription<br>Factors</strong>
      </td>
      <td><strong>p53</strong> ⭐⭐⭐</td>
      <td>TAD (aa 1-67)<br><small>Aromatic + Acidic</small></td>
      <td>Stress response, cell cycle arrest, tumor suppression</td>
      <td><a href="/resource/interactions/regulatory/p53/" class="btn btn-sm btn-outline-primary">View →</a></td>
    </tr>
    <tr style="background: #e0f2fe;">
      <td><strong>MYC</strong></td>
      <td>N-terminal LCD (aa 1-143)<br><small>Charged residues</small></td>
      <td>Growth control, metabolic regulation</td>
      <td><span class="badge badge-secondary">Planned</span></td>
    </tr>
    <tr style="background: #e0f2fe;">
      <td><strong>NFAT5</strong></td>
      <td>Auxiliary domain<br><small>IDR</small></td>
      <td>Osmotic stress response</td>
      <td>—</td>
    </tr>
    <tr style="background: #e0f2fe;">
      <td><strong>GCN4</strong></td>
      <td>Acidic activation domain</td>
      <td>Amino acid starvation response</td>
      <td>—</td>
    </tr>
    <!-- 染色質蛋白類 -->
    <tr style="background: #d1fae5;">
      <td rowspan="4" style="vertical-align: middle; font-weight: 600; color: #065f46;">
        <strong>染色質蛋白<br>Chromatin<br>Proteins</strong>
      </td>
      <td><strong>HP1α</strong> ⭐⭐</td>
      <td>Hinge (aa 70-120)<br><small>Positively charged IDR</small></td>
      <td>Heterochromatin formation, gene silencing</td>
      <td><a href="/resource/interactions/structural/hp1/" class="btn btn-sm btn-outline-success">View →</a></td>
    </tr>
    <tr style="background: #d1fae5;">
      <td><strong>PRC1 (CBX2)</strong></td>
      <td>C-terminal IDR (aa 300-532)<br><small>Low complexity</small></td>
      <td>Polycomb body formation</td>
      <td>—</td>
    </tr>
    <tr style="background: #d1fae5;">
      <td><strong>BRD4</strong></td>
      <td>IDR<br><small>Intrinsically disordered</small></td>
      <td>Super-enhancer assembly, transcription elongation</td>
      <td>—</td>
    </tr>
    <tr style="background: #d1fae5;">
      <td><strong>TIP5</strong></td>
      <td>IDR + RNA-binding</td>
      <td>Nucleolar silencing</td>
      <td>—</td>
    </tr>
    <!-- 共激活因子類 -->
    <tr style="background: #fce7f3;">
      <td rowspan="4" style="vertical-align: middle; font-weight: 600; color: #9f1239;">
        <strong>共激活因子<br>Coactivators</strong>
      </td>
      <td><strong>Mediator (MED1)</strong> ⭐</td>
      <td>IDR (aa 1-580)<br><small>Super-enhancer driver</small></td>
      <td>Transcription factory formation</td>
      <td>—</td>
    </tr>
    <tr style="background: #fce7f3;">
      <td><strong>p300/CBP</strong></td>
      <td>CH1-KIX-CH3 linkers<br><small>IDR</small></td>
      <td>Histone acetylation, chromatin opening</td>
      <td>—</td>
    </tr>
    <tr style="background: #fce7f3;">
      <td><strong>YAP/TAZ</strong></td>
      <td>C-terminal IDR</td>
      <td>Hippo pathway, mechanotransduction</td>
      <td>—</td>
    </tr>
    <tr style="background: #fce7f3;">
      <td><strong>NELF</strong></td>
      <td>RRM + IDR</td>
      <td>Transcription pausing control</td>
      <td>—</td>
    </tr>
  </tbody>
</table>

</div>


<!-- IDR對比表格 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 關鍵蛋白的IDR結構特徵

下表總結了主要LLPS驅動蛋白的IDR位置、序列特徵和驅動機制：

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

### IDR Structural Features of Key Proteins

The table summarizes the IDR positions, sequence features, and driving mechanisms of major LLPS-driving proteins:

  </div>
</div>

<div style="overflow-x: auto; margin: 1.5rem 0;">

<table class="table table-hover table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Protein</th>
      <th>IDR Region (aa)</th>
      <th>Key Residues</th>
      <th>Driving Mechanism</th>
      <th>Csat (approx.)</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: #fef3c7;">
      <td><strong>p53</strong></td>
      <td>TAD (1-67)<br>CTD (363-393)</td>
      <td>Phe, Trp (π-π)<br>Glu, Asp (electrostatic)</td>
      <td>Aromatic stacking + Electrostatic</td>
      <td>~0.5 μM</td>
    </tr>
    <tr>
      <td><strong>MYC</strong></td>
      <td>N-term (1-143)</td>
      <td>Charged residues (Arg, Glu)</td>
      <td>Electrostatic interactions</td>
      <td>~2 μM</td>
    </tr>
    <tr style="background: #d1fae5;">
      <td><strong>HP1α</strong></td>
      <td>Hinge (70-120)</td>
      <td>Arg, Lys (positive)<br>RNA-binding</td>
      <td>Electrostatic + RNA bridging</td>
      <td>~1 μM</td>
    </tr>
    <tr>
      <td><strong>CBX2</strong></td>
      <td>C-term (300-532)</td>
      <td>Low complexity</td>
      <td>Weak multivalent interactions</td>
      <td>~5 μM</td>
    </tr>
    <tr style="background: #fce7f3;">
      <td><strong>MED1</strong></td>
      <td>IDR (1-580)</td>
      <td>Ser, Thr, Gln-rich</td>
      <td>Polar interactions + TF binding</td>
      <td>~0.1 μM</td>
    </tr>
    <tr>
      <td><strong>FUS</strong></td>
      <td>LCD (1-267)</td>
      <td>Gly, Ser, Gln, Tyr</td>
      <td>π-π + Hydrogen bonds</td>
      <td>~0.05 μM</td>
    </tr>
  </tbody>
</table>

</div>

<div class="bilingual-pair">
  <div class="lang-zh-block">

**表格說明**：
- **Csat**：體外測定的相分離濃度閾值（實際細胞內受多種因素調控）
- **高亮行**：與本項目研究重點相關（p53, HP1α, MED1）
- **FUS**：RNA結合蛋白，作為經典LLPS模型蛋白列出

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

**Table Notes**:
- **Csat**: In vitro measured phase separation concentration threshold (regulated by multiple factors in cells)
- **Highlighted rows**: Related to project research focus (p53, HP1α, MED1)
- **FUS**: RNA-binding protein, listed as a classical LLPS model protein

  </div>
</div>

---

<!-- ========== 推薦閱讀區 ========== -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

## 推薦閱讀 | Recommended Reading

### 里程碑綜述

1. **Banani SF, Lee HO, Hyman AA, Rosen MK (2017)**
   *Biomolecular condensates: organizers of cellular biochemistry*
   **Nat Rev Mol Cell Biol** 18:285-298
   [DOI: 10.1038/nrm.2017.7](https://doi.org/10.1038/nrm.2017.7)
   - LLPS領域的全面綜述，涵蓋基本原理、生物學功能和疾病相關性

2. **Sabari BR, Dall'Agnese A, Young RA (2020)**
   *Biomolecular condensates in the nucleus*
   **Trends Biochem Sci** 45:961-977
   [DOI: 10.1016/j.tibs.2020.06.007](https://doi.org/10.1016/j.tibs.2020.06.007)
   - 聚焦轉錄凝聚體的形成、功能和調控機制

### p53相關原創研究

3. **Chong S, Dugast-Darzacq C, Liu Z, et al. (2018)**
   *Imaging dynamic and selective low-complexity domain interactions that control gene transcription*
   **Science** 361:eaar2555
   [DOI: 10.1126/science.aar2555](https://doi.org/10.1126/science.aar2555)
   - 首次在活細胞中觀察到p53等轉錄因子的液滴動態

4. **Guo YE, Manteiga JC, Henninger JE, et al. (2019)**
   *Pol II phosphorylation regulates a switch between transcriptional and splicing condensates*
   **Nature** 572:543-548
   [DOI: 10.1038/s41586-019-1464-0](https://doi.org/10.1038/s41586-019-1464-0)
   - 揭示轉錄凝聚體與剪接凝聚體的動態轉換

### 異染色質相分離

5. **Strom AR, Emelyanov AV, Mir M, et al. (2017)**
   *Phase separation drives heterochromatin domain formation*
   **Nature** 547:241-245
   [DOI: 10.1038/nature22989](https://doi.org/10.1038/nature22989)
   - 證明HP1α通過相分離驅動異染色質形成

6. **Sanulli S, Trnka MJ, Dharmarajan V, et al. (2019)**
   *HP1 reshapes nucleosome-containing chromatin*
   **Nature** 575:390-394
   [DOI: 10.1038/s41586-019-1669-2](https://doi.org/10.1038/s41586-019-1669-2)
   - Fierz實驗室揭示HP1α如何通過相分離重塑染色質結構

### 物理機制與理論

7. **Alberti S, Gladfelter A, Mittag T (2019)**
   *Considerations and challenges in studying liquid-liquid phase separation and biomolecular condensates*
   **Cell** 176:419-434
   [DOI: 10.1016/j.cell.2018.12.035](https://doi.org/10.1016/j.cell.2018.12.035)
   - 討論LLPS研究的方法學挑戰和注意事項

  </div>

  <div class="bilingual-divider"></div>

  <div class="lang-en-block">

## Recommended Reading

### Milestone Reviews

1. **Banani SF, Lee HO, Hyman AA, Rosen MK (2017)**
   *Biomolecular condensates: organizers of cellular biochemistry*
   **Nat Rev Mol Cell Biol** 18:285-298
   [DOI: 10.1038/nrm.2017.7](https://doi.org/10.1038/nrm.2017.7)
   - Comprehensive review of LLPS, covering principles, biological functions, and disease relevance

2. **Sabari BR, Dall'Agnese A, Young RA (2020)**
   *Biomolecular condensates in the nucleus*
   **Trends Biochem Sci** 45:961-977
   [DOI: 10.1016/j.tibs.2020.06.007](https://doi.org/10.1016/j.tibs.2020.06.007)
   - Focus on transcriptional condensate formation, function, and regulation

### p53-Related Original Research

3. **Chong S, Dugast-Darzacq C, Liu Z, et al. (2018)**
   *Imaging dynamic and selective low-complexity domain interactions that control gene transcription*
   **Science** 361:eaar2555
   [DOI: 10.1126/science.aar2555](https://doi.org/10.1126/science.aar2555)
   - First observation of p53 and other TF droplet dynamics in live cells

4. **Guo YE, Manteiga JC, Henninger JE, et al. (2019)**
   *Pol II phosphorylation regulates a switch between transcriptional and splicing condensates*
   **Nature** 572:543-548
   [DOI: 10.1038/s41586-019-1464-0](https://doi.org/10.1038/s41586-019-1464-0)
   - Reveals dynamic transition between transcriptional and splicing condensates

### Heterochromatin Phase Separation

5. **Strom AR, Emelyanov AV, Mir M, et al. (2017)**
   *Phase separation drives heterochromatin domain formation*
   **Nature** 547:241-245
   [DOI: 10.1038/nature22989](https://doi.org/10.1038/nature22989)
   - Demonstrates HP1α-driven heterochromatin formation via phase separation

6. **Sanulli S, Trnka MJ, Dharmarajan V, et al. (2019)**
   *HP1 reshapes nucleosome-containing chromatin*
   **Nature** 575:390-394
   [DOI: 10.1038/s41586-019-1669-2](https://doi.org/10.1038/s41586-019-1669-2)
   - Fierz lab reveals how HP1α reshapes chromatin structure via phase separation

### Physical Mechanisms and Theory

7. **Alberti S, Gladfelter A, Mittag T (2019)**
   *Considerations and challenges in studying liquid-liquid phase separation and biomolecular condensates*
   **Cell** 176:419-434
   [DOI: 10.1016/j.cell.2018.12.035](https://doi.org/10.1016/j.cell.2018.12.035)
   - Discusses methodological challenges and considerations in LLPS research

  </div>
</div>

---


<!-- JavaScript for language toggle -->
<script>
function toggleLanguage(lang) {
  const section = document.querySelector('.bilingual-section');
  const buttons = document.querySelectorAll('.lang-toggle button');
  
  buttons.forEach(btn => btn.classList.remove('active'));
  
  if (lang === 'zh') {
    section.classList.add('hide-en');
    section.classList.remove('hide-zh');
    buttons[1].classList.add('active');
  } else if (lang === 'en') {
    section.classList.add('hide-zh');
    section.classList.remove('hide-en');
    buttons[2].classList.add('active');
  } else {
    section.classList.remove('hide-zh', 'hide-en');
    buttons[0].classList.add('active');
  }
}
</script>

<style>
/* Card hover effect */
.hover-card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.hover-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0,0,0,0.15) !important;
}

/* Protein card styling - Fix overlapping issue */
.protein-item {
  display: block;
  padding: 0.75rem 0;
  border-bottom: 1px solid #f1f5f9;
  min-height: 80px;
}

.protein-item:last-child {
  border-bottom: none;
}

.protein-name {
  display: block;
  margin-bottom: 0.5rem;
  line-height: 1.4;
}

.protein-details {
  display: block;
  margin-bottom: 0.5rem;
}

.protein-details small {
  display: block;
  margin-bottom: 0.25rem;
  line-height: 1.5;
}

.priority-badge {
  display: inline-block;
  margin-left: 0.25rem;
  font-size: 0.9em;
  vertical-align: middle;
}

/* Ensure proper alignment in bilingual blocks */
.lang-zh-block h3, .lang-en-block h3 {
  color: #1e293b;
  border-bottom: 2px solid #e5e7eb;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

.lang-zh-block h4, .lang-en-block h4 {
  color: #475569;
  margin-top: 1.5rem;
}

/* Table styling enhancement */
.table-hover tbody tr:hover {
  background-color: #f0f9ff;
}

/* Dark mode support */
@media (prefers-color-scheme: dark) {
  .protein-item {
    border-bottom-color: #334155;
  }
  
  .lang-zh-block h3, .lang-en-block h3 {
    color: #e2e8f0;
    border-bottom-color: #475569;
  }
  
  .lang-zh-block h4, .lang-en-block h4 {
    color: #cbd5e1;
  }
  
  .table-hover tbody tr:hover {
    background-color: #1e3a5f;
  }
  
  .card {
    background: #1e293b;
    border-color: #334155;
  }
  
  .alert-success {
    background-color: #064e3b;
    border-color: #065f46;
    color: #d1fae5;
  }
  
  .alert-info {
    background-color: #1e3a8a;
    border-color: #1e40af;
    color: #dbeafe;
  }
  
  .alert-warning {
    background-color: #78350f;
    border-color: #92400e;
    color: #fef3c7;
  }
}
</style>
