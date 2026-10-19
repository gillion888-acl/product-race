<div align="center">

# 🧭 产品对照看板 · Product Board

**同一套硬约束、同一套评分标准，多个产品同时从零实作，逐项对照。最终标准只有一个：能不能卖出去。**

[![Products](https://img.shields.io/badge/products-6-1e3a5f)](https://github.com/gillion888-acl/product-race)
[![Tests](https://img.shields.io/badge/unit%20tests-376-146b33)](#-各仓库概览)
[![License](https://img.shields.io/badge/license-MIT-64748b)](#-许可证)

</div>

---

## 📋 这是什么

这是一个产品原型的公开对照看板：每一轮有多个产品原型各自从零实作，全部满足同一套硬约束（纯静态可离线、零构建、零 npm 依赖、成熟 UI 元件库本地内嵌、禁止提及任何其他公司或产品），交付物包含**可在线体验的网址、评分依据、一页商业论证**。

每个产品的九维度评分依据，写在各自仓库的品质自评文档里。

## 🏁 第一轮（教育场景）

| 名次 | 产品 | 一句话 | 总分 | 在线体验 |
|:--:|---|---|:--:|---|
| 🥇 | **课迹 CourseTrail** | 资料不出校的课程问答 + 一键交出院系要收的备案包 | **87** | <https://gillion888-acl.github.io/coursetrail/> |
| 🥈 | **题盾 TopicShield** | 把 AI 抄不了的作业设计出来（不检测 AI，只改作业） | **82.5** | <https://gillion888-acl.github.io/topicshield/> |
| 🥉 | **捡分 Exam Sprint** | 把课件变成会考你的题，每题都指回原文那一段 | **79.5** | <https://gillion888-acl.github.io/exam-sprint/> |

> **本轮结论**：技术最强的没有赢。工程最完整的「捡分」输在选了一个免费大厂正在打的赛道；赢的「课迹」卖的不是问答功能，而是院系能收、能核、能存档的交付物。

## 🏁 第二轮（非教育场景）

| 产品 | 一句话 | 在线体验 |
|---|---|---|
| **标前自检 BidCheck** | 投标截止前 30 分钟，把会废标的坑逐条查一遍 | <https://gillion888-acl.github.io/bid-check/> |
| **车间质检本 Shopfloor QC** | 车间没网络，也能一笔一笔记下检验、事后追溯 | <https://gillion888-acl.github.io/shopfloor-qc/> |
| **交屋证据包 MoveIn Proof** | 入住花 10 分钟留证，退租不吵押金 | <https://gillion888-acl.github.io/move-in-proof/> |

> **为什么开这一轮**：上一轮三个产品都落在教育场景，那是被第一个分析对象锚定的结果。这一轮刻意换成校园之外、买方更具体的场景，用来检验「痛感强度」与「决策链长度」对成不成得了生意的影响。

## 📊 各仓库概览

| 产品 | 技术栈 | 单元测试 | 仓库 |
|---|---|:--:|---|
| 课迹 CourseTrail | Vue 3 + Element Plus | 35 | <https://github.com/gillion888-acl/coursetrail> |
| 题盾 TopicShield | Vue 3 + Element Plus | 29 | <https://github.com/gillion888-acl/topicshield> |
| 捡分 Exam Sprint | Vue 3 + Element Plus | 81 | <https://github.com/gillion888-acl/exam-sprint> |
| 标前自检 BidCheck | Vue 3 + Element Plus | 52 | <https://github.com/gillion888-acl/bid-check> |
| 车间质检本 Shopfloor QC | Vue 3 + Element Plus | 78 | <https://github.com/gillion888-acl/shopfloor-qc> |
| 交屋证据包 MoveIn Proof | 原生 JS + IndexedDB | 101 | <https://github.com/gillion888-acl/move-in-proof> |

## 📊 评分标准（九维度，满分 100）

| 维度 | 权重 | 看什么 |
|---|:--:|---|
| 产品选题 | 15 | 痛点是否真实、是否已被占满、时机对不对、有无外部证据 |
| 产品方向 | 10 | 定位是否锐利、差异化撑不撑得住「为什么不用免费的」 |
| 产品能力 | 15 | 核心能力深度、可解释性、边界与退化处理 |
| 产品质量 | 10 | 可用性、完成度、空／载入／错误态、响应式、键盘 |
| 产品代码 | 10 | 分层、纯函数、零依赖、测试与断言、可维护 |
| 代码描述精确性 | 10 | 命名与注释、文档与实现一致性、有无占位与残留 |
| 市场 | 15 | 买方是否具体、定价是否有支撑、第一单是否可执行 |
| GitHub 传播面 | 10 | 描述、topics、README 排版、截图、体验入口、授权 |
| 风险与诚实度 | 5 | 是否主动揭露「看起来有但没验证」的部分 |

## 🔁 赛制

- **硬约束统一**：纯静态、可离线、零构建、零 npm 依赖、UI 元件库本地内嵌、示例数据自撰、不提及任何其他公司或产品。
- **交付统一**：线上可体验 + `README.md`（产品文档）+ `pitch.md`（一页商业论证）+ 品质自评文档（评分依据）。
- **晋级与淘汰**：连续两轮在「市场」与「选题」两维度低于 10/15 的方向淘汰，不再投入。
- **每一轮都做全链路审核**：从选题、方向、能力、质量、代码、文档、市场到传播面，逐项打分并公开。

## ✅ 怎么审核这些产品

1. 打开任意产品的**在线体验**，点首屏那颗主按钮（每个产品都有「用示例数据试一次」），十秒内能看到核心价值。
2. 看它的**常见问题**与已知限制——每个产品都在 README 里主动写了自己的边界与做不到的事。
3. 读 `pitch.md`（一页商业论证）：目标客户、替代做法与成本、定价、第一单怎么拿。
4. 读仓库里的品质自评：九维度得分与依据。

## 📄 许可证

本仓库内容（看板文档与首页）采用 [MIT License](https://opensource.org/licenses/MIT)。各产品仓库各自附带许可证。

---

<div align="center">

**评分与审核**：由产品负责人执行

所有产品均为独立实作，未包含任何第三方产品的代码或素材；示例资料与文档模板为原创内容。

</div>
