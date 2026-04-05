# 附錄 A — 全指令速查表（一頁式索引）

> **用途**：不記得某個功能在哪？翻這裡。3 秒找到、5 秒理解、10 秒複製使用。
> **使用方式**：按平台（A-1）、按場景（A-2）、或按字母（A-3）三種方式查找。

---

## A-1：按平台分類

### 網頁版 (claude.ai)

| 功能 | 操作方式 | 難度 | 方案要求 | 詳見 |
|------|----------|------|----------|------|
| **Projects 專案** | | | | |
| 建立新專案 | 左側欄 → New Project | ★☆☆ | Free+ | → Ch4.2 |
| 上傳 Project Knowledge | Project → Add Content（30MB/檔，20 檔/對話） | ★☆☆ | Free+ | → Ch4.2 |
| 設定 Custom Instructions | Project → Instructions | ★☆☆ | Free+ | → Ch4.3 |
| 共享專案 | Project → Share | ★☆☆ | Team+ | → Ch4.2 |
| **Artifacts 成品** | | | | |
| 建立 Artifact | 對話中要求生成（支援 8 種類型） | ★☆☆ | Free+ | → Ch9 |
| 內嵌編輯 Artifact | 點擊 Artifact → Edit（速度比重生快 3-4x） | ★☆☆ | Free+ | → Ch9 |
| 下載 Artifact | Artifact 右上角 → Download | ★☆☆ | Free+ | → Ch9 |
| Artifact 8 種類型 | Code / HTML+CSS+JS / React / SVG / Mermaid / Markdown / 可下載檔案 / 分析視覺化 | ★☆☆ | Free+ | → Ch9 |
| **Styles 風格** | | | | |
| 切換預設風格 | 訊息框下方 → Style 選單（Normal/Concise/Formal/Explanatory） | ★☆☆ | Free+ | → Ch4.4 |
| 建立自訂風格（寫作樣本） | Settings → Styles → Create → 貼上範例 | ★★☆ | Free+ | → Ch4.4 |
| 建立自訂風格（描述） | Settings → Styles → Create → 文字描述 | ★★☆ | Free+ | → Ch4.4 |
| **Memory 記憶** | | | | |
| 檢視記憶 | Settings → Memory | ★☆☆ | Free+ | → Ch4.5 |
| 編輯 / 刪除記憶 | Settings → Memory → 單條 Edit/Delete | ★☆☆ | Free+ | → Ch4.5 |
| 匯入 ChatGPT / Gemini 記憶 | Settings → Memory → Import | ★☆☆ | Free+ | → Ch4.5 |
| **MCP 連接器（38+ 個）** | | | | |
| 連接 Google Drive | Settings → Integrations → Google Drive | ★☆☆ | Pro+ | → Ch4.6 |
| 連接 GitHub | Settings → Integrations → GitHub | ★☆☆ | Pro+ | → Ch4.6 |
| 連接 Slack | Settings → Integrations → Slack | ★☆☆ | Pro+ | → Ch4.6 |
| 連接 Notion | Settings → Integrations → Notion | ★☆☆ | Pro+ | → Ch4.6 |
| 連接其他（MS365/Asana/Linear 等） | Settings → Integrations → 選擇服務 | ★☆☆ | Pro+ | → Ch4.6 |
| 自訂 Remote MCP | Settings → Integrations → Custom MCP URL | ★★★ | Pro+ | → Ch20 |
| **其他核心功能** | | | | |
| 網頁搜尋 | 自動觸發或要求「搜尋 XXX」，附引用來源 | ★☆☆ | Free+ | → Ch9 |
| 檔案上傳 | 迴紋針圖示（30MB/檔，支援 PDF/圖片/CSV/程式碼） | ★☆☆ | Free+ | → Ch9 |
| 圖片理解 | 上傳圖片（最大 8000x8000px，建議 1000x1000+） | ★☆☆ | Free+ | → Ch9 |
| Code Execution | 自動觸發（資料分析、繪圖、程式驗證） | ★☆☆ | Free+ | → Ch9 |
| Extended Thinking | 對話設定 → 開啟（4.6 為 Adaptive Thinking 自動調節） | ★☆☆ | Pro+ | → Ch4.7 |
| 模型切換 | 訊息框下方 → Model 選單 | ★☆☆ | Pro+ | → Ch1 |
| Generative UI | 互動式視覺化元件（2026 年 3 月新增） | ★★☆ | Free+ | → Ch9 |

### 桌面版 (Claude Desktop) 獨佔功能

