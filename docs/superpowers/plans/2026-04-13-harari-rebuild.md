# Harari Skill Rebuild Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rebuild `jazzqi/harari-skill` into a full Nuwa-style, research-backed Harari perspective skill focused on civilization history, narrative power, and technology/AI.

**Architecture:** Keep the existing repository shape, but replace the thin evidence chain with six dedicated research documents, then regenerate `SKILL.md`, `README.md`, and `examples/demo-conversation.md` from that research. Validate the rebuilt skill with baseline-vs-rebuilt pressure scenarios so the repo ships a stronger research-first Harari voice instead of a quote-driven macro-history shell.

**Tech Stack:** Markdown, Git, GitHub, Copilot CLI subagents, web/GitHub retrieval tools

---

## File Structure

- Modify: `SKILL.md`
- Modify: `README.md`
- Modify: `examples/demo-conversation.md`
- Create or replace: `references/research/01-writings.md`
- Create or replace: `references/research/02-conversations.md`
- Create or replace: `references/research/03-expression-dna.md`
- Create or replace: `references/research/04-external-views.md`
- Create or replace: `references/research/05-decisions.md`
- Create or replace: `references/research/06-timeline.md`
- Create: `references/research/README.md`
- Create: `docs/superpowers/specs/2026-04-13-harari-rebuild-design.md`
- Create: `docs/superpowers/plans/2026-04-13-harari-rebuild.md`

## Task 1: Capture Baseline Failure Modes

**Files:**
- Modify: `docs/superpowers/plans/2026-04-13-harari-rebuild.md`
- Read: `SKILL.md`
- Read: `README.md`
- Read: `examples/demo-conversation.md`

- [ ] **Step 1: Run a baseline read of the current skill**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
sed -n '1,220p' SKILL.md && \
printf '\n--- README ---\n' && sed -n '1,220p' README.md && \
printf '\n--- EXAMPLE ---\n' && sed -n '1,260p' examples/demo-conversation.md
```

Expected: enough context to identify where the current repo is strong and where it remains template-like.

- [ ] **Step 2: Record the concrete baseline gaps to beat**

Use this checklist:

```markdown
- Research files are not yet a 6-dimension Nuwa evidence base
- Agentic Protocol is mostly fixed-pattern narration, not research-routed behavior
- README and examples do not yet fully prove research-first answering
- Internal tensions and serious outside criticism need stronger preservation
- Recent-12-month signal and timeline staging need explicit treatment
```

- [ ] **Step 3: Treat these baseline gaps as the failing test**

Pass condition for the rebuild:

```markdown
The rebuilt repo must make each baseline gap false:
1. six research files exist and are source-disciplined
2. protocol distinguishes framework vs fact-dependent questions
3. examples include a true research-first path
4. tensions and criticisms are preserved, not smoothed away
5. recent timeline developments are visible and dated
```

- [ ] **Step 4: Commit the planning checkpoint**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
git add docs/superpowers/specs/2026-04-13-harari-rebuild-design.md docs/superpowers/plans/2026-04-13-harari-rebuild.md && \
git commit -m "docs: add harari rebuild plan" -m "Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

Expected: a plan commit exists before content changes begin.

## Task 2: Produce Six Research Documents

**Files:**
- Create or replace: `references/research/01-writings.md`
- Create or replace: `references/research/02-conversations.md`
- Create or replace: `references/research/03-expression-dna.md`
- Create or replace: `references/research/04-external-views.md`
- Create or replace: `references/research/05-decisions.md`
- Create or replace: `references/research/06-timeline.md`
- Create: `references/research/README.md`

- [ ] **Step 1: Launch focused research work**

Dispatch one research track per dimension with this scope:

```markdown
01-writings.md
- Harari books and long essays
- repeated claims appearing 3+ times
- concept inventory: imagined orders, intersubjective reality, dataism, information networks

02-conversations.md
- long podcasts, stage interviews, testimony
- how he reframes pushback
- how he handles over-simplification criticism

03-expression-dna.md
- phrase patterns, cadence, triads, question endings, certainty markers

04-external-views.md
- scholarly criticism, praise, simplification charges, political/elite-platform critique

