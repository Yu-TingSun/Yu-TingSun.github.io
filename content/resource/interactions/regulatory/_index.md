---
title: "Regulatory Proteins"
subtitle: "调控蛋白 - 基因表达与染色质状态调节"
summary: "调控转录、染色质结构和表观遗传状态的蛋白质"
date: 2025-01-15
---

{{< toc >}}

## 概述 | Overview

调控蛋白通过识别特定DNA序列或染色质结构，控制基因转录、染色质可及性和表观遗传状态。这些蛋白是细胞命运决定、应激反应和疾病发生的关键调节因子。

Regulatory proteins control gene transcription, chromatin accessibility, and epigenetic states by recognizing specific DNA sequences or chromatin structures. These proteins are key regulators of cell fate determination, stress responses, and disease development.

---

## 蛋白质家族 | Protein Families

### 1. 转录因子 | Transcription Factors

#### ✓ p53 - Guardian of the Genome
<div class="card mb-3">
  <div class="row no-gutters">
    <div class="col-md-3">
      <img src="p53/featured.jpg" class="card-img" alt="p53 tetramer bound to DNA">
    </div>
    <div class="col-md-9">
      <div class="card-body">
        <h5 class="card-title">
          <a href="p53/">肿瘤抑制蛋白 | Tumor Suppressor</a>
        </h5>
        <p class="card-text">
          <strong>结构：</strong>
          <ul>
            <li><strong>TAD (1-67):</strong> 转录激活结构域</li>
            <li><strong>PRD (67-98):</strong> 富脯氨酸结构域</li>
            <li><strong>DBD (98-303):</strong> DNA结合结构域</li>
            <li><strong>TD (323-363):</strong> 四聚化结构域</li>
            <li><strong>CTD (363-393):</strong> C端调控结构域</li>
          </ul>
          <strong>功能机制：</strong>
          <ul>
            <li>DNA损伤响应与细胞周期阻滞</li>
            <li>细胞凋亡与衰老诱导</li>
            <li>与组蛋白竞争染色质结合</li>
            <li>液-液相分离形成转录凝聚体</li>
          </ul>
          <strong>研究方法：</strong>Single-molecule imaging, LLPS assays, ChIP-seq, Co-IP
        </p>
        <p class="card-text">
          <span class="badge badge-danger">50% cancers mutated</span>
          <span class="badge badge-info">Drug target</span>
          <span class="badge badge-success">Complete</span>
        </p>
        <div class="mt-2">
          <a href="p53/" class="btn btn-sm btn-outline-primary">查看详情 →</a>
          <a href="p53/histone-competition/" class="btn btn-sm btn-outline-secondary">p53-组蛋白竞争 →</a>
          <a href="p53/phase-separation/" class="btn btn-sm btn-outline-secondary">相分离机制 →</a>
        </div>
      </div>
    </div>
  </div>
</div>

**研究亮点：**
- ✨ p53-组蛋白在生理条件下的竞争结合机制
- ✨ p53相分离对转录激活的影响
- ✨ 突变型p53的功能获得（gain-of-function）

---

#### ⏳ MYC - Master Growth Regulator
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">生长调控转录因子 | Growth Master TF</span>
      <span class="badge badge-warning float-right">高优先级</span>
    </h5>
    <p class="card-text text-muted">
      <strong>功能：</strong>
      <ul>
        <li>细胞增殖与代谢调控</li>
        <li>与MAX异源二聚化结合E-box (CACGTG)</li>
        <li>激活~15%基因组基因</li>
        <li>形成转录凝聚体</li>
      </ul>
      <strong>临床意义：</strong>
      <ul>
        <li>多种癌症中过表达或扩增</li>
        <li>与p53在细胞命运决定中的拮抗作用</li>
        <li>MYC-p53凝聚体sequential remodeling机制</li>
      </ul>
      <strong>研究方向：</strong>
      <ul>
        <li>MYC-MAX-DNA三元复合物结构</li>
        <li>复制压力下的MYC→p53转换</li>
        <li>相分离驱动的基因激活</li>
      </ul>
    </p>
    <p class="card-text">
      <span class="badge badge-danger">High-value target</span>
      <span class="badge badge-info">Undruggable</span>
    </p>
  </div>
