.....﻿
# 📝 GCE PDF Scraper (Cameroon Special)

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

A fast and reliable Python script to automatically download **A-Level past questions For all science subjects** from [Cameroon GCE Revision](https://cameroongcerevision.com/a-level/cameroon-gce-questions-mathematics-a-level/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/june-chemistry-a-level/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/june-biology-a-level/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/june-computer-science/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/cameroon-gce-questions-a-level-physics/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/cameroon-gce-questions-a-level-ict/).
[Cameroon GCE Revision](https://cameroongcerevision.com/a-level/june-f-math-a-level/).


It organizes PDFs by year, handles Google Drive embeds, and ensures only valid PDFs are downloaded.

---

## 🚀 Features

* ✅ Depending on the script, it Downloads **only papers for that subject**, ignores other subjects
* ✅ Detects and organizes PDFs by **year**
* ✅ Handles **Google Drive embedded PDFs**
* ✅ Verifies real PDFs to prevent corrupted downloads
* ✅ **Parallel scanning and downloading** for faster performance
* ✅ Organizes files in `GCE_SUBJECT/<year>/` folders
* ✅ Uses **persistent connections** for efficiency

---

## ⚙️ Requirements

* Python 3.8 or higher
* Required packages:

```bash
pip install requests beautifulsoup4
```

---

## 📦 Usage

1. Clone or download the repository.
2. Run the script partaning to the Subject you want to get

## Mathematics
```bash
python GCE Paper Scrapper (Math).py
```
## Chemistry
```bash
python GCE Paper Scrapper (Chemistry).py
```
## Physics
```bash
python GCE Paper Scrapper (Physics).py
```
## Biology
```bash
python GCE Paper Scrapper (Biology).py
```
## Further-Math
```bash
python GCE Paper Scrapper (Further Math).py
```
## ICT
```bash
python GCE Paper Scrapper (ICT).py
```
## Computer Science
```bash
python GCE Paper Scrapper (Computer Science).py
```

3. PDFs will be downloaded into the `GCE_(SUBJECT)` folder, automatically sorted by year.

---

## 🧠 How It Works

1. Scrapes the main A-Level page for all subjects to find links to all paper pages.
2. Extracts PDF links from:

   * Google Docs Viewer embedded iframes
   * Direct PDF links
3. Downloads PDFs safely, verifying each file is a valid PDF.
4. Saves PDFs into **year-specific folders** for easy organization.

---

## ⚠️ Notes

* Uses **multi-threading** (`ThreadPoolExecutor`) for faster downloads.
* Already downloaded files are skipped automatically.
* PDFs without a detectable year are stored in `Unknown_Year`.

---

## 📂 Folder Structure

```
GCE_(SUBJECT)/
├── 2018/
│   ├── paper1.pdf
│   └── paper2.pdf
├── 2019/
│   └── paper1.pdf
└── Unknown_Year/
    └── paper.pdf
```

---

## 📜 License

This project is licensed under the MIT License.


