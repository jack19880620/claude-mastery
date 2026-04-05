---
name: code-review
description: >
  執行程式碼審查，專注於安全漏洞和邏輯錯誤。
  當用戶請求 code review、審查、review、安全檢查時使用。
user-invocable: true
allowed-tools:
  - Read
  - Grep
  - Glob
  - Bash(git diff:*)
---

## 程式碼審查標準

### 必查項目
1. SQL Injection — 所有資料庫查詢必須用參數化
2. XSS — 所有用戶輸入必須轉義
3. 未驗證的使用者輸入 — 信任邊界外的一切都要驗證
4. 敏感資料外洩 — API key、密碼不能 hardcode
5. 認證缺陷 — session 管理、token 過期

### 審查格式
每個問題用以下格式回報：
- **嚴重度**：Critical / Warning / Info
- **位置**：file:line_number
- **問題**：一句話描述
- **修復**：具體的程式碼修改建議

### 審查流程
1. 先跑 git diff 看所有改動
2. 逐檔案審查
3. 跨檔案邏輯一致性檢查
4. 最後產出摘要報告
