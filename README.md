# Copilot-Friendly 文档 & 流程体系

> 一个由 prompts + instructions 推动、支持微步推进、文件态记忆机制的文档创作与审校工具链。

## 一、项目简介

本项目开源了一整套配合 **Copilot Agent / Chat** 使用的 **写作 prompts 与流程说明**，帮助实现如下目标：

- 让 Copilot 像人类一样进行文档创作、审阅、完善、评分；
- 基于“微步 (micro-step)”与“文件态记忆 (file-state memory)”理念，规避上下文长度限制；
- 提供体系化 prompts：包括文档生成、审阅（review）、修复（fix）、代码补充文档（enrich），支持多轮迭代；
- 流程可审计、可记忆、可重复。

## 二、关键功能

- **文档生成 prompts**：自动生成 Copilot-friendly 文档骨架。
- **审阅 prompts**：检查文档与代码一致性、引用合法性、示例正确性等。
- **修复 prompts**：基于审阅结果安全地修正文档。
- **代码补充 prompts**：从现有代码中挖掘技巧/范式并插入文档。
- **评分 prompts**：自动打分、产出评分报告与改进建议。

## 三、适用对象

- 想构建高质量技术文档的人；
- 以 Copilot 为辅助，从提示文件优化写作流程的团队/个人；
- 需要长期维护文档且可审计生成过程的项目。

## 四、快速开始

```bash
git clone https://github.com/chinawrj/copilot-prompts.git
cd copilot-prompts
# 查看示例 prompts 文件
```

示例 prompt 文件路径：

- `prompts/01-gen-docs.md` —— 文档生成流程
- `prompts/02-review-docs.md` —— 审阅 prompts
- `prompts/03-fix-docs.md` —— 修补 prompts
- `prompts/04-enrich-docs.md` —— 代码补充 prompts
- `prompts/05-score-docs.md` —— 文档评分 prompts

使用指导：

1. 打开 VS Code → Copilot Chat；
2. 输入 `@workspace` + 选择目标 prompt 文件；
3. 按照提示进行“微步”执行，查看落盘结果。

## 五、贡献指南

欢迎参与这个项目！你可以：

- 基于已有技术/项目场景提供新的 prompts；
- 优化现有 prompts 流程；
- 补充 README 中的示例、CI 集成、license 等。

建议贡献流程：

1. Fork 本仓库；
2. 新建你的 `prompts/xx‑yourscenario.md` 文件；
3. 提交 PR，说明适用场景与使用方式。

## 六、许可协议

本项目采用 **MIT 许可证**。详细内容请参见 `LICENSE` 文件。

---

希望你能从这个流程体系获益，写出高质量、可审计、可复用、Copilot Friendly 的文档。如有建议或改进，欢迎提 Issue 或发 PR！
