# Edexcel EPQ Coach

> 面向 Pearson Edexcel Level 3 EPQ 的选题、Proposal、Activity Log、Evaluation/Reflection 和论文质量评估 skill。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 适用范围

本 skill 专门服务于 Edexcel Level 3 Extended Project Qualification：

- P301 Dissertation
- P302 Investigation / Field Study
- P303 Performance
- P304 Artefact

Proposal 和 process-record 指导覆盖 P301-P304；详细的论文质量与 AO1-AO4 评估主要适用于 P301/P302。

明确排除 LRN EPQ 文件、表格、分数和案例。混合学生档案中，只使用能够确认属于 Edexcel 的材料。

## 完整工作流

```text
定题与可行性判断
        ↓
Proposal
        ↓
Activity Log
        ↓
论文、调查、表演或 artefact
        ↓
Evaluation / Reflection
        ↓
论文与证据链质量评估
```

### 阶段 -1：定题与可行性

保留原有的三种定题路径：

| 方法 | 适合情况 | 核心操作 |
|---|---|---|
| 兴趣锚定法 | 学生有具体兴趣、经历或素材 | 从兴趣收敛到可争论或可实现的问题 |
| 三源混合法 | 只有宽泛学科方向 | 结合兴趣、问题/张力和可靠来源生成候选 |
| 四维收窄法 | 题目过大或过于模糊 | 通过时间、地点、对象/群体和核心变量收窄 |

定题阶段还会：

- 生成多个候选，而不是直接替学生拍板；
- 区分 topic、research question/hypothesis/brief 和 objectives；
- 验证来源、数据、材料、设备、场地或参与者是否可获得；
- 检查范围、方法、伦理、隐私、同意和安全；
- 保存被放弃题目、修改原因和下一步验证任务；
- 将定题记录衔接到 Proposal 和 Activity Log。

六维可行性评分只是内部比较工具，不是 Edexcel 官方分数，也不能换算成保证的等级。

### Proposal、Activity Log 与 Evaluation

skill 会根据真实学生信息引导或生成：

- focused title、question、objectives 和选题理由；
- activities、timescales、milestones、resources 和 contingencies；
- 具有真实日期和项目证据的 Activity Log；
- 基于实际计划与执行差异的 Evaluation/Reflection；
- 缺失事实、需要学生确认的内容和下一步行动。

不会编造日期、活动、来源、数据、发现、导师反馈、签名或第一人称经历。

### 论文质量评估

评估时优先检查完整证据链，而不是只看语言流畅度：

`question -> objectives -> plan -> dated activity evidence -> resources/data -> analysis -> outcome -> evaluation`

输出可包括：

- provisional AO1-AO4 marks/bands 及证据定位；
- 研究问题对齐、范围、来源、引用、综合分析和论证质量；
- P302 的样本、方法、数据质量、计算、局限和可复现性；
- 证据缺口、学术诚信/AI disclosure 风险和最高价值修改建议。

本地成绩分布、文档外观和 AI 检测结果不能单独证明等级；最终成绩仍由中心评估和 moderation 决定。

## 使用与安装

这是一个以 `SKILL.md` 为核心的 skill package。将仓库内容放入目标 agent 的 skills 目录，并确保保留 `references/` 和 `agents/openai.yaml`：

```bash
git clone https://github.com/msafang/edexcel-epq-coach.git
```

在支持 skill 自动发现的环境中，可使用 `edexcel-epq-coach` 或 `$edexcel-epq-coach` 调用。

## 适合的请求

- “帮学生从兴趣确定一个 Edexcel EPQ 题目。”
- “检查这个 Proposal 是否可执行。”
- “根据真实活动记录填写 Activity Log。”
- “帮我写 Evaluation，但不要编造经历。”
- “根据论文、Proposal 和日志评估 P301/P302 质量。”
- “排除 LRN 文件，只分析 Edexcel 产出。”

## 文件结构

- `SKILL.md`：主工作流与边界
- `references/topic-selection.md`：定题、候选验证、可行性和 Proposal 衔接
- `references/proposal-section1.md`：Proposal Section 1 / Project Objectives 的学生语言与计划阶段规则
- `references/proposal-coaching.md`：Proposal 分阶段教学与一致性检查
- `references/form-workflow.md`：表格填写与直接生成流程
- `references/edexcel-rubric.md`：P301/P302 AO 评估要点
- `references/local-evidence.md`：脱敏后的本地 Edexcel 证据边界
- `agents/openai.yaml`：skill 的界面元数据
- `CHANGELOG.md`：版本历史
- `LICENSE`：MIT 许可证

## 重要边界

- 本 skill 是辅导和评估工具，不替代 Edexcel supervisor、centre assessor 或 moderation。
- Proposal、Activity Log 和 Reflection 必须建立在学生真实信息和项目证据上。
- P301 不应被强迫加入一手数据；P302 必须能说明数据收集方法并提供可用数据。
- Tutor/proposal checker 的批准、签名和 safeguarding/ethics 决策必须由授权人完成。

## Credits

- **方法论源头**：已脱敏的 EPQ 定题教学记录
- **整理与沉淀**：Fang Ai（方皑）| 上海方辰式教育科技
- **Skill 化与 Edexcel 流程扩展**：Codex
- **License**：MIT

相关链接：[作者 GitHub](https://github.com/msafang)
