# Basic Context Skills

一对配套使用的 Agent skills，用于建立和持续维护项目的 **basic context**。

Basic context 由用户和 Agent 共同维护。文档讲清项目背景、目标和全局规则，示例代码展示这个项目里什么叫写得好。

| Skill | 用法 |
| --- | --- |
| [Setup Matt Pocock Skills（modified）](skills/setup-matt-pocock-skills/SKILL.md) | 和用户讨论项目结构，在 `AGENTS.md` 中明确目录、文档职责和各项信息的权威来源。确认方案后再实施。 |
| [Wrap-up](skills/wrap-up/SKILL.md) | 按项目约定整理本轮文件和上下文文档，裁剪重复记录，保留验收证据。关键取舍由用户决定，已授权的整理在同一轮做完。 |

将两份 skill 目录连同各自的配套文件放进客户端的 skills 目录。开始项目时调用 `$setup-matt-pocock-skills`，收尾时调用 `$wrap-up`。Setup 可复用已安装的 `grilling`，也可在对话里对结构决策做聚焦访谈。


## skill核心理念
agent进行有效的任务前提是符合用户意图的basic context（我引出的新概念，指的是由用户高度参与构建，表述全局规则，背景目标并包含优秀代码示例的基层context，另一些context是session过程中的或者类似ticket那样即用即抛的），basic context由文档和示例代码两部分组成。需要共同围绕用户意图维护，用户需要在setup和wrapup阶段高度参与决策和实际维护，在对目标功能grill产出工单的过程中才能减少反复赘述。立场是如果项目内容需要高度符合用户独特的构思而非模板修改元素用户必须在此阶段高度参与，而非信赖不确定性的agent记忆系统。
问题核心是：LLM无论再智能也会受到杂乱的context文档影响，产出难以维护的屎山代码，将用户意图转述的过于复杂让简单问题变得难以解决。

## 上游

Setup 改自 [mattpocock/skills](https://github.com/mattpocock/skills)，安装基线为 [4ae2317](https://github.com/mattpocock/skills/commit/4ae2317ddb22b046e26455e4f9c9b3aaaf62212d)。[上游 MIT 许可与署名](skills/setup-matt-pocock-skills/LICENSE)随其分发。