</div>

#### ⏳ NF-κB - Inflammation Master
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">炎症响应转录因子 | Inflammation Master TF</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>激活途径：</strong>
      <ul>
        <li>经典途径：TNFα/IL-1β → IKK → p65/p50核转位</li>
        <li>非经典途径：BAFF/CD40L → NIK → p52/RelB</li>
      </ul>
      <strong>功能：</strong>免疫应答、炎症、细胞存活<br>
      <strong>疾病相关：</strong>慢性炎症、癌症、自身免疫病
    </p>
  </div>
</div>

---

### 2. 染色质重塑复合体 | Chromatin Remodeling Complexes

#### ⏳ SWI/SNF Complex
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">ATP依赖染色质重塑酶 | ATP-Dependent Remodeler</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>核心亚基：</strong>
      <ul>
        <li><strong>BRG1/BRM:</strong> ATPase催化亚基</li>
        <li><strong>BAF/PBAF:</strong> 不同组装形式</li>
      </ul>
      <strong>功能：</strong>
      <ul>
        <li>核小体滑动与弹出</li>
        <li>转录激活与抑制</li>
        <li>DNA修复辅助</li>
      </ul>
      <strong>临床意义：</strong>20%癌症有SWI/SNF亚基突变
    </p>
  </div>
</div>

#### ⏳ INO80 Complex
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">INO80染色质重塑酶 | INO80 Remodeler</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>特点：</strong>含有RuvB AAA+ ATPase<br>
      <strong>功能：</strong>
      <ul>
        <li>DNA双链断裂修复</li>
        <li>复制叉保护</li>
        <li>转录调控</li>
      </ul>
    </p>
  </div>
</div>

---

### 3. 组蛋白修饰酶 | Histone Modifying Enzymes

#### ⏳ HAT (Histone Acetyltransferase)
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">组蛋白乙酰化酶 | Histone Acetylation Writer</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>主要家族：</strong>
      <ul>
        <li><strong>p300/CBP:</strong> 转录共激活因子</li>
        <li><strong>GCN5/PCAF:</strong> SAGA复合体成分</li>
        <li><strong>TIP60:</strong> DNA修复相关</li>
      </ul>
      <strong>功能：</strong>乙酰化组蛋白赖氨酸，开放染色质<br>
      <strong>应用：</strong>表观遗传药物靶点
    </p>
  </div>
</div>

#### ⏳ HDAC (Histone Deacetylase)
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">组蛋白去乙酰化酶 | Histone Acetylation Eraser</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>分类：</strong>
      <ul>
        <li><strong>Class I (HDAC1-3, 8):</strong> 核内，辅阻遏</li>
        <li><strong>Class II (HDAC4-7, 9-10):</strong> 核-质穿梭</li>
        <li><strong>Class III (Sirtuins):</strong> NAD+依赖</li>
        <li><strong>Class IV (HDAC11):</strong> 独特催化机制</li>
      </ul>
      <strong>抑制剂：</strong>Vorinostat, Romidepsin (FDA批准抗癌药)
    </p>
  </div>
</div>

#### ⏳ HMT (Histone Methyltransferase)
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">组蛋白甲基化酶 | Histone Methylation Writer</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>主要靶点：</strong>
      <ul>
        <li><strong>H3K4me3:</strong> 活性启动子标记 (SET1/MLL)</li>
        <li><strong>H3K9me3:</strong> 异染色质标记 (SUV39H)</li>
        <li><strong>H3K27me3:</strong> Polycomb沉默 (EZH2)</li>
        <li><strong>H3K36me3:</strong> 基因体标记 (SET2)</li>
      </ul>
      <strong>临床：</strong>EZH2抑制剂治疗淋巴瘤
    </p>
  </div>
