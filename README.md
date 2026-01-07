# 🧬 qPCR PrimerBatch Designer (High-GC Specialized)

### 基于热力学优化的 qPCR 引物批量设计与可视化系统

[![User](https://img.shields.io/badge/Developer-wwp643-0284c7.svg)](https://github.com/wwp643)
[![Field](https://img.shields.io/badge/Field-Molecular%20Biology-red.svg)](https://en.wikipedia.org/wiki/Quantitative_PCR)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📖 项目简介
**qPCR PrimerBatch Designer** 是一款专为复杂基因组研究者开发的轻量化引物设计工具。特别针对以结核分枝杆菌为代表的 **高 GC 含量基因组**（GC > 60%）进行了算法强化，解决了通用引物设计软件在处理此类高难度模板时匹配率低、特异性差的痛点。

本项目采用纯前端架构，无需安装任何后台环境，即可在浏览器中实现从序列输入到位置可视化的完整工作流。

## ✨ 核心优势
* **高 GC 适配算法**：内置宽 $T_m$ 搜索逻辑（支持 55°C - 75°C 区间），在极端序列中寻找热力学平衡点。
* **批量并行处理**：支持同时输入数十条 FASTA 序列，一次性完成全基因组多靶点引物筛选。
* **动态序列地图**：自动渲染引物在模板序列上的物理位置，使用颜色高亮区分 Forward 和 Reverse 绑定区。
* **3' 端稳定性校验**：严格过滤 3' 末端 GC 含量过高的候选，有效降低非特异性扩增和引物二聚体风险。
* **科研数据导出**：结果支持一键复制，格式完美兼容 Excel 等科研记录表格。

## 🚀 快速启动

### 1. 获取项目
```bash
git clone [https://github.com/wwp643/qPCR-Primer-Designer.git](https://github.com/wwp643/qPCR-Primer-Designer.git)