05-decisions.md
- public positioning choices, major book turns, institutional alignments, policy posture

06-timeline.md
- biography, book phases, career pivot to public intellectual, recent 12-month updates
```

- [ ] **Step 2: Write the research files with explicit source discipline**

Every file must distinguish:

```markdown
- 一手来源：Harari's own books, essays, talks, interviews
- 二手来源：reviews, criticism, analysis
- 推断：clearly marked inference, never presented as direct fact
```

- [ ] **Step 3: Add a research index**

Create `references/research/README.md` with:

```markdown
# Harari Research Index

- 01-writings.md: books and repeated propositions
- 02-conversations.md: interview behavior and improvisation
- 03-expression-dna.md: phrasing and rhetorical structure
- 04-external-views.md: criticism, praise, and unresolved disputes
- 05-decisions.md: action patterns and public choices
- 06-timeline.md: life stages and recent developments
```

- [ ] **Step 4: Verify the research layer exists**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
ls references/research && \
for f in references/research/*.md; do echo "--- $f"; sed -n '1,40p' "$f"; done
```

Expected: all seven research markdown files exist and are non-empty.

- [ ] **Step 5: Commit the research layer**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
git add references/research && \
git commit -m "docs: rebuild harari research base" -m "Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

## Task 3: Rebuild the Skill Core

**Files:**
- Modify: `SKILL.md`

- [ ] **Step 1: Draft the new section map**

`SKILL.md` should be organized around this skeleton:

```markdown
---
name: harari-perspective
description: Use when ...
---

# [title]

## 角色扮演规则
## 回答工作流（Agentic Protocol）
## 身份卡
## 核心心智模型
## 决策启发式
## 表达 DNA
## 价值观与反模式
## 内在张力
## 时间线
## 诚实边界
## 调研来源
```

- [ ] **Step 2: Replace the fixed protocol with a research-routed protocol**

The protocol must include:

```markdown
### Step 1: 问题分类
- 纯框架问题
- 需要事实的问题
- 混合问题

### Step 2: 赫拉利式研究
- 当前问题依赖什么想象秩序或主体间现实
- 哪些信息网络、媒体结构、算法或制度在塑造结果
- 哪些历史类比真的成立，哪些只是叙事偷懒
- 谁获得了叙事权力 / 数据优势 / 组织优势
- 哪些关键事实仍未知，因而必须降低结论强度

### Step 3: 赫拉利式回答
- 拉长时间轴
- 反直觉重构
- 以开放问题或限制条件收尾
```

- [ ] **Step 3: Rebuild the mental models from research instead of headline memory**

Target shape:

```markdown
3-7 models, each with:
- 名称
- 核心命题
- 至少2类证据来源
- 使用方式
- 局限性
```

Suggested model pool to validate against research:

```markdown
- 想象秩序 / 主体间现实
- 信息网络塑造现实
- 历史中的进步叙事与代价错位
- 算法化的人类与自由意志侵蚀
- 叙事权力决定合作与操控
- 冥想作为去叙事化认识工具
```

- [ ] **Step 4: Add values, anti-patterns, tensions, and boundaries**

Minimum content:

```markdown
价值观
- 认识论诚实
- 对大规模叙事与权力的警觉
- 从物种尺度重新评估当下问题

反模式
- 伪装成必然历史的政治故事
- 用技术效率掩盖权力集中
- 把好故事当作真事实

内在张力
- 宏大叙事能力 vs 学术严谨性质疑
- 警告科技精英风险 vs 身处精英平台
- 公共知识分子姿态 vs 历史预测的不确定性

诚实边界
- 不是技术实现专家
- 不是微观政策细节专家
- 对未来的回答应保持警告式而非预言式
```

- [ ] **Step 5: Review the top of the rebuilt file**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && sed -n '1,260p' SKILL.md
```

Expected: the file reads like a Nuwa rebuild, not a patched summary.

- [ ] **Step 6: Commit the rebuilt core skill**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
git add SKILL.md && \
git commit -m "feat: rebuild harari perspective skill" -m "Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

## Task 4: Rebuild README and Example Conversation

**Files:**
- Modify: `README.md`
- Modify: `examples/demo-conversation.md`

- [ ] **Step 1: Rewrite the README to match the rebuilt architecture**

`README.md` must cover:

```markdown
# harari-perspective

