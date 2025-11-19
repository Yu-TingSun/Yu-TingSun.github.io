---
title: "Histones - 核小体核心蛋白"
subtitle: "DNA包装的基本单位"
summary: "组蛋白是真核生物DNA包装的核心蛋白，147 bp DNA缠绕组蛋白八聚体形成核小体"
date: 2025-01-15
authors: ["Yu-Ting Sun"]
tags: ["Structural", "Nucleosome", "Epigenetics", "Chromatin"]
categories: ["DNA-Protein Interaction", "Structural Proteins"]
featured: true

# Featured image
image:
  caption: 'Nucleosome structure (PDB: 1AOI)'
  focal_point: "Center"
  preview_only: false
---

{{< toc >}}

## 基本信息 | Basic Information

<div class="row">
  <div class="col-md-6">
    <h4>蛋白信息</h4>
    <ul class="list-unstyled">
      <li><strong>分类：</strong>Structural Proteins → DNA-packaging</li>
      <li><strong>物种：</strong>真核生物 (Universal)</li>
      <li><strong>功能：</strong>DNA包装、表观遗传调控</li>
      <li><strong>研究进展：</strong>⭐⭐⭐⭐⭐</li>
    </ul>
  </div>
  <div class="col-md-6">
    <h4>核小体组成</h4>
    <ul class="list-unstyled">
      <li><strong>核心组蛋白：</strong>H2A, H2B, H3, H4 (各2个)</li>
      <li><strong>连接组蛋白：</strong>H1/H5</li>
      <li><strong>DNA长度：</strong>147 bp (核心) + 20-80 bp (连接)</li>
      <li><strong>总分子量：</strong>~200 kDa</li>
    </ul>
  </div>
</div>

---

## 结构特征 | Structure

### 核小体核心颗粒 (Nucleosome Core Particle, NCP)

{{< figure src="nucleosome-structure.png" caption="核小体晶体结构 (Luger et al. 1997, Nature)" width="600px" >}}

**关键结构特点：**
1. **组蛋白八聚体：**
   - (H3-H4)₂四聚体位于中心
   - 两个H2A-H2B二聚体位于两侧
   - 组蛋白折叠为"histone fold"结构域

2. **DNA缠绕：**
   - 147 bp DNA左旋缠绕1.65圈
   - 每圈约10 bp，形成超螺旋
   - 14个DNA-组蛋白接触点

3. **组蛋白尾部：**
   - N端和C端无序区域伸出核心
   - 富含赖氨酸和精氨酸（正电荷）
   - 翻译后修饰的主要位点

```
结构层次：
DNA (2 nm) 
  → 核小体 (11 nm)
    → 30 nm 染色质纤维
      → 更高级结构
        → 染色体 (1400 nm)
```

---

## 功能机制 | Function & Mechanism

### 1. DNA包装压缩

**压缩比：**
- 核小体水平：6-7倍 (200 bp → 30 nm纤维)
- 染色质纤维：~40倍
- 有丝分裂染色体：~10,000倍

### 2. 基因表达调控

**两种状态：**

| 特征 | 活性染色质 (Euchromatin) | 沉默染色质 (Heterochromatin) |
|------|------------------------|---------------------------|
| 核小体密度 | 低 | 高 |
| 组蛋白修饰 | H3K4me3, H3K27ac | H3K9me3, H3K27me3 |
| DNA可及性 | 高 | 低 |
| 转录活性 | 活跃 | 抑制 |

### 3. 表观遗传记忆

**组蛋白变体：**
- **H3.3：** 转录活跃区域
- **CENP-A：** 着丝粒特异性
- **H2A.Z：** 启动子区域，调控边界
- **macroH2A：** X染色体失活

**组蛋白修饰（Histone code）：**
- **乙酰化 (ac)：** 激活转录
- **甲基化 (me)：** 激活或抑制（取决于位点）
- **磷酸化 (ph)：** DNA损伤信号
- **泛素化 (ub)：** 转录延伸

