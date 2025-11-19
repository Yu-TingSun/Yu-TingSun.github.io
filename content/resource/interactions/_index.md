---
title: "DNA-Protein Interaction"
subtitle: "DNA-蛋白质相互作用分类体系"
summary: "系统性总结DNA结合蛋白的结构、功能与研究方法"
date: 2025-11-15
type: widget_page
headless: false
draft: true  
---

{{< toc >}}

## 概述 | Overview

DNA-蛋白质相互作用是生命活动的核心过程，涉及基因组的复制、修复、重组和转录调控。本资源库系统性整理了参与DNA相互作用的主要蛋白质家族及其研究方法。

DNA-protein interactions are central to life processes, involving genome replication, repair, recombination, and transcriptional regulation. This resource systematically organizes major protein families that interact with DNA and their research methods.

---

## 分类体系 | Classification System

{{< figure src="/images/resource/DNA-Protein.png" caption="DNA-interacting proteins 分类总览" width="100%" >}}

### 📊 三大类蛋白质概览

<div class="table-responsive">
<table class="table table-hover">
  <thead class="thead-light">
    <tr>
      <th width="15%">中文名称</th>
      <th width="20%">英文名称</th>
      <th width="20%">核心功能</th>
      <th width="25%">典型代表</th>
      <th width="20%">主要亚类</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>1️⃣ 结构蛋白</strong></td>
      <td><strong>Structural proteins</strong></td>
      <td>维持DNA或染色质结构的完整性与组织</td>
      <td>Histones, SMC family, CTCF</td>
      <td>
        • DNA-packaging<br>
        • Chromosome architectural<br>
        • Boundary proteins<br>
        • Nuclear scaffold
      </td>
    </tr>
    <tr>
      <td><strong>2️⃣ 酶类蛋白</strong></td>
      <td><strong>Enzymatic proteins</strong></td>
      <td>执行化学反应：复制、修复、重组、拓扑变化、修饰</td>
      <td>DNA Pol, Ligase, RecA/Rad51, Topoisomerase, DNMT</td>
      <td>
        • Replication enzymes<br>
        • Repair enzymes<br>
        • Recombination enzymes<br>
        • Topoisomerases<br>
        • Modification enzymes
      </td>
    </tr>
    <tr>
      <td><strong>3️⃣ 调控蛋白</strong></td>
      <td><strong>Regulatory proteins</strong></td>
      <td>控制基因表达或染色质状态</td>
      <td>p53, MYC, SWI/SNF, HAT/HDAC, BRD4</td>
      <td>
        • Transcription factors<br>
        • Chromatin remodelers<br>
        • Histone modifiers<br>
        • Epigenetic readers<br>
        • Co-regulators
      </td>
    </tr>
  </tbody>
</table>
</div>

### 🌳 详细分类树状图

<div style="background: #f8f9fa; padding: 20px; border-radius: 8px; font-family: 'Monaco', 'Courier New', monospace; font-size: 0.9em; line-height: 1.8;">
<strong>DNA-interacting proteins</strong><br>
├── <span style="color: #4ECDC4;">I. Structural proteins</span><br>
│   ├── DNA-packaging proteins → <a href="structural/histones/">Histones</a><br>
│   ├── Chromosome architectural proteins → SMC1–6, Cohesin, Condensin<br>
│   ├── Boundary proteins → <a href="structural/#ctcf">CTCF</a><br>
│   └── Nuclear scaffold proteins → Lamin A/C<br>
│<br>
├── <span style="color: #FFD93D;">II. Enzymatic proteins</span><br>
│   ├── DNA replication enzymes → Pol α/δ/ε, MCM<br>
│   ├── DNA repair enzymes → Ligase, PARP, Rad50<br>
│   ├── DNA recombination enzymes → <a href="enzymatic/reca-rad51/">RecA, Rad51, Dmc1</a><br>
│   ├── DNA topoisomerases → Topo I/II<br>
│   └── DNA modification enzymes → DNMT, TET<br>
│<br>
└── <span style="color: #FF6B9D;">III. Regulatory proteins</span><br>
    ├── Transcription factors → <a href="regulatory/p53/">p53</a>, MYC, NF-κB<br>
    ├── Chromatin remodelers → SWI/SNF, INO80<br>
    ├── Histone modifiers → HAT, HDAC, HMT<br>
    ├── Epigenetic readers → BRD4, HP1<br>
    ├── Co-regulators → Mediator, p300/CBP<br>
    └── 3D chromatin organizers → CTCF, Cohesin
</div>

---

## 蛋白质分类 | Protein Classification

