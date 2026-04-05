# Claude 大師級使用大全 — Companion Repository

> 購買完整電子書：[立即購買](https://jacksonfire526.gumroad.com/l/qsiagl) | [Landing Page](https://jacksonfire526.gumroad.com/l/qsiagl) | [讀者社群](https://ko-fi.com/onewallai)

[![Stars](https://img.shields.io/github/stars/jacksonfire526/claude-mastery?style=social)](https://github.com/jacksonfire526/claude-mastery)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

806 頁 PDF + EPUB。32 章 + 9 附錄。180+ 研究來源。繁體中文。

這本書解決一個問題：**大多數人只用到 Claude 三分之一的能力。**

Ch27 用 10 個真實任務做了控制變量實驗 — 同模型、同提示詞，只改前置設定。平均品質差距 **2.9 倍**。最大差距 5.1 倍。

本倉庫收錄精選範例和模板。完整內容請見正式電子書。

---

## 為什麼需要這本書

| 你的狀況 | 書裡的答案 |
|----------|-----------|
| Claude 結果忽好忽壞 | Ch4-8：前置設定五層架構，每層該放什麼 |
| 不知道 CLI 能做什麼 | Ch11：40+ 斜線指令完整索引，含版本變更追蹤 |
| API 費用太高 | Ch25-26：Token 精算 + 七種優化策略（最高省 95%） |
| 不知道選 Claude 還是 ChatGPT | Ch31：SWE-bench 實測分數 + 12 維度量化對比 |
| CLAUDE.md 不知道怎麼寫 | Ch7：80+ 真實開源專案範例 + 7 大反模式 |
| 想自動化工作流 | Ch20-23：MCP + Agent SDK + GitHub Actions + Headless |

---

## 精選 15 個可複製提示詞

以下範例可直接複製使用，將 `[替換]` 部分改為你的內容即可。

### 1. 萬用 System Prompt 模板
```
你是一位 [替換：專業領域] 專家。
你的工作風格：[替換：簡潔/詳細/學術/口語]。
你的輸出格式：[替換：Markdown/JSON/純文字]。
你永遠用 [替換：繁體中文] 回覆。
當你不確定時，先問問題再回答，不要猜測。
```

### 2. CLAUDE.md 基礎模板
```markdown
# Project: [替換：專案名稱]

## Overview
[替換：一句話描述專案]

## Tech Stack
- [替換：語言/框架/工具]

## Directory Structure
- src/ — 主程式碼
- tests/ — 測試檔案
- docs/ — 文件

## Commands
- Build: [替換：npm run build]
- Test: [替換：npm test]
- Lint: [替換：npm run lint]

## Style Guide
- [替換：你的程式碼風格偏好]
```

### 3. 高品質程式碼生成（XML 結構）
```
<context>
語言：[替換：TypeScript]
框架：[替換：Next.js 14]
規範：[替換：ESLint + Prettier]
</context>

<task>
寫一個 [替換：功能描述]。
要求：
1. 包含完整的 TypeScript 型別
2. 包含錯誤處理
3. 包含 JSDoc 註解
4. 包含單元測試（使用 [替換：Jest]）
</task>

<output_format>
先列出檔案結構，然後逐一輸出每個檔案的完整程式碼。
</output_format>
```

### 4. 文案寫作（COSTAR 框架）
```
<context>目標受眾是 [替換：25-35歲的科技從業者]</context>
<objective>寫一篇 [替換：產品介紹文]</objective>
<style>語調 [替換：專業但有溫度]，用「你」稱呼讀者</style>
<tone>[替換：自信、數據導向]</tone>
<audience>[替換：已使用過類似產品但想升級的用戶]</audience>
<response>
格式：[替換：800字文章，含標題和3個小標]
包含：至少2個具體數據、1個使用場景、1個CTA
</response>
```

### 5. 數據分析
```
分析以下數據：

<data>
[替換：貼上你的數據]
</data>

請依序完成：
1. 數據概覽：基本統計量（平均、中位數、標準差、範圍）
2. 趨勢分析：找出顯著的上升/下降趨勢
3. 異常值：標記超過 2 個標準差的數據點
4. 相關性：變數間的相關係數
5. 結論：3 個可執行的建議

用表格呈現數據，用 Mermaid 圖表呈現趨勢。
```

### 6. 程式碼審查
```
請審查以下程式碼：

<code>
[替換：貼上程式碼]
</code>

審查標準：
1. Bug 風險（會不會出錯？）
2. 效能（有沒有明顯的效能問題？）
3. 安全（有沒有安全漏洞？）
4. 可讀性（別人看得懂嗎？）
5. 架構（設計合理嗎？）

對每個問題：說明問題 → 給出修改建議 → 提供修改後的程式碼。
```

### 7. 翻譯（保留術語）
```
將以下 [替換：英文] 文本翻譯為 [替換：繁體中文]。

規則：
- 技術術語保留英文原文，首次出現時括號附中文翻譯
- 保持原文的段落結構
- 語調：[替換：專業但易讀]
- 如有歧義，列出多種翻譯方式讓我選擇

<source>
[替換：貼上原文]
</source>
```

### 8. 學習新概念
```
我想學習 [替換：概念名稱]。

我的背景：[替換：我是前端工程師，會 JavaScript 和 React]
我的目標：[替換：能在專案中實際使用]
希望的深度：[替換：★★☆ 進階]

請用以下結構教我：
1. 一句話解釋（白話）
2. 為什麼重要（解決什麼問題）
3. 核心概念（3-5 個關鍵點）
4. 實際範例（用我熟悉的技術棧舉例）
5. 常見陷阱（初學者最容易錯的 3 件事）
6. 延伸資源（推薦 3 個學習資源）
```

### 9. 會議紀錄整理
```
以下是會議的原始紀錄/逐字稿：

<transcript>
[替換：貼上會議紀錄]
</transcript>

請整理為：

## 會議摘要（3 句話以內）

## 決議事項
| 編號 | 決議 | 負責人 | 截止日 |
|------|------|--------|--------|

## 待辦事項（Action Items）
- [ ] [事項] — @[負責人] — [截止日]

## 關鍵討論點
（重要但未形成決議的討論）

## 下次會議
- 時間：
- 議題：
```

### 10. 省 Token 的 System Prompt
```
你是一個注重效率的助手。遵守以下規則：
1. 回答簡潔精確，不加不必要的客套話
2. 除非我要求，不要解釋你的推理過程
3. 用列表和表格代替長段落
4. 如果問題簡單，用 1-2 句話回答
5. 程式碼只輸出改動的部分，不要重複未修改的程式碼
```

### 11. Prompt Caching 模板（API）
```json
{
  "model": "claude-sonnet-4-6-20260401",
  "max_tokens": 1024,
  "system": [
    {
      "type": "text",
      "text": "[替換：你的固定 system prompt，放在這裡會被快取]",
      "cache_control": {"type": "ephemeral"}
    }
  ],
  "messages": [
    {"role": "user", "content": "[替換：每次不同的問題]"}
  ]
}
```

### 12. 自動修正提示詞
```
完成以下任務：[替換：任務描述]

完成後，請自行審查：
1. 有沒有遺漏任何要求？
2. 有沒有邏輯錯誤？
3. 有沒有可以改善的地方？

如果發現問題，直接修正後輸出最終版本。
不要輸出初稿，只輸出審查修正後的版本。
```

### 13. 競品分析
```
請分析 [替換：產品A] vs [替換：產品B] vs [替換：產品C]。

分析維度：
| 維度 | 產品A | 產品B | 產品C |
|------|-------|-------|-------|
| 價格 | | | |
| [替換：核心功能1] | | | |
| [替換：核心功能2] | | | |
| 優勢 | | | |
| 劣勢 | | | |

最後給出：
1. 各產品最適合的使用場景
2. 如果只能選一個，推薦哪個（說明理由）
```

### 14. Git Commit 訊息生成
```
根據以下 diff 生成 commit message：

<diff>
[替換：貼上 git diff]
</diff>

格式：Conventional Commits
語言：英文
規則：
- 第一行 <type>(<scope>): <description>，不超過 72 字
- 空一行後寫 body（說明 why，不是 what）
- type: feat/fix/refactor/docs/test/chore
```

### 15. Skills 檔案模板
```yaml
---
name: [替換：skill 名稱]
description: [替換：一句話描述，何時觸發此 skill]
trigger: "[替換：觸發條件描述]"
---

# [替換：Skill 名稱]

## 適用場景
- [替換：場景1]
- [替換：場景2]

## 執行步驟
1. [替換：步驟1]
2. [替換：步驟2]

## 品質標準
- [替換：標準1]
- [替換：標準2]

## 範例
[替換：一個完整的輸入輸出範例]
```

---

## 章節預覽

| Part | 章節 | 主題 | 難度 |
|------|------|------|------|
| 1 | Ch 1-3 | 認識 Claude：模型家族、四大入口、付費策略 | ★☆☆ |
| 2 | Ch 4-8 | **前置設定決定成敗**：網頁/桌面/CLI/CLAUDE.md/Skills | ★★☆ |
| 3 | Ch 9-14 | 指令集完整索引：全功能操作手冊、斜線指令、API 參考 | ★☆☆ — ★★★ |
| 4 | Ch 15-19 | 提示詞架構：基礎、Claude 專屬技巧、進階框架、模板 | ★★☆ |
| 5 | Ch 20-24 | 生態系統：MCP、Agent SDK、Plugins、CI/CD、IDE 整合 | ★★☆ — ★★★ |
| 6 | Ch 25-30 | **大師級實戰**：Token 精算、成本優化、對比實驗、隱藏功能 | ★★★ |
| 7 | Ch 31-32 | 知己知彼：Claude vs ChatGPT vs Gemini、開發工具大比拼 | ★★☆ |
| 附錄 | A-I | 速查表、模板庫、範本庫、費用計算器、錯誤代碼、快捷鍵 | — |

---

## 書中的幾個關鍵發現

- **中文 token 比英文貴 54%**：1 中文字 ≈ 2 tokens，1 英文字 ≈ 1.3 tokens（Ch25）
- **前置設定的品質差距是 2.9 倍**：不是 prompt 的問題，是設定的問題（Ch27）
- **Prompt Caching + Batch API 疊加可省 95%**：大多數付費用戶從未使用過（Ch26）
- **Skills 三層架構省 82-98% context**：把 CLAUDE.md 從 10,000 tokens 壓到 2,000（Ch8）
- **Anthropic 內部 70% 程式碼由 AI 自主完成**：但 2/3 任務需至少一輪修正（附錄 H）

---

## 如何使用本倉庫

```bash
# 複製整個倉庫
git clone https://github.com/jacksonfire526/claude-mastery.git

# 進入目錄
cd claude-mastery

# 瀏覽提示詞模板
ls prompts/

# 複製 CLAUDE.md 範本到你的專案
cp templates/claude-md/basic.md /path/to/your-project/CLAUDE.md
```

### 目錄結構

```
claude-mastery/
├── README.md              ← 你正在看的文件
├── prompts/               ← 精選提示詞模板（分類整理）
│   ├── coding/
│   ├── writing/
│   ├── analysis/
│   └── general/
├── templates/             ← 設定檔範本
│   ├── claude-md/         ← CLAUDE.md 範本（10 種專案類型）
│   ├── skills/            ← Skills 檔案範本
│   └── mcp/               ← MCP 設定範本
├── cheatsheets/           ← 速查表（可列印）
│   ├── shortcuts.pdf
│   ├── error-codes.pdf
│   └── slash-commands.pdf
└── examples/              ← 真實專案設定範例
```

---

## 支持本專案

如果這個倉庫對你有幫助：

- **Star** 本倉庫，幫助更多人發現這個資源
- 在社群**分享**這個倉庫
- 提交 **Issue** 回報問題或建議
- 提交 **PR** 貢獻新的提示詞模板

---

## 授權

本倉庫的提示詞模板採用 [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) 授權。
你可以自由使用和分享，但不可用於商業販售。

完整書籍內容版權所有 ONE WALL AI。

---

<p align="center">
  <b>讓 Claude 發揮 100%——從正確的設定開始。</b>
  <br><br>
  <a href="https://jacksonfire526.gumroad.com/l/qsiagl">購買電子書</a> · <a href="https://jacksonfire526.gumroad.com/l/qsiagl">Landing Page</a> · <a href="https://github.com/jacksonfire526/claude-mastery/issues">回報問題</a>
</p>