## 这是什么
## 适用问题
## 蒸馏出的核心模型
## 回答工作流
## 对话示例
## 诚实边界
## 调研来源结构
```

- [ ] **Step 2: Rewrite the example file with at least four scenarios**

The example set must include:

```markdown
1. 纯框架问题：例如“民族国家是不是一种虚构？”
2. AI / 信息网络问题：例如“生成式AI会改变民主吗？”
3. 历史叙事问题：例如“农业革命是进步还是陷阱？”
4. research-first问题：例如“赫拉利会怎么看某个当下事件/公司/政策？”
```

- [ ] **Step 3: Make the research-first scenario explicit**

The scenario should visibly show:

```markdown
- 先识别这是事实依赖问题
- 先研究当前事实与信息网络结构
- 再输出赫拉利式判断
- 保留未知项和置信度限制
```

- [ ] **Step 4: Review packaging consistency**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
printf '\n--- README ---\n' && sed -n '1,240p' README.md && \
printf '\n--- EXAMPLE ---\n' && sed -n '1,260p' examples/demo-conversation.md
```

Expected: README, example, and `SKILL.md` describe the same models and workflow.

- [ ] **Step 5: Commit the packaging updates**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
git add README.md examples/demo-conversation.md && \
git commit -m "docs: align harari readme and examples" -m "Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

## Task 5: Verify the Rebuild

**Files:**
- Read: `SKILL.md`
- Read: `README.md`
- Read: `examples/demo-conversation.md`
- Read: `references/research/*.md`

- [ ] **Step 1: Run three pressure checks against the rebuilt repo**

Use these checks:

```markdown
Sanity check:
- compare rebuilt skill behavior to Harari's known public posture on AI / information / imagined orders

Edge check:
- ask a new but adjacent question and ensure the answer says "based on this framework" rather than pretending certainty

Voice check:
- read a short generated-style answer and confirm it sounds like Harari, not generic macro futurism
```

- [ ] **Step 2: Verify the four key rebuild outcomes**

Checklist:

```markdown
- six research files plus research README exist
- protocol clearly routes fact-dependent questions to research
- examples include a real research-first scenario
- criticisms and tensions remain present
```

- [ ] **Step 3: Inspect the final diff**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && git --no-pager diff --stat HEAD~3..HEAD && git --no-pager diff -- README.md SKILL.md examples/demo-conversation.md references/research
```

Expected: the diff is tightly focused on the rebuild deliverables.

- [ ] **Step 4: Commit verification-only fixes if needed**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && \
git add -A && \
git commit -m "fix: tighten harari rebuild consistency" -m "Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>"
```

Expected: skip this commit if no new changes were required.

## Task 6: Push the Rebuilt Repository

**Files:**
- Modify: repository history only

- [ ] **Step 1: Check branch and remote**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && git remote -v && git branch --show-current
```

Expected: `origin` points to `jazzqi/harari-skill` and branch is `main`.

- [ ] **Step 2: Push**

Run:

```bash
cd /Users/qfei/Workspace/harari-skill && git push --set-upstream origin main
```

Expected: GitHub receives the rebuild.

- [ ] **Step 3: Mark SQL todo progression**

Use these transitions:

```sql
UPDATE todos SET status = 'done' WHERE id = 'harari-baseline';
UPDATE todos SET status = 'in_progress' WHERE id = 'harari-research';
UPDATE todos SET status = 'done' WHERE id = 'harari-research';
UPDATE todos SET status = 'in_progress' WHERE id = 'harari-synthesis';
UPDATE todos SET status = 'done' WHERE id = 'harari-synthesis';
UPDATE todos SET status = 'in_progress' WHERE id = 'harari-verify';
UPDATE todos SET status = 'done' WHERE id = 'harari-verify';
UPDATE todos SET status = 'in_progress' WHERE id = 'harari-git';
UPDATE todos SET status = 'done' WHERE id = 'harari-git';
```

Expected: the todo table reflects the real rebuild lifecycle.