| 功能 | 操作方式 | 難度 | 方案要求 | 詳見 |
|------|----------|------|----------|------|
| Quick Entry 快速呼叫 | Double-tap Option (Mac) / Alt+Space (Win) | ★☆☆ | Pro+ | → Ch5, Ch14 |
| Voice Mode 語音對話 | Caps Lock 或工具列麥克風圖示（5 種人格） | ★☆☆ | Pro+ | → Ch5 |
| Cowork 協作模式 | 拖拽資料夾 → 啟動自主工作，可多任務同時進行 | ★★☆ | Pro+ | → Ch10 |
| Computer Use 電腦操作 | Settings → Research Preview → 啟用 | ★★★ | Pro+ | → Ch13 |
| Desktop Extensions | 一鍵安裝本地 MCP 伺服器 | ★★☆ | Pro+ | → Ch5, Ch20 |
| Dispatch 跨裝置分發 | 在一台裝置啟動任務，另一台監控 | ★★☆ | Pro+ | → Ch10 |
| Scheduled Tasks 排程任務 | 設定定時執行的任務 | ★★☆ | Pro+ | → Ch10 |

### CLI 斜線指令 (Claude Code)

#### 工作階段管理

| 指令 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `/help` | 顯示指令列表與說明 | ★☆☆ | → Ch11 |
| `/clear` | 清除對話紀錄，重新開始 | ★☆☆ | → Ch11 |
| `/compact [重點]` | 壓縮對話歷史，釋放 context 空間 | ★☆☆ | → Ch11 |
| `/exit` | 結束 Claude Code 工作階段 | ★☆☆ | → Ch11 |
| `/export` | 匯出對話紀錄為 Markdown | ★☆☆ | → Ch11 |
| `/context` | 查看 context 使用率（建議 < 80%） | ★☆☆ | → Ch11 |
| `/cost` | 查看本次工作階段的花費與 token 消耗 | ★☆☆ | → Ch11 |

#### 設定與認證

| 指令 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `/config` | 開啟互動式設定面板 | ★☆☆ | → Ch6 |
| `/init` | 在當前專案自動生成 CLAUDE.md | ★☆☆ | → Ch7 |
| `/login` | 登入 Anthropic 帳號 | ★☆☆ | → Ch6 |
| `/logout` | 登出當前帳號 | ★☆☆ | → Ch6 |
| `/permissions` | 管理工具使用權限 | ★★☆ | → Ch6.3 |
| `/model` | 切換模型（Opus/Sonnet/Haiku） | ★☆☆ | → Ch11 |
| `/effort` | 設定思考深度（low/medium/high/max） | ★★☆ | → Ch11 |
| `/hooks` | 管理生命週期鉤子 | ★★★ | → Ch6 |
| `/terminal-setup` | 設定終端環境（Shift+Enter 等） | ★☆☆ | → Ch6 |
| `/theme` | 切換介面主題 | ★☆☆ | → Ch6 |
| `/doctor` | 診斷環境問題 | ★☆☆ | → Ch29 |

#### 開發工具

| 指令 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `/security-review` | 掃描目前變更的安全風險 | ★★☆ | → Ch11 |
| `/memory` | 管理 CLAUDE.md 記憶 | ★★☆ | → Ch7 |
| `/config` → Editor mode | 啟用 / 停用 Vim 模式 | ★★☆ | → Ch14 |
| `/ide` | 切換 IDE 整合模式 | ★★☆ | → Ch24 |
| `/bug` | 回報 Claude Code 的 bug | ★☆☆ | → Ch11 |
| `/status` | 查看背景任務狀態 | ★☆☆ | → Ch11 |
| `/add-dir` | 新增額外目錄到工作區 | ★☆☆ | → Ch11 |

#### 進階指令

| 指令 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `/fast` | 快速模式（降低思考深度換取速度） | ★★☆ | → Ch11 |
| `/agents` | 管理自訂 agent | ★★★ | → Ch11 |
| `/bashes` | 管理多個 bash 工作階段 | ★★★ | → Ch11 |
| `/loop` | 迴圈執行指令 | ★★★ | → Ch11 |
| `/schedule` | 排程遠端 agent | ★★★ | → Ch23 |

### CLI 命令列參數 (claude 指令)

