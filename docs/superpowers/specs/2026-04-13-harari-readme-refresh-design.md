# Harari README Refresh Design

## Problem

当前 `harari-skill/README.md` 已经对齐了新版 research-routed `SKILL.md`，但包装结构仍偏“说明书式”，缺少 `li-lu-skill/README.md` 那种更成熟的仓库首页组织方式：标题定位更强、导航更清晰、效果示例更前置、安装入口更直接。

用户的新要求不是重做 Harari 的研究或 `SKILL.md`，而是**参考 `li-lu-skill` 的 README 结构，重写 Harari 的 README，然后提交**。

## Goal

在不退回旧版浅层角色卡包装的前提下，把 Harari README 改写为：

1. 更接近 `li-lu-skill` 的首页结构；
2. 仍然忠实于 Harari 当前的 research-routed skill 定义；
3. 明确体现 Harari skill 的研究边界、使用方式与高价值问题类型；
4. 与仓库当前已完成的 Harari 全套重建内容（research / `SKILL.md` / examples）保持一致。

## Non-Goals

- 不在本次工作里重写 `SKILL.md`
- 不重新设计 research 文件结构
- 不把 README 改回纯角色扮演导向包装
- 不拆分为只提交 README 的最小 patch；用户已明确同意把当前 Harari 全套改动一起提交

## Reference

结构参考文件：

- `/Users/qfei/Workspace/li-lu-skill/README.md`

内容约束来源：

- `/Users/qfei/Workspace/harari-skill/SKILL.md`
- `/Users/qfei/Workspace/harari-skill/references/research/*.md`

## Proposed Structure

### 1. Header / Positioning

- 仓库名标题
- 一句定位
- 徽章与快速导航（如“看效果 / 安装 / 蒸馏了什么”）

### 2. 效果示例

- 前置 2-3 个短片段
- 形式参考 `li-lu-skill`
- 内容必须体现 Harari 的新版使用方式：
  - 文明尺度重写问题
  - AI / 信息网络 / 民主脆弱性
  - 至少一个边界意识片段

### 3. 安装

- 与 `li-lu-skill` 类似的简洁安装段落
- 补触发式使用示例

### 4. 蒸馏了什么

保留并重组为更适合首页浏览的几个小节：

- 6 个心智模型
- 8 条决策启发式
- 表达 DNA
- 3-4 对关键张力

### 5. 诚实边界

- 调研截止时间
- 不能替代实时事实核验
- 不适合窄领域史实裁决、技术审计、法条落地

### 6. 这个 Skill 是怎么造出来的

- 说明女娲蒸馏与 research 基础
- 保留 creator footer

## Design Constraints

1. **结构像李录 README，内容必须像 Harari skill**
2. **首页包装更强，但不能牺牲 research-routed 边界**
3. **README 改完后，提交当前 Harari 全套改动**

## Risks

### 风险 1：参考结构时退回浅层包装

缓解：所有示例与文案都以新版 `SKILL.md` 为准，而不是复用旧 README 的表达。

### 风险 2：README 与 examples / SKILL 不一致

缓解：重写时同步检查核心模型命名、边界表述、研究文件结构。

### 风险 3：提交范围不一致

缓解：本次提交以“当前 Harari 重建全套改动”为单位，而不是只摘出 README。

## Acceptance Criteria

1. README 结构明显向 `li-lu-skill` 靠拢。
2. README 内容与当前 Harari `SKILL.md` 一致。
3. README 明确展示 Harari 的 6 个核心模型与边界意识。
4. 当前 Harari 全套改动可以作为一个 coherent commit 提交。
