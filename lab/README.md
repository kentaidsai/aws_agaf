# Task 2：Build Your First AI Agent — 實驗室摘要

本資料夾包含 AWS「Agentic AI Foundations」課程中 **Task 2** 的實作筆記本，說明如何使用 **Strands Agents** 框架，搭配 **Amazon Bedrock（Amazon Nova Lite 模型）** 建立你的第一個 AI 代理程式（AI Agent），並附有逐步解析文件、簡報與網頁版整理成果。

## 檔案內容

| 檔案 | 說明 |
| --- | --- |
| `Task.ipynb` | 英文版筆記本，共 28 個 cell |
| `Task_zh_TW.ipynb` | 繁體中文版筆記本，內容與英文版完全對應（markdown 說明已翻譯，程式碼相同），共 28 個 cell |
| `Task_逐步詳細解析.md` | 針對 `Task.ipynb` 全部 28 個 cell 的逐步詳細解析，每個任務先講「目的」再逐格說明程式碼邏輯，並附完整流程圖（Mermaid） |
| `Task_AI_Agent_解析.pptx` | 13 頁簡報版，將逐步解析整理成投影片，含任務說明、程式碼重點、temperature 滑桿視覺化、流程圖等 |
| `index.html` | 響應式網頁版（RWD），支援手機／深色模式，離線可直接雙擊開啟瀏覽，內容與簡報一致 |

兩份筆記本內容與結構完全一致，僅語言不同，可依需求擇一使用；`Task_逐步詳細解析.md`、`.pptx`、`.html` 三者內容一致，僅呈現形式不同（文件／簡報／網頁），可依使用情境（自讀、對外簡報、離線瀏覽）選用。

## 情境設定

你任職於 AnyCompany，一家正在成長的科技公司，希望探索 AI 代理程式如何協助自動化日常任務（例如研究、客戶支援）。本實驗室從建立智慧代理程式的基礎概念開始。

AI 代理程式與傳統 LLM 的差異在於：代理程式能夠自發採取動作、使用工具、朝目標運作，而不僅是回答問題。

## 各任務重點

1. **Task 2.1：環境設定** — 安裝 `strands-agents` 與 `strands-agents-tools` 套件。
2. **Task 2.2：建立第一個 AI 代理程式** — 使用 `strands.Agent` 搭配 `amazon.nova-lite-v1:0` 模型，設定 `system_prompt` 建立一個對話式代理程式，並發送訊息測試（例如請它講笑話）。
3. **Task 2.3：為代理程式新增工具**
   - 加入 Strands SDK 內建的 `calculator` 計算器工具。
   - 使用 `@tool` 裝飾器自訂一個 `weather` 天氣工具（僅為示範用的預留位置，固定回傳「Sunny」）。
   - 測試代理程式如何依問題內容自動判斷該使用哪個（或哪些）工具，並示範以 `agent.tool.tool_name()` 直接呼叫工具，略過代理程式的自然語言判斷流程。
4. **Task 2.4：設定記錄（Logging）** — 使用 Python 標準 `logging` 模組，設定日誌層級以觀察代理程式的內部運作與工具呼叫過程。
5. **Task 2.5：探索模型組態** — 透過 `BedrockModel` 自訂模型參數（例如 `temperature`），瞭解溫度值如何影響回應的一致性與創造性。
6. **Task 2.6：建立食譜助理代理程式** — 安裝 `ddgs` 套件並建立 `websearch` 工具，串接 DuckDuckGo 網路搜尋，打造一個名為 **RecipeBot** 的食譜助理，能上網搜尋食譜與烹飪資訊來回答使用者問題（範例：建議一道雞肉花椰菜料理）。

> 完整逐步說明（含每格程式碼的詳細解讀與流程圖）請見 `Task_逐步詳細解析.md`，或直接開啟 `index.html` 網頁版／`Task_AI_Agent_解析.pptx` 簡報版瀏覽。

## 使用的技術/套件

- **Strands Agents 框架**（`strands`、`strands-agents-tools`）
- **Amazon Bedrock**：`amazon.nova-lite-v1:0`（Amazon Nova Lite 模型）
- **ddgs**：DuckDuckGo 網路搜尋套件，用於 websearch 工具
- Python 標準函式庫：`logging`、`warnings`

## 學習成果

完成本實驗室後，你將學會：

- 如何使用 Strands Agents 框架建立可對話的 AI 代理程式。
- 如何為代理程式加入內建工具與自訂工具（含直接呼叫工具的方式）。
- 如何啟用日誌記錄以觀察代理程式的決策與工具使用過程。
- 如何調整模型參數（如 temperature）來控制回應風格。
- 如何整合外部網路搜尋能力，打造具備實際應用價值的代理程式（食譜助理）。

## 延伸練習

- 修改 `system_prompt`，打造適用於不同情境的代理程式。
- 為團隊實際需求設計自訂工具。
- 嘗試不同的模型組態，觀察對代理程式行為的影響。

---
*本 README 由分析 `Task.ipynb` 與 `Task_zh_TW.ipynb` 兩份筆記本內容，並整合逐步解析文件、簡報與網頁版產出後自動整理產生。*