| 參數 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `-p "提示詞"` | Headless 模式（無互動，適用 CI/CD） | ★★☆ | → Ch11 |
| `--output-format json` | 輸出為 JSON 格式 | ★★☆ | → Ch11 |
| `--output-format stream-json` | 串流 JSON 輸出 | ★★☆ | → Ch11 |
| `--max-budget-usd N` | 設定最大費用上限 | ★★☆ | → Ch26 |
| `--allowedTools "tool1,tool2"` | 限制可用工具 | ★★★ | → Ch11.5 |
| `--json-schema '{...}'` | 強制結構化輸出 | ★★★ | → Ch12 |
| `--fallback-model MODEL` | 備用模型（主模型不可用時切換） | ★★☆ | → Ch11 |
| `--continue` | 繼續上一個工作階段 | ★☆☆ | → Ch11 |
| `--resume SESSION_ID` | 恢復指定工作階段 | ★★☆ | → Ch11 |
| `--fork-session` | 分叉當前工作階段 | ★★☆ | → Ch11 |
| `--name "NAME"` | 命名工作階段 | ★☆☆ | → Ch11 |
| `--from-pr URL` | 從 PR 開始工作 | ★★☆ | → Ch23 |
| `-w` | Worktree 隔離模式 | ★★★ | → Ch11 |
| `--tmux` | 搭配 tmux 平行工作 | ★★★ | → Ch11 |
| `--bare` | 最小模式（跳過自動載入） | ★★★ | → Ch11 |

### API 核心參數 (Messages API)

| 參數 | 類型 | 必須 | 功能 | 詳見 |
|------|------|------|------|------|
| `model` | string | 是 | 模型 ID（claude-opus-4-6-20260401 等） | → Ch12 |
| `messages` | array | 是 | 對話訊息陣列 | → Ch12 |
| `max_tokens` | int | 是 | 最大輸出 token 數 | → Ch12 |
| `system` | string | 否 | 系統提示詞 | → Ch12 |
| `temperature` | float | 否 | 隨機度 0-1（預設 1） | → Ch12 |
| `top_p` | float | 否 | Nucleus sampling | → Ch12 |
| `tools` | array | 否 | 工具定義列表 | → Ch12 |
| `tool_choice` | object | 否 | 強制工具選擇策略 | → Ch12 |
| `thinking` | object | 否 | Extended Thinking（adaptive 推薦） | → Ch12 |
| `output_config` | object | 否 | 結構化輸出（JSON Schema） | → Ch12 |
| `metadata` | object | 否 | 使用者識別（用於濫用偵測） | → Ch12 |
| `stream` | bool | 否 | 啟用 SSE 串流（6 種事件） | → Ch12 |

### API Server-side Tools

| 工具 | 功能 | 難度 | 詳見 |
|------|------|------|------|
| `web_search` | 即時網頁搜尋 | ★☆☆ | → Ch12 |
| `web_fetch` | 抓取指定 URL 內容 | ★☆☆ | → Ch12 |
| `code_execution` | 在沙盒環境執行程式碼 | ★★☆ | → Ch12 |
| `bash` | 執行 bash 指令 | ★★☆ | → Ch12 |
| `text_editor` | 檔案編輯 | ★★☆ | → Ch12 |
| `memory` | 記憶管理 | ★★☆ | → Ch12 |

### API 端點

| 端點 | 方法 | 功能 | 詳見 |
|------|------|------|------|
| `/v1/messages` | POST | 發送對話（核心端點） | → Ch12 |
| `/v1/messages/count_tokens` | POST | 計算 token 數（免費） | → Ch12, Ch25 |
| `/v1/messages/batches` | POST | 批次處理（50% 折扣） | → Ch12, Ch26 |

---

## A-2：按場景分類

### 我想寫程式碼

| 場景 | 推薦做法 | 關鍵設定 | 詳見 |
|------|----------|----------|------|
| 日常編程 | Sonnet + CLAUDE.md + 明確需求 | `/model sonnet` | → Ch6, Ch7 |
| 複雜架構設計 | Opus + Plan 模式 + Extended Thinking | `/effort max` | → Ch17 |
| 程式碼審查 | `/security-review`；完整審查用 `code-review` plugin 或直接請 Claude 檢查 git diff | 視需求加 plugin | → Ch11, Ch22 |
| Bug 修復 | 貼 error log + 相關程式碼 + 上下文 | → Ch19 模板 | → Ch19, Ch29 |
| 重構 | Worktree 隔離 + 分步執行 | `claude -w` | → Ch11 |
| 多檔案修改 | Cowork 模式或 Headless 批次 | Desktop / `-p` | → Ch10, Ch11 |

### 我想寫文章 / 翻譯

