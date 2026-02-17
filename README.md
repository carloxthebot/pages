# OpenClaw Pages

自動化索引系統 - 新增 HTML 檔案後會自動更新首頁

## 🚀 使用方式

### 新增頁面

```bash
# 1. 直接把 HTML 檔案放進來
cp your-page.html .

# 2. Commit（index.html 會自動更新）
git add your-page.html
git commit -m "Add your page"
```

### 手動生成（如果需要）

```bash
node generate-index.js
```

## 🔧 自動化機制

- **Pre-commit hook** 會在每次 commit 前自動執行 `generate-index.js`
- 自動掃描所有 `.html` 檔案（除了 `index.html`）
- 自動更新首頁連結列表
- 自動加入此次 commit

## 📂 檔案結構

```
pages/
├── .git/hooks/pre-commit  ← 自動化 hook
├── generate-index.js      ← 生成 script
├── index.html             ← 自動生成的首頁
├── README.md              ← 說明文件
└── *.html                 ← 你的頁面們
```

## 🎨 設計特色

- 現代化漸層背景
- 卡片式設計
- Hover 動畫效果
- 響應式設計
- 自動統計頁面數量

---

**Built by CarloX 🦞**
