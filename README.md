# Batch Rename Pro for After Effects / After Effects 批量重命名 Pro

[![License](https://img.shields.io/badge/License-非商用学习-blue.svg)](./LICENSE)
[![Language](https://img.shields.io/badge/语言-7种语言-green.svg)](#语言支持)

**Batch Rename Pro** 是一个为 Adobe After Effects 设计的强大批量重命名脚本。它支持项目面板中的素材、以及当前合成时间线上的图层，提供四种重命名模式：**格式重命名**、**文本替换**、**添加序号** 和 **添加文本**。界面简洁，多语言支持，并记忆您的设置。

> **作者**: ZBT Studio  
> **代码**: 完全由 [DeepSeek](https://chat.deepseek.com/) 编写

---
[English instructions](https://github.com/zbt00123/Batch-Rename-Pro-for-AE/blob/main/README_EN.md)

## ✨ 特性

- 🎯 **四种重命名模式**
  - **格式重命名**：批量定义基础名称 + 序号（前缀/后缀）
  - **替换文本**：查找并替换名称中的任意文本
  - **添加序号**：在原名称基础上添加递增序号（前缀/后缀）
  - **添加文本**：在名称开头或末尾添加自定义文本

- 🌐 **多语言支持**（内置 7 种语言，可随时切换）
  - 简体中文 · English · Français · Italiano · Русский · 日本語 · 한국어

- 🖱️ **友好的交互**
  - 每个模式独立切换

- 💾 **持久化设置**
  - 自动保存设置

- 📁 **灵活的目标选择**
  - 支持 **Project（项目）窗口** 中选中的任意素材（文件、合成、文件夹等）
  - 支持 **当前合成 Timeline（时间线）** 中选中的图层（按图层顺序排序）

- 📜 **版权与作者信息**
  - 仅限学习使用，可以任意修改、复制和转发，**严禁商用**。 
---

## 🚀 使用方法

### 安装
1. 下载 `Batch Rename Pro for AE.jsx` 脚本文件。
2. 将脚本放置到 After Effects 的脚本目录：
   - Windows: `C:\Program Files\Adobe\Adobe After Effects <版本>\Support Files\Scripts\ScriptUI Panels\`
   - macOS: `/Applications/Adobe After Effects <版本>/Scripts/ScriptUI Panels/`
3. 在 After Effects 中，通过菜单 `Window` > `Batch Rename Pro.jsx` 打开面板。

### 基本操作
1. 在 **Project 面板** 中选中要重命名的项目，或者在 **合成时间线** 中选中图层。
2. 在脚本面板中选择重命名 **模式**（格式 / 替换 / 添加序号 / 添加文本）。
3. 根据模式填写参数（例如基础名称、分隔符、起始数字等）。
4. 点击 **“执行重命名”** 按钮。

> **注意**：操作会创建撤销步骤（`Undo`），如果您不满意结果，可以按 `Ctrl+Z`（Win）或 `Cmd+Z`（Mac）撤销。

---

## ⚙️ 模式参数说明

| 模式 | 参数 | 说明 |
|------|------|------|
| **格式重命名** | 基础名称、分隔符、起始、步长、位数、序号位置 | 生成 `基础名称_序号` 或 `序号_基础名称` 格式，序号按设置递增 |
| **替换文本** | 查找、替换为 | 将名称中的指定文本全部替换为新文本 |
| **添加序号** | 分隔符、起始、步长、位数、序号位置 | 在原名称后（或前）追加递增序号，如 `原名称_001` |
| **添加文本** | 添加文本、位置（开头/末尾） | 在名称开头或末尾插入固定文本 |

- **序号位置**：`后缀` 表示序号在末尾，`前缀` 表示在开头。
- **起始 / 步长 / 位数**：支持鼠标滚轮、上下按钮和键盘方向键快速调整。

---

## 🌐 语言切换

点击主面板中的 **⚙** 齿轮按钮打开设置窗口，在 **语言** 下拉列表中选择您喜欢的语言。语言设置会自动保存，下次打开脚本时自动生效。

---

## 📝 注意事项

- 脚本仅对 **Project 窗口选中的项目** 或 **当前合成选中的图层** 生效，不会影响其他对象。
- 如果同时选中了项目和时间线图层，脚本会优先处理 **Project 窗口的选择**（符合 After Effects 默认行为）。
- 若替换文本的“查找”字段为空，脚本会提示错误。
- 序号位数建议在 1~10 之间，起始和步长有范围限制（0~999999 和 1~999999），超出会提示。

---

## 📄 许可证

本脚本**仅供学习使用**，您可以自由修改、复制和转发，但**严禁用于商业用途**。  
详细的许可证文本请见脚本内部的版权信息（设置窗口中也可查看）。

---

## 🤝 贡献与反馈

欢迎提交 [Issue](https://github.com/zbt00123/Batch-Rename-Pro-for-AE/issues) 和 [Pull Request](https://github.com/zbt00123/Batch-Rename-Pro-for-AE/pulls)。  
如果您发现任何问题或有改进建议，请在 GitHub 仓库中提出。

---

## 🙏 致谢

- 感谢 **DeepSeek** 提供强大的 AI 编码支持。
- 感谢所有使用和测试本脚本的用户。

---

*Made with ❤️ by ZBT Studio & DeepSeek*