---

## 动态调控 | Dynamic Regulation

### 核小体重塑 | Nucleosome Remodeling

**ATP依赖染色质重塑复合体：**

<div class="row">
  <div class="col-md-6">
    <h5>SWI/SNF家族</h5>
    <ul>
      <li>核小体滑动</li>
      <li>核小体弹出</li>
      <li>转录激活</li>
    </ul>
  </div>
  <div class="col-md-6">
    <h5>CHD家族</h5>
    <ul>
      <li>核小体间距调整</li>
      <li>组蛋白变体交换</li>
      <li>转录和修复</li>
    </ul>
  </div>
</div>

### 组蛋白伴侣 | Histone Chaperones

- **CAF-1：** 复制偶联的组装
- **HIRA：** 复制非依赖的H3.3沉积
- **NAP1：** 核小体组装/去组装
- **FACT：** 转录过程中的重组装

---

## 研究方法 | Research Methods

### 生化技术
```yaml
EMSA (Electrophoretic Mobility Shift Assay):
  用途: 核小体组装效率
  优势: 定量、简单
  限制: 体外条件

MNase-seq (Micrococcal Nuclease Sequencing):
  用途: 全基因组核小体定位
  分辨率: ~150 bp
  应用: 表观基因组图谱

ChIP-seq:
  用途: 组蛋白修饰和变体定位
  特点: 特异性抗体依赖
  数据: ENCODE, Roadmap Epigenomics
```

### 单分子技术

{{< figure src="single-molecule-methods.png" caption="单分子研究核小体动态" width="700px" >}}

**1. FRET (Förster Resonance Energy Transfer)**
- 测量核小体展开/缠绕动态
- 监测组蛋白-DNA相互作用变化
- 实时观察重塑酶活性

**实验示例：**
```
Donor (Cy3) 标记 H2A
Acceptor (Cy5) 标记 DNA
↓
E_FRET = 0.7 (紧密缠绕)
E_FRET = 0.3 (部分展开)
E_FRET = 0 (完全解离)
```

**2. Optical Tweezers (光镊)**
- 测量核小体解旋所需力 (~20 pN)
- 核小体稳定性定量
- 重塑酶机械学研究

**3. AFM (Atomic Force Microscopy)**
- 核小体阵列的高分辨率成像
- 30 nm纤维结构
- DNA-蛋白复合物形貌

### 结构生物学

**X-ray Crystallography:**
- 1997年首个核小体结构 (Luger et al., Nature)
- 分辨率: 1.9 Å
- 限制: 静态结构

**Cryo-EM:**
- 核小体与重塑酶复合物
- 染色质纤维结构
- 分辨率: 3-4 Å
- 优势: 更接近生理状态

---

## 生理与病理意义 | Physiological & Pathological Significance

### 正常生理功能
- **细胞周期：** 核小体组装与传代
- **DNA修复：** 核小体去稳定化促进修复
- **发育调控：** 组蛋白变体介导分化
- **X染色体失活：** macroH2A富集

### 疾病相关

<div class="alert alert-danger">
<h5>癌症</h5>
<ul>
  <li><strong>组蛋白突变：</strong>H3K27M (儿童脑肿瘤), H3.3G34R/V (骨肉瘤)</li>
  <li><strong>染色质重塑缺陷：</strong>20%癌症有SWI/SNF突变</li>
  <li><strong>表观遗传失调：</strong>EZH2过表达导致H3K27me3异常</li>
</ul>
</div>

<div class="alert alert-warning">
<h5>神经退行性疾病</h5>
<ul>
  <li>阿尔茨海默病中的组蛋白乙酰化减少</li>
  <li>HDAC抑制剂的神经保护作用</li>
</ul>
</div>

---

## 治疗靶点 | Therapeutic Targets

### 表观遗传药物

