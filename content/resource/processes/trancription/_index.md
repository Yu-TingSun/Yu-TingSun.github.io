---
title: "p53 - 基因组守护者 | Guardian of the Genome"
date: 2025-11-15
draft: true  
---

<!-- 语言切换按钮 -->
<div class="lang-toggle">
  <button onclick="toggleLanguage('both')" class="active">🌐 双语显示 Both</button>
  <button onclick="toggleLanguage('zh')">🇨🇳 仅中文 Chinese Only</button>
  <button onclick="toggleLanguage('en')">🇬🇧 仅英文 English Only</button>
</div>

<script>
function toggleLanguage(lang) {
  const section = document.querySelector('.bilingual-section') || document.body;
  const buttons = document.querySelectorAll('.lang-toggle button');
  
  // 移除所有active类和hide类
  section.classList.remove('hide-zh', 'hide-en');
  buttons.forEach(b => b.classList.remove('active'));
  
  // 应用选择
  if (lang === 'zh') {
    section.classList.add('hide-en');
    buttons[1].classList.add('active');
  } else if (lang === 'en') {
    section.classList.add('hide-zh');
    buttons[2].classList.add('active');
  } else {
    buttons[0].classList.add('active');
  }
  
  // 保存偏好到localStorage
  localStorage.setItem('preferred-language', lang);
}

// 页面加载时恢复用户偏好
document.addEventListener('DOMContentLoaded', function() {
  const preferred = localStorage.getItem('preferred-language');
  if (preferred && preferred !== 'both') {
    toggleLanguage(preferred);
  }
});
</script>

<!-- 主要内容区域 -->
<div class="bilingual-section">

<!-- 第1段：结构域总览 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

## 结构域组成

**功能速览：**

- **TAD (1-67):** 招募转录机器，驱动相分离
- **PRD (67-98):** 蛋白白相互作用，调控凋亡
- **DBD (98-303):** 特异性DNA识别，突变热点区域
- **Linker (303-323):** 柔性连接，允许构象变化
- **TD (323-363):** 形成稳定四聚体
- **CTD (363-393):** 负调控DNA结合，翻译后修饰

  </div>
  
  <div class="bilingual-divider"></div>
  
  <div class="lang-en-block">

## Domain Architecture

**Function Overview:**

- **TAD (1-67):** Recruits transcriptional machinery, drives phase separation
- **PRD (67-98):** Protein interactions, regulates apoptosis
- **DBD (98-303):** Specific DNA recognition, mutation hotspot region
- **Linker (303-323):** Flexible connection, allows conformational changes
- **TD (323-363):** Forms stable tetramers
- **CTD (363-393):** Negatively regulates DNA binding, post-translational modifications

  </div>
</div>

<!-- 第2段：TAD详解 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 1️⃣ TAD - 转录激活域 (1-67 aa)

TAD是p53的转录激活核心，负责招募转录共激活因子和通用转录因子。TAD分为两个子域：

**TAD1 (1-40 aa):**
- 主要的转录激活区域
- 包含关键的酸性和疏水性氨基酸残基
- 结合p300/CBP组蛋白乙酰转移酶
- 磷酸化位点：Ser15（ATM/ATR磷酸化），Thr18, Ser20

**TAD2 (40-67 aa):**
- 辅助激活区域，增强TAD1功能
- 结合TFIID复合体中的TAFII31/TAFII70
- 磷酸化位点：Ser46（促凋亡基因激活）

**相分离特性：**

TAD富含芳香族氨基酸（Phe, Tyr, Trp），这些残基通过π-π相互作用驱动p53的液-液相分离（LLPS），形成转录凝聚体。

**翻译后修饰：**
- **磷酸化：** 响应DNA损伤，阻断MDM2结合
- **乙酰化：** 增强DNA结合和转录活性
- **泛素化：** MDM2介导的降解标记

  </div>
  
  <div class="bilingual-divider"></div>
  
  <div class="lang-en-block">

### 1️⃣ TAD - Transactivation Domain (1-67 aa)

TAD is the transcriptional activation core of p53, responsible for recruiting transcriptional co-activators and general transcription factors. TAD is divided into two subdomains:

**TAD1 (1-40 aa):**
- Primary transcriptional activation region
- Contains key acidic and hydrophobic amino acid residues
- Binds p300/CBP histone acetyltransferases
- Phosphorylation sites: Ser15 (ATM/ATR phosphorylation), Thr18, Ser20

**TAD2 (40-67 aa):**
- Auxiliary activation region, enhances TAD1 function
- Binds TAFII31/TAFII70 in the TFIID complex
- Phosphorylation site: Ser46 (pro-apoptotic gene activation)

**Phase Separation Properties:**

TAD is rich in aromatic amino acids (Phe, Tyr, Trp), and these residues drive liquid-liquid phase separation (LLPS) of p53 through π-π interactions, forming transcriptional condensates.

**Post-translational Modifications:**
- **Phosphorylation:** Responds to DNA damage, blocks MDM2 binding
- **Acetylation:** Enhances DNA binding and transcriptional activity
- **Ubiquitination:** MDM2-mediated degradation marking

  </div>
</div>

<!-- 第3段：PRD详解 -->
<div class="bilingual-pair">
  <div class="lang-zh-block">

### 2️⃣ PRD - 富脯氨酸域 (67-98 aa)

**结构特点：**
- 含有多个PXXP模体（脯氨酸重复序列）
- 无固定二级结构（内在无序区域）

**主要功能：**
- 结合含SH3结构域的蛋白质
- 调控细胞凋亡信号传导
- 影响p53蛋白稳定性

  </div>
  
  <div class="bilingual-divider"></div>
  
  <div class="lang-en-block">

### 2️⃣ PRD - Proline-Rich Domain (67-98 aa)

**Structural Features:**
- Contains multiple PXXP motifs (proline repeats)
- No fixed secondary structure (intrinsically disordered region)

**Major Functions:**
- Binds proteins containing SH3 domains
- Regulates apoptotic signaling
- Affects p53 protein stability

  </div>
</div>

</div> <!-- End of bilingual-section -->

---
