# 🧪 PermeationNet: Open Skin Permeation Database

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Vue.js](https://img.shields.io/badge/Vue.js-3.0-4FC08D?logo=vue.js)](https://vuejs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-blue?logo=github)](https://pages.github.com/)

**PermeationNet** 是一个专注于布洛芬（Ibuprofen）及其他药物皮肤渗透数据的开源数据库项目。旨在通过结构化的数据展示，帮助研究人员快速查阅文献中的渗透参数、实验条件及证据片段。

🔗 **在线访问:** [点击这里查看演示](https://你的用户名.github.io/你的仓库名/) 
*(请替换上面的链接为你实际的 GitHub Pages 链接)*

---

## ✨ 项目亮点

* **⚡️ 极速体验**: 基于 Vue.js 的响应式架构，提供毫秒级的搜索和筛选体验。
* **📱 优雅界面**: 使用 Tailwind CSS 构建的现代化 UI，适配桌面端与移动端。
* **📄 证据溯源**: 每一条数据都关联了 DOI 链接和原始文献中的文本片段（Evidence Snippets），确保数据可信度。
* **🛠 零依赖部署**: 纯静态网页（Single File Component），无需安装 Node.js、数据库或后端服务，下载即用。

---

## 🚀 如何使用

### 1. 在线浏览
直接访问我们的 [GitHub Pages 页面](https://你的用户名.github.io/你的仓库名/) 即可开始检索数据。

### 2. 本地运行
如果你想在本地查看代码或离线使用：

1.  克隆或下载本项目：
    ```bash
    git clone [https://github.com/你的用户名/你的仓库名.git](https://github.com/你的用户名/你的仓库名.git)
    ```
2.  进入文件夹，**直接双击打开 `index.html`**。
3.  没错，就是这么简单！不需要 `npm install`，也不需要配置服务器。

---

## 📊 数据更新指南

本项目的核心是一个纯 HTML 文件，数据直接嵌入在代码中。如果你需要更新数据集：

1.  准备好你的清洗后的数据（JSON 格式）。
2.  使用文本编辑器（如 VS Code, Notepad++）打开 `index.html`。
3.  搜索代码中的 `const rawData` 变量。
4.  将 `[...]` 中的内容替换为你新的 JSON 数据。
5.  保存文件并提交到 GitHub，网页会自动更新。

### 数据字段说明

| 字段名 | 类型 | 说明 |
| :--- | :--- | :--- |
| `title` | String | 文献标题 |
| `doi` | String | 数字对象标识符 (不含 https 前缀) |
| `concentration` | String | 药物浓度 (如 "10 wt%") |
| `value` | Number | 渗透值 (Q_final 或 Flux) |
| `unit` | String | 数值单位 (如 "µg cm−2") |
| `evidence` | Array | 包含 `field` (字段名) 和 `snippet` (原文片段) 的证据列表 |

---

## 🤝 贡献与反馈

这是一个开源项目，非常欢迎社区贡献！

* 如果你发现了数据错误，请提交 **Issue**。
* 如果你想改进网页界面，欢迎提交 **Pull Request**。

## 📜 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。
数据内容来源于公开科学文献，仅供科研参考。

---
*Created with ❤️ for Open Science.*