| 場景 | 推薦做法 | 關鍵設定 | 詳見 |
|------|----------|----------|------|
| 商業報告 | Formal Style + 角色設定 | Styles → Formal | → Ch4.4, Ch19 |
| 技術文件 | Explanatory Style + Artifacts | 搭配 Project Knowledge | → Ch4.4, Ch9 |
| 創意寫作 | Custom Style + temp 0.7-1.0 | API `temperature` | → Ch16, Ch19 |
| 翻譯 | System Prompt + Few-shot 範例 | 搭配術語表 | → Ch19 模板 |
| 摘要 | Concise Style + 長文放前面查詢放後面 | 30% 品質提升 | → Ch15, Ch16 |

### 我想分析資料

| 場景 | 推薦做法 | 關鍵設定 | 詳見 |
|------|----------|----------|------|
| CSV / Excel 分析 | Code Execution + 明確分析目標 | 上傳檔案 | → Ch9 |
| PDF 報告摘要 | Projects + Vision（< 100 頁最佳） | 搭配 Custom Instructions | → Ch4.2, Ch9 |
| 圖表解讀 | 上傳圖片 + 具體問題 | 建議 1000x1000+ 解析度 | → Ch9 |
| 多文件比對 | 1M Context + XML 標記分隔文件 | `<document>` 包裹 | → Ch15, Ch16 |

### 我想自動化

| 場景 | 推薦做法 | 關鍵設定 | 詳見 |
|------|----------|----------|------|
| 定時任務 | `/schedule` 或 Desktop Scheduled Tasks | Cron 語法 | → Ch23, Ch10 |
| CI/CD 整合 | GitHub Actions + `claude-code-action` | `-p` Headless | → Ch23 |
| 多 Agent 協作 | Agent SDK（Python/TypeScript） | 子 agent 平行化 | → Ch21 |
| 外部服務整合 | MCP 連接器或自訂 MCP 伺服器 | `.mcp.json` | → Ch20 |
| 批次處理管線 | Headless 模式 + 結構化輸出 | `--output-format json` | → Ch11 |

### 我想省錢

| 場景 | 推薦做法 | 預估節省 | 詳見 |
|------|----------|----------|------|
| 選對模型 | 日常用 Sonnet，困難用 Opus | 60% vs Opus | → Ch1, Ch25 |
| 快取命中 | Prompt Caching（重複系統提示詞） | 90% 輸入成本 | → Ch26 |
| 批次折扣 | Batch API（不需即時回應時） | 50% | → Ch26 |
| 快取 + 批次疊加 | 同時使用 Cache + Batch | 95% | → Ch26 |
| 減少輸出 | 系統提示詞加「Be concise」 | 40-60% 輸出 token | → Ch16, Ch25 |
| 定期壓縮 | `/compact` 在 80% 時手動觸發 | 避免重啟浪費 | → Ch11, Ch26 |
| Skills 取代 CLAUDE.md | 按需載入取代全量載入 | 82-98% context | → Ch8 |

---

## A-3：按字母順序（全指令混排）

