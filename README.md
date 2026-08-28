# Agentic AI Foundations — 課程重點摘要圖卡

AWS 官方課程 **Agentic AI Foundations**（課程代碼 `100-MLAGAF-11-EN`，ILT 講師投影片 v1.1.9）Module 1–7 的視覺化重點摘要，依原始投影片內容整理製作。

## 如何瀏覽

打開 `index.html`（雙擊或用瀏覽器開啟即可，離線可用），即可看到七張圖卡的索引首頁，點擊任一張卡片會**以新視窗開啟**該模組的完整摘要圖卡。

## 檔案結構

```
summary-cards/
├── index.html                                    索引首頁（開啟入口）
├── README.md                                      本說明文件
├── course-metro-map.html                          課程議程捷運路線圖
├── module-01-from-llms-to-agents.html             Module 1：From LLMs to Agents
├── module-02-exploring-agentic-ai.html            Module 2：Exploring Agentic AI
├── module-03-agentic-ai-workflows.html            Module 3：Understanding Agentic AI Workflows
├── module-04-aws-dev-productivity-tools.html      Module 4：AWS Agentic Development & Productivity Tools
├── module-05-agentic-ai-frameworks-agentcore.html Module 5：Agentic AI Frameworks & Bedrock AgentCore
├── module-06-customizing-agentic-solutions.html   Module 6：Customizing Agentic Solutions
└── module-07-course-wrap-up.html                  Module 7：Course Wrap-Up
```

每個檔案都是**單一自包含的 HTML**（CSS／字型連結／內容都在同一檔案內），可獨立開啟、分享或列印，不需要額外的資源檔。

## 課程路線圖（Course Metro Map）

`course-metro-map.html` 把官方一日課程議程表畫成「捷運路線圖」：12 個停靠站依時間順序排列，圖示區分模組（圓點）、實作 Lab（雙圈）與午餐（小站），並列出總時長、模組數、實作／示範時數、休息時數等統計。RWD 響應式設計：桌面為橫向蛇行路線，手機自動切換為直向單線路線，並支援直接列印。

依議程表製作，總時長 **7.75 小時**（不含午餐；含午餐總時長 8 小時 45 分）：

| 時段 | 項目 | 時間 |
|---|---|---|
| M0 | Course and Student Introductions | 15 分 |
| M1 | From LLMs to Agents | 45 分 |
| M2 | Exploring Agentic AI | 45 分 |
| M3 | Understanding Agentic AI Workflows | 25 分 |
| M4 | Introducing Autonomous Agents | 50 分 |
| — | 午餐 LUNCH | 60 分 |
| Lab | Accelerating Software Development using Kiro | 60 分 |
| M5 | Amazon Q and Agentic Development Tools | 45 分 |
| Lab | Building Your First AI Agent with Strands Agents SDK | 60 分 |
| M6 | Agentic AI with Amazon Bedrock | 60 分 |
| M7 | Building DIY Solutions | 45 分 |
| M8 | Course Wrap-up | 15 分 |

> **注意**：此議程表的模組編號／名稱（M0–M8，9 個模組）來自使用者提供的官方課程議程，與上方 M1–M6 摘要圖卡所依據的投影片版本（`100-MLAGAF-11-EN-PPTX.1.1.9-20260804153132`，M0–M7，8 個模組）在部分模組命名與拆分上不完全一致，應為不同課程改版。兩者暫未一一對應，如需要可再協助校對整合。

## 各模組涵蓋重點

| 模組 | 標題 | 涵蓋重點 |
|---|---|---|
| M1 | From LLMs to Agents | LLM 的侷限、驅動 Agent 發展的四項創新、從 LLM 到 Agentic AI 系統的演進、自主性四等級（L1–L4） |
| M2 | Exploring Agentic AI | Agentic 系統的三個架構元件（感知／推理／行動）、常見工具類型、四種 Agent 類型比較、貫穿全課程的 Email Agent 案例 |
| M3 | Understanding Agentic AI Workflows | 四種工作流模式（串聯／平行化／路由／協調）、客服工單實戰範例、Amazon Bedrock Flows |
| M4 | AWS Agentic Development & Productivity Tools | AWS Agentic 服務堆疊、Amazon Quick Suite、Amazon Q Developer 的 SDLC 流程、Kiro spec-driven 開發 |
| M5 | Agentic AI Frameworks & Bedrock AgentCore | 四大開源框架比較（CrewAI／LangGraph／LlamaIndex／Strands）、用 Strands Agents 建立 Agent、Amazon Bedrock AgentCore 七大核心元件 |
| M6 | Customizing Agentic Solutions | 產業客製化案例、AWS 客製化基礎架構堆疊、CloudWatch 可觀測性、A2A 與 MCP 互通協定比較 |
| M7 | Course Wrap-Up | 全課程學習成果總覽（11 項）、AWS Skill Builder 持續學習資源、AWS 認證分級、考試準備四步驟 |

> Module 0（課程介紹，行政性質）暫未納入本套摘要圖卡；如需要可再另行製作。

## 內容校對記錄

2026-08-28：逐頁比對六張圖卡（M2、M4、M5、M6）與原始投影片，補齊先前遺漏的重點：

- **M2**：新增「技術演進」（技術驅動因素、POC → Production → Scale 導入階段、技術挑戰）
- **M4**：Quick Suite 六項能力補上個別說明；新增 Q Developer 介紹、六項典型使用情境、CLI Agentic 指令能力
- **M5**：新增 AgentCore Browser／Code Interpreter 應用案例
- **M6**：新增 Model Invocations 儀表板、跨應用程式可觀測性（Service Maps）、Agent Card 關鍵屬性、MCP 三大核心概念（Resources／Prompts／Tools）；A2A 四項能力與 A2A／MCP 本質差異補充完整；Module summary 學習目標由 5 項補齊為 7 項

同時新增 **Module 7（Course Wrap-Up）** 摘要圖卡，完成 M1–M7 全套。

## 資料來源

`ILT-TF-100-MLAGAF-11-EN_M01–M07_InstructorDeck.pptx`（AWS 官方講師投影片，位於上層 `100-MLAGAF-11-EN-PPTX.1.1.9-20260804153132/` 資料夾）。

---
由 Claude 依投影片內容分析整理製作。
