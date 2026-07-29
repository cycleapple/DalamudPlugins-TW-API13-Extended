# zh-TW 介面本地化稽核

本文件追蹤 Extended repo 內所有插件的繁體中文介面翻譯。翻譯基準為台灣 FFXIV 7.3 客戶端用語，遊戲固有名詞優先參考 [HoshinoCorp/ffxiv-datamining-tc](https://github.com/HoshinoCorp/ffxiv-datamining-tc)。

## 修改界線

允許修改：

- 視窗標題、頁籤、按鈕、核取方塊、輸入欄位標籤
- 工具提示、設定名稱、設定說明、錯誤提示與指令說明
- 專門用於顯示的 `.resx`、i18n JSON、語言檔及 UI 常數
- manifest 的顯示名稱、簡介與說明

禁止修改：

- Signature、hook、offset、IPC 名稱與 InternalName
- 指令本身、設定鍵、序列化欄位、資料格式與網路協定
- 用於遊戲選單點選、Regex、文字解析或精確比對的字串
- Excel/Lumina 查詢條件、遊戲物件 ID、資料 ID、路徑與檔名
- 格式化 placeholder；例如 `{0}`、`{name}`、`<link>`、`##ImGuiId`

若同一字串同時負責顯示與功能判斷，先拆分顯示字串；無法安全拆分時保留原文並記錄原因。

## 進度

| 插件 | 狀態 | 備註 |
|---|---|---|
| AntiAfkKick | 待處理 | 硬編碼 UI |
| Saucy | 待處理 | 需盤點主 UI 與 Triple Triad 語言資料 |
| NoClippy | 待處理 | 硬編碼 UI |
| Pixel Perfect | 待處理 | 硬編碼 UI |
| Price Insight | 待處理 | 硬編碼 UI |
| Wrath Combo | 待處理 | 大型硬編碼 UI |
| Splatoon | 待複核 | 已有 Chinese 語言檔，需轉為台服用語 |
| AutoRetainer | 待複核 | 已有局部台服文字修正 |
| NecroLens | 待處理 | 需建立 zh-TW 資源 |
| TextAdvance | 待複核 | 已有 `Lang.cs`，需隔離功能比對字串 |
| Lifestream | 待複核 | 已有局部台服文字修正 |
| YesAlready | 待處理 | 大型硬編碼 UI |
| LazyLoot | 待處理 | 硬編碼 UI |
| Burning Down the House | 待處理 | 硬編碼 UI |
| Raphael.Dalamud | 待處理 | 硬編碼 UI |
| Something Need Doing | 待處理 | 大型硬編碼 UI |
| GatherBuddy Reborn | 待複核 | 需區分 UI 與採集資料 |
| Artisan | 待複核 | 已有局部台服文字修正 |
| AutoDuty | 待處理 | 大型硬編碼 UI |
| Rotation Solver Reborn | 待處理 | 大型 UI 與職業術語 |
| Boss Mod | 待處理 | 大型 UI 與戰鬥術語 |
| Bossmod Reborn | 待處理 | 大型 UI 與戰鬥術語 |
| vnavmesh | 待處理 | 硬編碼 UI |
| MidiBard 2 | 待複核 | 已有 zh-Hant 資源 |
| Questionable | 待處理 | 大型 UI 與任務術語 |
| Gearsetter | 待處理 | 裝備與屬性術語 |
| Ice's Cosmic Exploration | 待複核 | 需盤點既有翻譯資料 |
| BOCCHI | 待複核 | 已有 i18n 架構 |
| Umbra XIV | 待複核 | 已有 `zh.json` |
| MissFisher | 待複核 | 已有 `lang.json` |
| Skippy | 待處理 | 硬編碼 UI |
| AutoHook | 待複核 | 已有中文 `.resx` |
| Avarice | 待處理 | 硬編碼 UI |
| Orbwalker | 待處理 | 硬編碼 UI |
| Palace Pal | 待處理 | 已有資源架構但沒有中文資源 |
| Pandora's Box | 待處理 | 大型硬編碼 UI |
| Marketbuddy | 待處理 | 硬編碼 UI |
| JobBars | 待處理 | 硬編碼 UI |
| NotificationMaster | 待處理 | 硬編碼 UI |
| CBT / Automaton | 待處理 | 大型模組化 UI |
| GatheringPathRenderer | 待處理 | 硬編碼 UI |
| Deliveroo | 待處理 | 硬編碼 UI |
| Chilled Leves | 待處理 | 硬編碼 UI |
| Explorer's Icebox | 待處理 | 硬編碼 UI |
| Easier Faux Hollows | 待處理 | 硬編碼 UI |
| Hyperborea | 待處理 | 硬編碼 UI |
| AutoMinion | 待處理 | 小型硬編碼 UI |
| XIV 藏寶圖工具小幫手 | 待複核 | 既有繁中介面，需術語稽核 |
| Visland | 待處理 | 大型硬編碼 UI |
| Chat 2 | 第一輪完成 | 426 個 zh-Hant 鍵齊全；清除非技術性殘留英文並校訂明顯非台灣用語 |
| Doorbell | 完成 | 設定 UI、工具提示、指令說明、狀態訊息及預設通知已翻譯 |

## 驗證要求

每一批都必須：

1. 比對翻譯資源鍵與基準語言鍵，確認無缺漏。
2. 搜尋殘留英文及簡體／異體用字並人工判定。
3. 以台服 Dalamud API13 與 TC-BASE 相依套件編譯。
4. 檢查 ZIP manifest 的 InternalName、版本與 API13。
5. 上傳 GitHub release 後重新下載並核對 SHA-256。