| 药物类型 | 代表药物 | 靶点 | 适应症 |
|---------|---------|------|--------|
| HDAC抑制剂 | Vorinostat, Romidepsin | HDAC1-11 | T细胞淋巴瘤 |
| EZH2抑制剂 | Tazemetostat | EZH2 | 滤泡性淋巴瘤 |
| BET抑制剂 | JQ1, OTX015 | BRD4 | 多种癌症（临床试验） |
| LSD1抑制剂 | ORY-1001 | LSD1/KDM1A | 急性白血病 |

### 联合治疗策略
- HDAC抑制剂 + 化疗
- BET抑制剂 + 免疫检查点抑制剂
- 表观遗传重编程 + 分化疗法

---

## 研究进展与前沿 | Recent Advances

### 🔥 2020-2025 重要发现

1. **相分离与染色质组织** (Science 2020)
   - HP1相分离驱动异染色质形成
   - 组蛋白修饰调控相分离行为

2. **核小体呼吸动力学** (Nature 2021)
   - 核小体自发展开-缠绕（呼吸）
   - 平均寿命 ~250 ms (体外)
   - 转录因子利用呼吸瞬间结合

3. **CUT&Tag技术革新** (Nature Biotechnology 2019)
   - 低至100细胞的表观基因组分析
   - 无需交联和超声破碎
   - 更高信噪比

4. **组蛋白-p53竞争机制** (进行中)
   - 生理拥挤条件下的竞争动态
   - 纳米流体单分子研究
   - 相分离对竞争的影响

---

## 相关蛋白 | Related Proteins

<div class="row">
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">染色质重塑酶</h5>
        <ul class="small">
          <li><a href="../../regulatory/swi-snf/">SWI/SNF</a></li>
          <li><a href="../../regulatory/ino80/">INO80</a></li>
          <li>CHD family</li>
          <li>ISWI family</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">组蛋白修饰酶</h5>
        <ul class="small">
          <li><a href="../../regulatory/hat/">HAT</a></li>
          <li><a href="../../regulatory/hdac/">HDAC</a></li>
          <li><a href="../../regulatory/hmt/">HMT</a></li>
          <li>HDM (去甲基化酶)</li>
        </ul>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">转录因子</h5>
        <ul class="small">
          <li><a href="../../regulatory/p53/">p53</a></li>
          <li><a href="../../regulatory/myc/">MYC</a></li>
          <li>Nuclear receptors</li>
          <li>Pioneer factors</li>
        </ul>
      </div>
    </div>
  </div>
</div>

---

## 参考文献 | References

### 开创性工作
1. **Luger et al. (1997)** *Nature* 389:251-260
   - 首个核小体晶体结构 (1.9 Å)
   - PDB: 1AOI

2. **Kornberg & Lorch (1999)** *Cell* 98:285-294
   - 核小体与转录调控综述

### 近期综述
3. **Fyodorov et al. (2018)** *Nat Rev Mol Cell Biol* 19:192-206
   - 核小体机制与功能

4. **Zhou et al. (2019)** *Genes Dev* 33:1619-1634
   - 组蛋白变体功能

5. **Peng & Karpen (2023)** *Nat Rev Genet* 24:183-198
   - 染色质三维结构

### 方法学
6. **Kaya-Okur et al. (2019)** *Nat Protoc* 14:2264-2283
   - CUT&Tag protocol

---

## 扩展资源 | Additional Resources

### 在线工具
- [NucPlot](http://www.nucleosome.org/) - 核小体结构可视化
- [Histone Database](https://www.actrec.gov.in/histome/) - 组蛋白修饰数据库
- [ENCODE](https://www.encodeproject.org/) - ChIP-seq和MNase-seq数据

### 教学视频
- [iBiology - Nucleosome Structure and Function](https://www.youtube.com/watch?v=xxx)
- [HHMI BioInteractive - Epigenetics](https://www.biointeractive.org/classroom-resources/epigenetics)

---

<div class="alert alert-success">
  <strong>✅ 本页面状态：</strong>已完成 | Last updated: 2025-01-15
</div>
