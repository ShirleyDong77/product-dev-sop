# Product Development SOP Skill

_A general-purpose product development workflow template._

---

## ⚠️ How to handle a new request from Shirley

When Shirley gives you a new task, follow this exact sequence:

```
Step 1: Research & Assess
↓
Step 2: Report to Shirley — Can we do it?
↓
Step 3: If YES → Create project folder in Feishu wiki root
↓
Step 4: Write 01 Requirements Analysis
↓
Step 5: Review 01 → Approved
↓
Step 6: Write 02 PRD
↓
Step 7: Review 02 → Approved
↓
Continue through Phase 2–7
```

**Step 1 — Research & Assess:**

Do NOT immediately start building. First research:
- Is this worth doing? (Priority × Resources × Value)
- Who is the user? What is the real problem?
- What is the success criteria?

**Step 2 — Report to Shirley:**
Present your assessment:
- Should we do this? Why or why not?
- What resources are needed?
- What is the一期 goal?

Wait for Shirley's decision: "do it" or "stop."

**Step 3 — If "do it":**
Create project folder in Feishu wiki root (like Magazine project did), THEN start 01 Requirements Analysis.

**Step 4 — Write 01 Requirements Analysis:**
See template below. 01 must be reviewed and approved before starting 02 PRD.

**⚠️ Critical rule: You do not skip to building. You research first, report second, create project third.**

---

## What is this skill?

This skill provides a complete 7-phase product development workflow for small to medium-sized projects. It is designed to be adapted to any team or individual.

**Who this is for:**
- Solo builders or small teams shipping projects alone
- Anyone who wants a systematic approach to product development
- Teams transitioning from ad-hoc workflows to structured processes

**What makes this different:**
- Built for asynchronous work (no mandatory meetings)
- Designed around written documentation (not verbal communication)
- Includes compliance checks for external releases
- All templates are ready to copy and use

---

## The 7 Phases

```
Phase 1  Requirements  → PRD + Review
Phase 2  Design       → Design Doc + Review
Phase 3  Development  → Dev Design + Schedule
Phase 4  Testing      → Test Cases + Hands-on Verification
Phase 5  Compliance   → Privacy / Accuracy / Consistency Check
Phase 6  Acceptance  → User Sign-off + Launch Notice + Report
Phase 7  Retrospective → Project + Data Retrospective
```

---

## Phase 1: Requirements

### ⚠️ Phase 1 has TWO required documents

**Phase 1 = 01需求分析 + 02PRD**

**01需求分析必须在02PRD之前完成。**
01未通过评审，不得开始02PRD。

**Why:** Without 01, the PRD lacks problem definition, user scenarios, and success criteria. This is why the Magazine calculator PRD was rejected — I skipped requirements analysis and went straight to PRD.

---

### 01 Requirements Analysis Template

```markdown
# [Project Name] 需求分析 01 v1.0
_Created:_

## 一、用户场景分析

### 场景 1：[描述具体场景]
用户正在……

**用户心理：**
- ……

**用户痛点：**
- ……

## 二、需求根因分析

**表面需求：**
**深层需求：**
**需求本质：**

## 三、竞品分析

| 竞品 | 优点 | 缺点 |
|------|------|------|
| | | |

## 四、成功标准

**功能成功标准：**
**业务成功标准：**
**目标用户：**

## 五、一期目标（v1.0）
[一句话说清楚本期做什么、不做什么]

## 六、后续扩展方向

## 七、与 PRD 的关系
[说明01和02的关系]

---

### 02 PRD Template

```markdown
# [Project Name] PRD v1.0
_Created:_
_Author:_

## Executive Summary
[One page overview: what this project is, why it matters, and what success looks like.]

## Feature List

| ID | Feature | Priority | One-liner |
|----|---------|----------|-----------|
| F-01 | | P0 | |

## Feature Details

### F-01: [Feature Name]