</div>

---

### 4. 表观遗传阅读器 | Epigenetic Readers

#### ⏳ BRD4 - Bromodomain Protein
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">乙酰化赖氨酸阅读器 | Acetyl-Lysine Reader</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>功能：</strong>
      <ul>
        <li>识别乙酰化组蛋白</li>
        <li>招募转录延伸复合体</li>
        <li>维持超级增强子活性</li>
      </ul>
      <strong>临床应用：</strong>
      <ul>
        <li><strong>BET抑制剂:</strong> JQ1, OTX015</li>
        <li><strong>适应症:</strong> MYC驱动癌症、炎症</li>
      </ul>
    </p>
  </div>
</div>

#### ⏳ HP1 - Heterochromatin Protein 1
<div class="card mb-3 opacity-75">
  <div class="card-body">
    <h5 class="card-title">
      <span class="text-muted">甲基化赖氨酸阅读器 | Methyl-Lysine Reader</span>
      <span class="badge badge-warning float-right">计划中</span>
    </h5>
    <p class="card-text text-muted">
      <strong>功能：</strong>
      <ul>
        <li>识别H3K9me3</li>
        <li>异染色质形成与扩散</li>
        <li>基因沉默维持</li>
      </ul>
      <strong>相分离：</strong>HP1相分离驱动异染色质组装
    </p>
  </div>
</div>

---

## 研究热点 | Current Trends

### 🔥 液-液相分离（LLPS）
- 转录因子凝聚体的形成与功能
- p53/MYC凝聚体的sequential remodeling
- 相分离对转录burst的影响

### 🧬 组蛋白-转录因子竞争
- 生理浓度与分子拥挤条件下的竞争动态
- 空间限域对结合平衡的影响
- 纳米流体技术研究竞争机制

### 💊 表观遗传疗法
- BET抑制剂优化
- HDAC抑制剂联合治疗
- EZH2抑制剂开发

### 🔬 单细胞表观基因组学
- scATAC-seq: 单细胞染色质可及性
- scChIP-seq: 单细胞组蛋白修饰
- 多组学整合

---

## 技术方法 | Research Methods

<div class="row">
  <div class="col-md-6">
    <h4>🔬 功能研究</h4>
    <ul>
      <li><strong>ChIP-seq:</strong> 全基因组结合位点</li>
      <li><strong>ATAC-seq:</strong> 染色质可及性</li>
      <li><strong>CUT&RUN:</strong> 低细胞量表观基因组</li>
      <li><strong>Luciferase assay:</strong> 转录活性</li>
    </ul>
  </div>
  <div class="col-md-6">
    <h4>🧪 机制研究</h4>
    <ul>
      <li><strong>LLPS assays:</strong> 相分离行为</li>
      <li><strong>FRET/FRAP:</strong> 动态与流动性</li>
      <li><strong>Nanofluidics:</strong> 空间限域研究</li>
      <li><strong>Cryo-EM:</strong> 复合物结构</li>
    </ul>
  </div>
</div>

---

## 学习资源 | Learning Resources

### 综述推荐
1. Lambert et al. (2018) *Cell* - 转录因子全面综述
2. Sabari et al. (2020) *Nat Rev Mol Cell Biol* - 转录凝聚体
3. Dawson & Kouzarides (2012) *Cell* - 表观遗传药物

### 数据库
- [JASPAR](https://jaspar.genereg.net/) - 转录因子结合位点
- [Cistrome](http://cistrome.org/) - ChIP-seq数据库
- [ENCODE](https://www.encodeproject.org/) - 表观基因组数据

---

<div class="alert alert-warning">
  <strong>🚀 MYC-p53研究计划：</strong>正在开展MYC-p53转录凝聚体sequential remodeling机制研究，将结合体内成像与体外单分子技术。
</div>
