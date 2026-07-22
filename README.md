# 📚 Superpowers Skill 编写课

> 一个为**零基础学习者**设计的离线交互课程，带你从「完全不懂 skill 是什么」到「能独立写出、测试、打包一个 superpowers skill」。

课程基于 [obra/superpowers](https://github.com/obra/superpowers) 项目（v5.1.0），拆解了它的 14 个真实 skill 的源码，提炼出可复用的写作方法论。

## 🎯 适合谁

- 听说过 Claude Code / Cursor / Gemini CLI 的 skill 系统，但不知道怎么自己写
- 英语 Level 1-2，看 superpowers 原版英文文档吃力
- 想要一份**沉淀下来、能反复看、能分享**的学习材料

## 🚀 在线预览

👉 **[直接打开课程](https://memoryl7.github.io/superpowers-course/)**

（首次加载约 1-2 秒，所有功能在浏览器本地运行，无需登录、无需联网）

## 📖 课程内容

7 个模块，共 **29 节课 + 1 个毕业项目**：

| 模块 | 主题 | 课程数 |
|:---:|---|:---:|
| 🟢 | **建立认知** —— skill 是什么、怎么被触发 | 4 课 |
| 🟡 | **拆解骨架** —— frontmatter、description、body 标准章节 | 5 课 |
| 🟠 | **掌握武器库** —— XML 标签 / 流程图 / 借口表 / Checklist / Bad-Good / 渐进式披露 | 6 课 |
| 🔴 | **动手实战** —— 用 TDD 思路写第一个 skill（RED-GREEN-REFACTOR） | 5 课 |
| 🟣 | **进阶精修** —— 说服心理学 7 原则、subagent 测试、Iron Law、Rigid vs Flexible | 4 课 |
| 🔵 | **打包发布** —— 从单个 skill 到完整 plugin（含 SessionStart hook） | 4 课 |
| 🏁 | **毕业项目** —— 做一个属于你自己的 mini-superpowers | 1 课 |

每节课包含：
- 📝 概念讲解（中英对照，专为零基础设计）
- 🔍 真实源码拆解（来自 superpowers v5.1.0）
- 📚 本课生词表
- ✅ 选择题作业（选完即时显示所有选项的解释）

## ✨ 功能特性

- 🎨 **学习平台风格**：左侧目录树 + 主内容区 + 顶部进度条
- 📊 **进度追踪**：自动记录你学到哪一课、哪些已完成（存 localStorage）
- 📝 **作业记录**：每课作业可在页面作答，自动保存
- 🌙 **暗色模式**：一键切换深/浅色主题
- 🔍 **全文搜索**：`Ctrl/Cmd + K` 快速检索课程内容
- 📱 **响应式**：手机也能正常看
- 🈶 **零依赖**：单文件 HTML，无外部 JS/CSS，**完全离线可用**

## 💻 本地使用

### 方法 1：直接双击

下载 [`index.html`](./index.html)，双击用浏览器打开即可。

### 方法 2：本地起服务（避免某些浏览器对 `file://` 的限制）

```bash
# 任选一种
python -m http.server 8000
# 或
npx serve
```

然后访问 `http://localhost:8000`。

### 方法 3：fork 本仓库

点击右上角 **Fork**，然后在你自己的仓库 Settings → Pages 里启用即可获得你自己的在线版本。

## 🛠️ 技术细节

- **架构**：单文件 HTML（HTML + CSS + 原生 JS，无框架、无构建）
- **数据**：所有课程内容存为 JS 对象字面量，直接嵌入 `<script>` 块
- **存储**：`localStorage`（key: `superpowers-course-state-v1`）
- **体积**：约 437 KB（含全部 29 课内容）

## 📚 致谢与版权

- 课程内容基于 [obra/superpowers](https://github.com/obra/superpowers)（MIT License，作者 Jesse Vincent）
- 所有 superpowers 真实源码片段的版权归原作者所有，本课程仅用于教学拆解
- 课程本身的组织、讲解、习题设计为原创

## 📝 License

MIT