**What it does:**
[Clear description]

**Value to user:**
[What problem does this solve?]

**Acceptance criteria:**
- [How do we know it's done?]
- [Specific, testable conditions]

**Dependencies:**
[What else does this depend on?]

## Non-functional Requirements

- Performance:
- Security:
- Compatibility:
- Compliance:

## Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| | | |

## Review Record

| Date | Reviewer | Decision | Notes |
|------|----------|----------|-------|
| | | | |
```

### Review Process

```
PRD written
    ↓
Share via doc comment @[Reviewer]
    ↓
State "please review, 48hr silence = approved"
    ↓
Reviewer comments
    ↓
Revise
    ↓
Reviewer approves
```

**Decision rules:**
- One decision-maker (assign at start)
- Outcomes: Approved / Rejected / Revise and resubmit
- 48 hours of silence = approved

---

## Phase 2: Design

### Design Doc Template

```markdown
# [Project Name] Design v1.0
_Created:_
_Review Date:_

## Design Links

- **Interactive prototype (HTML):** [link — must be a working HTML page, not a mockup image]
- Visual design: [link — Figma or image]
- Live preview: [link]
```

**⚠️ 重要：设计文档必须包含可运行的 HTML 原型链接，不接受只有文字描述的设计稿。**

## Core User Flow
[Text description of the main user path]

## Pages

| Page | Purpose | Notes |
|------|---------|-------|
| | | |

## Design Decisions

| Decision | Choice | Rationale |
|---------|--------|----------|
| | | |

## Review Issues

| ID | Issue | Priority | Status | Resolution |
|----|-------|----------|--------|------------|
| Q-01 | | P1 | ✅ Resolved | |
| Q-02 | | P0 | 🔄 In progress | |

## Version History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| V1.0 | | | Initial |
```

### Sync to PRD

After design is finalized:
- Copy key design decisions into the PRD
- Add "Design finalized, see [link]" note in PRD
- Keep both documents in sync

---

## Phase 3: Development

### Dev Design Template

```markdown
# [Project Name] Dev Design v1.0

## Technical Approach

## Task Breakdown

| Task | Est. Time | Owner | Status |
|------|-----------|-------|--------|
| | | | |

## Dependencies

## Risks

## Schedule
[Start] → [Milestone 1] → [Milestone 2] → [Launch]
```

---

## Phase 4: Testing

### Test Case Template

```markdown
# [Project Name] Test Cases

## Test Results

| TC | Check | Method | Expected | Result | Date |
|----|-------|--------|----------|--------|------|
| 01 | | | | | |

## Issues Found

| Issue | Root Cause | Fix | Status | Resolved |
|-------|-----------|-----|--------|----------|
| | | | | |

## Conclusion
[ ] Ready to launch / [ ] Needs fixing first
```

### Hands-on Testing Rule

**Test by doing, not by running scripts.**

Open the actual interface. Click through every flow. Do not skip steps.

Use DevTools to verify:
- No 302 redirects
- No 403/404 errors
- No broken images
- No console errors

---

## Phase 5: Compliance

### Three-stage Compliance Check

**Stage 1: Privacy Scan**

| Category | Keywords to Watch | Action |
|----------|-----------------|--------|
| Financial | Specific amounts, salary, investment | Remove or generalize |
| Personal relationships | Breakup, divorce, SO details | Generalize to "past experience" |
| Health / Death | Deceased, illness, surgery | Remove, generalize to "health-conscious" |
| Private records | Diary, personal journals | Remove |
| Specific itineraries | Exact routes, dates, companions | Generalize to "a trip" |
| Credentials | ID, passport, passwords | Remove completely |
| Private conversations | Chat logs, screenshots | Generalize or remove |

**Scan order:**
1. Read full content (do not skim)
2. Scan for keywords above
3. Fix each found item immediately
4. Then publish

**Stage 2: Accuracy Check**
- [ ] Numbers verified with tools (dates, percentages, amounts)
- [ ] Images verified with image recognition tool
- [ ] No "assumption presented as fact"
- [ ] All links valid and accessible

**Stage 3: Consistency Check**
- [ ] Tone fits the brand/voice
- [ ] No violations of Red Lines
- [ ] External-facing identity is consistent

### Compliance Report Format

```
【Compliance Check】[Project Name]

✅ Privacy: Passed (X items generalized)
✅ Accuracy: Passed
✅ Consistency: Passed

【Verdict】Ready to launch / Needs fixes first
```

---

## Phase 6: Acceptance

### Acceptance Report Template

```markdown
# [Project Name] Acceptance Report
_Launch Date:_
_Sign-off:_

## Scope

| Feature | Result | Notes |
|---------|--------|-------|
| F-01 | ✅ Pass | |

## Issues Found

| Issue | Priority | Resolution | Status |
|-------|----------|------------|--------|
| | | | ✅ Resolved |

## Final Verdict

[ ] APPROVED — Ready to launch
[ ] REJECTED — Fix before launching

## Launch Notice

- Time:
- Impact:
- Rollback plan:
```

---

## Phase 7: Retrospective

### Retrospective Template

```markdown
# [Project Name] Retrospective
_Date:_

## Overview
- Goal:
- Launch date:
- Outcome:

## What Went Well
1.

## What Could Improve
1.

## Data Retrospective (if applicable)
- Metrics:
- Analysis:
- Next steps:

## Action Items

| Item | Owner | Due |
|------|-------|-----|
| | | |
```

---

## Async Review Mechanism

### Problems solved by async reviews

| In-person problem | Async solution |
|-------------------|---------------|
| Multiple people need to see it | Doc comments |
| Quick discussion needed | Messaging |
| Decision needed | Comment reply |

### Decision rules
- One decision-maker assigned at project start
- Outcomes: Approved / Rejected / Revise and resubmit
- 48-hour silence = approved

### When async does NOT work
- Complex UX discussions (visual + interactive)
- Emergency decisions (use video/voice)

---

## Document Conventions

### Naming
```
[ProjectName]_[DocType]_v[Version]
Examples:
  Magazine_PRD_v1.0
  Magazine_Design_v1.0
  Magazine_TestCases_v1.0
```

### Deleting content
Use strikethrough, never direct deletion:
```
~~old content~~ → canceled (reason)
new content
```

### Version history
Every document tracks: version, date, author, changes

---

## Project Document Checklist

| Document | File Naming Convention | Phase | Status |
|----------|----------------------|-------|--------|
| 项目文件夹 | `{ProjectName}_项目` | 规划期 | |
| 01需求分析 | `{ProjectName}_需求分析01_v版本` | Phase 1 | |
| 02PRD | `{ProjectName}_PRD_v版本` | Phase 1 | |
| 设计稿 | `{ProjectName}_设计稿_v版本` | Phase 2 | |
| 开发设计 | `{ProjectName}_开发概念设计_v版本` | Phase 3 | |
| 测试用例 | `{ProjectName}_测试用例_v版本` | Phase 4 | |
| 合规报告 | `{ProjectName}_合规报告_v版本` | Phase 5 | |
| 验收报告 | `{ProjectName}_验收报告_v版本` | Phase 6 | |
| 上线通告 | `{ProjectName}_上线通告_v版本` | Phase 6 | |
| 项目复盘 | `{ProjectName}_项目复盘_日期` | Phase 7 | |

**命名示例：**
```
旅行购物计算器_项目/
旅行购物计算器_需求分析01_v1.0
旅行购物计算器_PRD_v1.0
旅行购物计算器_设计稿_v1.0
旅行购物计算器_测试用例_v1.0
旅行购物计算器_验收报告_v1.0
```

---

_This is a generalized product development SOP. Adapt the phases, templates, and review process to your own workflow._