<div class="row">
  <div class="col-lg-4 mb-4">
    <div class="card h-100 shadow-sm hover-card">
      <div class="card-body text-center">
        <div class="category-icon mb-3" style="font-size: 3rem; color: #4ECDC4;">
          🏗️
        </div>
        <h3 class="card-title">
          <a href="structural/" style="text-decoration: none; color: inherit;">
            结构蛋白<br>Structural Proteins
          </a>
        </h3>
        <p class="card-text text-muted">
          维持染色体结构与高级组装<br>
          <small>Maintain chromosome structure and higher-order organization</small>
        </p>
        <div class="mt-3">
          <span class="badge badge-info">4 protein families</span>
          <span class="badge badge-success">2 completed</span>
        </div>
        <ul class="list-unstyled text-left mt-3 small">
          <li>✓ Histones</li>
          <li>✓ H-NS</li>
          <li>⏳ SMC family</li>
          <li>⏳ CTCF</li>
        </ul>
        <a href="structural/" class="btn btn-outline-primary btn-sm mt-2">
          查看详情 →
        </a>
      </div>
    </div>
  </div>

  <div class="col-lg-4 mb-4">
    <div class="card h-100 shadow-sm hover-card">
      <div class="card-body text-center">
        <div class="category-icon mb-3" style="font-size: 3rem; color: #FFD93D;">
          ⚙️
        </div>
        <h3 class="card-title">
          <a href="enzymatic/" style="text-decoration: none; color: inherit;">
            酶类蛋白<br>Enzymatic Proteins
          </a>
        </h3>
        <p class="card-text text-muted">
          催化DNA代谢相关反应<br>
          <small>Catalyze DNA metabolic reactions</small>
        </p>
        <div class="mt-3">
          <span class="badge badge-info">5 protein families</span>
          <span class="badge badge-success">1 completed</span>
        </div>
        <ul class="list-unstyled text-left mt-3 small">
          <li>✓ RecA/Rad51/Dmc1</li>
          <li>⏳ DNA Polymerase</li>
          <li>⏳ DNA Ligase</li>
          <li>⏳ Topoisomerase</li>
          <li>⏳ DNMT</li>
        </ul>
        <a href="enzymatic/" class="btn btn-outline-warning btn-sm mt-2">
          查看详情 →
        </a>
      </div>
    </div>
  </div>

  <div class="col-lg-4 mb-4">
    <div class="card h-100 shadow-sm hover-card">
      <div class="card-body text-center">
        <div class="category-icon mb-3" style="font-size: 3rem; color: #FF6B9D;">
          📊
        </div>
        <h3 class="card-title">
          <a href="regulatory/" style="text-decoration: none; color: inherit;">
            调控蛋白<br>Regulatory Proteins
          </a>
        </h3>
        <p class="card-text text-muted">
          调节基因表达与染色质状态<br>
          <small>Regulate gene expression and chromatin states</small>
        </p>
        <div class="mt-3">
          <span class="badge badge-info">6 protein families</span>
          <span class="badge badge-success">1 completed</span>
        </div>
        <ul class="list-unstyled text-left mt-3 small">
          <li>✓ p53</li>
          <li>⏳ MYC</li>
          <li>⏳ NF-κB</li>
          <li>⏳ SWI/SNF</li>
          <li>⏳ HAT/HDAC</li>
          <li>⏳ BRD4</li>
        </ul>
        <a href="regulatory/" class="btn btn-outline-danger btn-sm mt-2">
          查看详情 →
        </a>
      </div>
    </div>
  </div>
</div>

---

## 研究方法 | Research Methods

### 单分子技术 | Single-Molecule Techniques
- **TIRF**: Total Internal Reflection Fluorescence
- **FRET**: Förster Resonance Energy Transfer
- **CoSMoS**: Co-localization Single-Molecule Spectroscopy
- **AFM**: Atomic Force Microscopy

### 生化分析 | Biochemical Analysis
- **EMSA**: Electrophoretic Mobility Shift Assay
- **ChIP-seq**: Chromatin Immunoprecipitation Sequencing
- **Pull-down Assay**

### 结构生物学 | Structural Biology
- **X-ray Crystallography**
- **Cryo-EM**: Cryo-Electron Microscopy
- **NMR**: Nuclear Magnetic Resonance

---
<style>
.hover-card {
  transition: all 0.3s ease;
  border: none;
}
.hover-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 15px rgba(0,0,0,0.2) !important;
}
.category-icon {
  animation: float 3s ease-in-out infinite;
}
@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}
</style>
