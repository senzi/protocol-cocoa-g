# Deep Sleep Protocol: Cocoa-G (DSP-01)

![Build Status](https://img.shields.io/badge/build-passing-success) ![Version](https://img.shields.io/badge/version-1.0.2-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![Target](https://img.shields.io/badge/target-Deep_Sleep-purple)

> **"Cooling the brain, flattening the glucose curve."**
> A bio-optimized hot cocoa formulation leveraging **Glycine** as a primary payload for enhanced sleep architecture.

## 📖 Abstract

**Protocol Cocoa-G** 是 "Sleep Fuzzing" 项目的一部分。这是一个针对夜间睡眠质量优化的热饮配方标准化协议。

主要目的是解决传统热可可配方中（如 `Cocoa-Condensed-Milk-v0.9`）存在的**高血糖波动** (Glucose Spikes) 和**皮质醇反弹** (Cortisol Rebound) 问题，同时引入 **甘氨酸 (Glycine)** 作为核心助眠剂，以物理降低核心体温，诱导 Delta 波（深睡）的产生。

## ⚠️ Problem Statement (The "Bug")

在早期的测试版本中，使用了 **炼乳 (Condensed Milk)** 作为甜味剂和增稠剂。经监测，该依赖项会导致以下运行时错误：

* **Issue #1:** 入睡前血糖飙升，诱发胰岛素大量分泌。
* **Issue #2:** 凌晨 03:00 左右出现反应性低血糖，触发肾上腺素/皮质醇分泌（"Cortisol Awakening Response"），导致用户惊醒且无法回滚（难以复睡）。
* **Issue #3:** 生长激素（HGH）分泌受抑制。

## 🛠️ The Solution (Patch v1.0)

本版本 (v1.0.2) 进行了以下重构：

1.  **Deprecated**: 移除 `Condensed Milk` (炼乳) 依赖。
2.  **Feature**: 引入 `Pure Glycine` (纯甘氨酸粉) 3000mg - 5000mg。
    * **甜味替代**：提供清爽甜味，掩盖可可苦味。
    * **体温调节**：促进血管舒张，降低核心体温。
    * **神经抑制**：拮抗兴奋性神经递质。
3.  **Optimization**: 优化了 `Raw Cocoa Powder` (生可可粉) 的溶解算法（SOP）。

## 📦 BOM (Bill of Materials)

| Component | Quantity | Role | Notes |
| :--- | :--- | :--- | :--- |
| **A2 Milk Powder** | 25g - 30g | Base / Tryptophan | A2 beta-casein reduces GI stress. |
| **Raw Cocoa Powder** | 5g (1.5 tsp) | Magnesium / Flavor | Natural source of Mg. |
| **NOW Foods Glycine** | **3g - 5g** | **Main Payload** | **DO NOT EXCEED 10g without testing.** |
| **Hot Water** | 250ml | Solvent | Target temp: 60°C. |
| **Sea Salt** | 1 pinch | Electrolyte | Flavor enhancer (Optional). |

## ⚙️ Usage / Deployment (SOP)

为了确保生化反应的一致性，请严格遵守以下构建步骤：

### Phase 1: Dry Mix (预混)
在容器中混合 **Glycine** 和 **Cocoa Powder**。
> *Dev Note: 甘氨酸颗粒充当磨料，可有效打散疏水的可可粉，防止结块。*

### Phase 2: Paste (糊化)
加入少量温水 (20ml)，快速搅拌直至形成深褐色浆液 (Chocolate Paste)。

### Phase 3: Fusion (融合)
加入 **A2 Milk Powder**，随后冲入剩余热水。充分搅拌。

### Phase 4: Runtime (运行)
在预计睡眠时间 (Bedtime) 前 **45-60 分钟** 饮用。

## 📊 Expected Results

成功部署后，预期数据如下：

* **Latency**: 入睡潜伏期缩短 (< 15 min)。
* **Deep Sleep**: 深度睡眠时长占比提升 (目标 > 20%)。
* **Heart Rate**: 夜间静息心率呈平滑下降曲线 ("Hammock Shape")。

## 📝 Changelog

* **v1.0.2**
    * Updated README documentation.
    * Standardized the SOP for better solubility.
* **v1.0.0**
    * Initial release of Glycine-based protocol.
    * Removed condensed milk.

## ⚖️ Disclaimer

* **Not Medical Advice**: 本项目仅为个人生活黑客实验 (Bio-hacking experiment)，不构成医疗建议。
* **Dependence**: 个体差异存在，请根据自身 Oura/Apple Watch 数据调整参数。

---
*Maintained by the Sleep Fuzzing Team.*