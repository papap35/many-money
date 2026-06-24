# Many Money

[![CI](https://github.com/papap35/many-money/actions/workflows/ci.yml/badge.svg)](https://github.com/papap35/many-money/actions/workflows/ci.yml)

AI 輔助記帳軟體，目標是幫助使用者**開源節流**。除了完整的記帳功能，還包含家庭共享帳本、Duolingo 式的記帳習慣養成機制，以及 AI 金流分析與節流建議。

> 🚧 專案目前處於早期開發階段，詳細功能規劃請見 [`SPEC.md`](./SPEC.md)。

## 功能定位

- 📒 **完整記帳功能** — 收支記錄、分類、多帳本管理
- 👨‍👩‍👧 **家庭共享** — 邀請家人共用帳本，共同管理家庭財務
- 🔥 **遊戲化** — 連續記帳天數、預算進度、情勒提醒，養成記帳習慣
- 🤖 **AI 金流分析** — 分析消費模式，提出具體可執行的開源節流建議

## 技術棧

- **框架**：[Next.js](https://nextjs.org)（App Router）+ TypeScript
- **樣式**：Tailwind CSS
- **部署**：Vercel（push 到 `main` 自動部署正式環境，PR 自動產生 preview）
- **CI**：GitHub Actions（lint + typecheck + build）

## 開發

```bash
npm install
npm run dev
```

開啟 [http://localhost:3000](http://localhost:3000) 查看結果。

```bash
npm run lint        # ESLint
npm run typecheck   # tsc --noEmit
npm run build       # production build
```

## 專案文件

- [`AGENTS.md`](./AGENTS.md) — AI agent 與開發者共同遵守的開發規範（程式碼原則、測試規範、Branch/Commit/PR 流程）
- [`SPEC.md`](./SPEC.md) — 功能規格書，依優先級（P0~P5）拆解需求