| 指令 / 功能 | 平台 | 難度 | 一句話說明 | 詳見 |
|-------------|------|------|-----------|------|
| `/add-dir` | CLI | ★☆☆ | 新增額外目錄到工作區 | → Ch11 |
| `/agents` | CLI | ★★★ | 管理自訂 agent | → Ch11 |
| Artifacts | Web | ★☆☆ | 8 種類型的成品生成與編輯 | → Ch9 |
| `/bashes` | CLI | ★★★ | 管理多個 bash 工作階段 | → Ch11 |
| Batch API | API | ★★☆ | 批次處理，50% 折扣 | → Ch12, Ch26 |
| `--bare` | CLI | ★★★ | 跳過自動載入的最小模式 | → Ch11 |
| `/bug` | CLI | ★☆☆ | 回報 Claude Code 的 bug | → Ch11 |
| CLAUDE.md | CLI | ★★☆ | 專案設定檔，4 層架構 | → Ch7 |
| `/clear` | CLI | ★☆☆ | 清除對話，重新開始 | → Ch11 |
| Code Execution | Web/API | ★☆☆ | 沙盒程式碼執行 | → Ch9, Ch12 |
| `/compact` | CLI | ★☆☆ | 壓縮對話歷史 | → Ch11 |
| Computer Use | Desktop/API | ★★★ | 控制電腦操作 | → Ch13 |
| `/config` | CLI | ★☆☆ | 開啟設定面板 | → Ch6 |
| `--continue` | CLI | ★☆☆ | 繼續上一個工作階段 | → Ch11 |
| `/context` | CLI | ★☆☆ | 查看 context 使用率 | → Ch11 |
| `/cost` | CLI | ★☆☆ | 查看花費與 token 消耗 | → Ch11 |
| Cowork | Desktop | ★★☆ | 拖拽資料夾，自主協作 | → Ch10 |
| Custom Instructions | Web | ★☆☆ | 專案指令設定 | → Ch4.3 |
| Desktop Extensions | Desktop | ★★☆ | 一鍵安裝本地 MCP | → Ch5, Ch20 |
| Dispatch | Desktop | ★★☆ | 跨裝置任務分發 | → Ch10 |
| `/doctor` | CLI | ★☆☆ | 環境診斷 | → Ch29 |
| `/effort` | CLI | ★★☆ | 設定思考深度 | → Ch11 |
| `/exit` | CLI | ★☆☆ | 結束工作階段 | → Ch11 |
| `/export` | CLI | ★☆☆ | 匯出對話 | → Ch11 |
| Extended Thinking | Web/API | ★☆☆ | 深度思考模式 | → Ch4.7, Ch12 |
| `/fast` | CLI | ★★☆ | 快速模式 | → Ch11 |
| `--fallback-model` | CLI | ★★☆ | 備用模型 | → Ch11 |
| `--fork-session` | CLI | ★★☆ | 分叉工作階段 | → Ch11 |
| Generative UI | Web/Mobile | ★★☆ | 互動式視覺化元件 | → Ch9 |
| `/help` | CLI | ★☆☆ | 顯示指令說明 | → Ch11 |
| `/hooks` | CLI | ★★★ | 管理生命週期鉤子 | → Ch6 |
| `/ide` | CLI | ★★☆ | 切換 IDE 整合 | → Ch24 |
| `/init` | CLI | ★☆☆ | 自動生成 CLAUDE.md | → Ch7 |
| `--json-schema` | CLI | ★★★ | 強制結構化輸出 | → Ch12 |
| `/login` | CLI | ★☆☆ | 登入帳號 | → Ch6 |
| `/logout` | CLI | ★☆☆ | 登出帳號 | → Ch6 |
| `/loop` | CLI | ★★★ | 迴圈執行指令 | → Ch11 |
| `--max-budget-usd` | CLI | ★★☆ | 費用上限 | → Ch26 |
| MCP Connectors | Web/Desktop | ★☆☆ | 38+ 預建連接器 | → Ch4.6, Ch20 |
| Memory | Web | ★☆☆ | 跨對話記憶系統 | → Ch4.5 |
| `/memory` | CLI | ★★☆ | 管理 CLAUDE.md 記憶 | → Ch7 |
| Messages API | API | ★★☆ | 核心對話端點 | → Ch12 |
| `/model` | CLI | ★☆☆ | 切換模型 | → Ch11 |
| `--name` | CLI | ★☆☆ | 命名工作階段 | → Ch11 |
| `-p` | CLI | ★★☆ | Headless 無互動模式 | → Ch11 |
| `/permissions` | CLI | ★★☆ | 管理工具權限 | → Ch6.3 |
| Projects | Web | ★☆☆ | 專案管理 | → Ch4.2 |
| Prompt Caching | API | ★★☆ | 快取重複提示詞，省 90% | → Ch12, Ch26 |
| Quick Entry | Desktop | ★☆☆ | 全域快速呼叫 | → Ch5, Ch14 |
| `/security-review` | CLI | ★★☆ | 安全審查 pending changes | → Ch11 |
| `--resume` | CLI | ★★☆ | 恢復指定工作階段 | → Ch11 |
| `/schedule` | CLI | ★★★ | 排程遠端 agent | → Ch23 |
| Scheduled Tasks | Desktop | ★★☆ | 定時任務 | → Ch10 |
| Skills | CLI | ★★☆ | 領域知識系統 | → Ch8 |
| `/status` | CLI | ★☆☆ | 查看背景任務狀態 | → Ch11 |
| Styles | Web | ★☆☆ | 4 預設 + 自訂風格 | → Ch4.4 |
| `/terminal-setup` | CLI | ★☆☆ | 終端環境設定 | → Ch6 |
| `/theme` | CLI | ★☆☆ | 介面主題切換 | → Ch6 |
| Token Counting | API | ★☆☆ | `/v1/messages/count_tokens`（免費） | → Ch12, Ch25 |
| `/config` → Editor mode | CLI | ★★☆ | Vim 模式切換 | → Ch14 |
| Voice Mode | Desktop/Mobile | ★☆☆ | 語音對話（5 種人格） | → Ch5 |
| Web Search | Web/API | ★☆☆ | 即時網頁搜尋 | → Ch9, Ch12 |
| `-w` | CLI | ★★★ | Worktree 隔離模式 | → Ch11 |

---

> TIP：本表列出最常用的指令與功能。完整細節請翻閱對應章節。
> 本表資訊基準日期：2026-04-05
