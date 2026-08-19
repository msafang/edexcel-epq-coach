# EPQ 课题定题教练 (epq-topic-coach)

> 引导 A-Level/EPQ 学生把兴趣收敛为可验证研究问题的 OpenClaw Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 这是什么

一个 OpenClaw skill,把一线 EPQ 老师的 3 套定题引导方法和授课记录中的可行性检查沉淀为可被 AI 复用的工作流:

| 方法 | 适合学生 | 核心武器 |
|---|---|---|
| **兴趣锚定法** | 有明确兴趣 + 看过相关素材 | "应用+挑战/前景"模板 |
| **三源杂交法** | 自称"淡人"/无明确兴趣 | "兴趣/痛点/热点"三源 + 候选清单 |
| **四维收窄法** | 完全没方向 | 四维变量公式 + 学术伦理筛查 |

v4 在三种方法之间增加了候选题验证、6 维可行性评分、题目/研究问题/研究目标拆分和定题决策记录，方便与 Proposal、Activity Log 衔接。

## 触发词

- `帮学生定题`
- `EPQ 选题`
- `用 epq-topic-coach`
- `定题辅导`
- `确定研究方向`

## 安装

### 方式 A:ClawHub(推荐,需要 OpenClaw)

```bash
npx clawhub@latest install epq-topic-coach \
  --registry=https://mirror-cn.clawhub.com \
  --dir ~/.agents/skills
```

### 方式 B:git clone + 手动安装

```bash
git clone https://github.com/msafang/epq-topic-coach.git
mkdir -p ~/.agents/skills/epq-topic-coach
cp -r epq-topic-coach/* ~/.agents/skills/epq-topic-coach/
```

### 方式 C:直接下载 zip

从 GitHub Releases 下载 `epq-topic-coach-v3.zip`,解压到 `~/.agents/skills/epq-topic-coach/`。

## 使用示例

启动 OpenClaw 后,直接说:

> "帮张同学确定研究方向,他是领科 A2 经济学方向的"

AI 会自动:
1. 问 3-5 个摸底问题
2. 根据学生画像选方法
3. 引导出题目
4. 过 5 个学术伦理雷区
5. 输出最终题目 + 研究问题 + 选题理由 + 思维导图
6. 输出可行性评分和下一步验证任务

## 包含内容

- `SKILL.md` —— 完整的 skill 定义(3 套方法 / 3 公式 / 可行性评分 / 5 雷区 / 防误操作 / 案例)
- `CHANGELOG.md` —— 版本历史
- `LICENSE` —— MIT 许可证

## 适用场景

- **EPQ**(英国 A-Level Extended Project Qualification)
- **IA**(IB Internal Assessment)
- **EE**(IB Extended Essay)
- **IPQ** 等研究性论文选题阶段

## 重要提示

- 本 skill 是**方法论沉淀**,不是替代老师。AI 定题后必须由真人 EPQ supervisor 审核、签字。
- 学术伦理 5 雷区只覆盖 A-Level EPQ 高频问题;具体学校 IRB 要求请以学校为准。
- 课题定下来后,后续的**文献综述、思维导图、研究目标拆解**会用到其他 skill(可后续沉淀为 `epq-research-coach` 等)。

## Credits

- **方法论源头**:3 份 EPQ 定题课逐字稿(已脱敏)
- **整理与沉淀**:Fang Ai(方皑)| 上海方辰式教育科技
- **OpenClaw skill 化**:MM(贴身秘书 AI)
- **License**:MIT

---

🔗 **相关链接**:
- OpenClaw 项目:[openclaw/openclaw](https://github.com/openclaw/openclaw)
- ClawHub 国内镜像:[mirror-cn.clawhub.com](https://mirror-cn.clawhub.com)
- 作者 GitHub:[msafang](https://github.com/msafang)
