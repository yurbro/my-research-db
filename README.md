# 🧪 PermeationNet: Open Skin Permeation Database

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Vue.js](https://img.shields.io/badge/Vue.js-3.0-4FC08D?logo=vue.js)](https://vuejs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-blue?logo=github)](https://pages.github.com/)

[**English**](README.md) | [**简体中文**](README_zh-CN.md)

</div>

**PermeationNet** is an open-source database dedicated to skin permeation data of Ibuprofen and other APIs. It aims to provide researchers with quick access to structured permeation parameters, experimental conditions, and evidence snippets extracted from scientific literature.

🔗 **Live Demo:** [Click here to explore](https://yurbro.github.io/my-research-db/)

---

## ✨ Highlights

* **⚡️ Blazing Fast**: Built with Vue.js reactive architecture, offering millisecond-level search and filtering.
* **📱 Modern UI**: Designed with Tailwind CSS, fully responsive for both desktop and mobile devices.
* **📄 Evidence-Based**: Every record is linked to its DOI and includes original text snippets (Evidence Snippets) to ensure data credibility.
* **🛠 Zero Dependency**: Pure static web application (Single File Component approach). No Node.js installation, database, or backend required. Just download and run.

---

## 🚀 How to Use

### 1. Online Access
Visit our [GitHub Pages](https://yurbro.github.io/my-research-db/) to start searching the database immediately.

### 2. Run Locally
If you want to view the code or use the database offline:

1.  Clone the repository:
    ```bash
    git clone [https://github.com/yurbro/my-research-db.git](https://github.com/yurbro/my-research-db.git)
    ```
2.  Enter the folder and **simply double-click `index.html`**.
3.  That's it! No `npm install` or server configuration needed.

---

## 📊 Data Update Guide

This project separates logic from data for easier maintenance.

1.  Prepare your cleaned data in JSON format.
2.  Open the `data.js` file in a text editor.
3.  Replace the content inside `window.dbData = [...]` with your new data.
4.  Save the file. Open `index.html` to see the changes immediately.

### Data Fields

| Field | Type | Description |
| :--- | :--- | :--- |
| `title` | String | Title of the publication |
| `doi` | String | Digital Object Identifier (without https prefix) |
| `concentration` | String | Drug concentration (e.g., "10 wt%") |
| `value` | Number | Permeation value (Q_final or Flux) |
| `unit` | String | Unit of measurement (e.g., "µg cm−2") |
| `evidence` | Array | List of evidence snippets containing `field` and `snippet` |

---

## 🤝 Contribution

Contributions are welcome!

* Found a data error? Please submit an **Issue**.
* Want to improve the UI? Feel free to submit a **Pull Request**.

## 📜 License

This project is licensed under the [MIT License](LICENSE).
Data content is sourced from public scientific literature and is for research reference only.

---
*Created with ❤️ for Open Science.*
