# Repository Memory

## Stable Context
- **Repository**: `xz9254442-alt/bao`  
  - 監控所有 Issue（`state: all`），上限 100 件，回溯最近 30 天。  
- **資料來源**：所有原始資訊皆來自 GitHub Issue / Comment，`shared/manual.md` 只作為長期規則與限制的參考，不會被自動覆寫。  
- **Agent 角色**  
  - **前端捕捉（2 號機）**：即時接收主人指令，使用 `agent‑browser` 等技能在網路上搜尋、抓取、摘要資訊，並以 Markdown 回報。  
  - **需求中樞（初號機）**：作為新建的「需求接收」節點，列出 15 項可用技能（`agent‑browser、audio‑transcriber、deep‑researcher…`），等待主人或其他協作者分派任務。  
- **工作流程**  
  1. 主人下達指令（如 Telegram） → 由前端捕捉機即時執行。  
  2. 取得初步結果 → 以簡短摘要回報，待主人確認。  
  3. 主人批准後，前端機可進一步取得全文、深化整理或交由其他 agent 處理。  
- **回報格式**：使用 Markdown，必要時加入文言文風格或其他指定語氣。  
- **限制**：  
  - 不得直接複製 Issue 原文於長期記憶檔案。  
  - `shared/manual.md` 只作為「穩定規則」與「共同行為」的參考，任何自動化流程不會改寫此檔。  
  - 若資訊不確定或僅在單日出現，須標記為「暫時」或「待確認」而非寫成永久規則。  

## Recent Themes
- **即時資訊抓取與摘要**  
  - 2 號機在 2026‑03‑21
