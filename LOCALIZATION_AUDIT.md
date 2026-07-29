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
| AntiAfkKick | 完成 | 插件本身無設定介面；安裝頁說明與摘要已翻譯 |
| Saucy | 完成 | 主介面、統計、九宮幻卡、重擊伽美什、孤樹無援與其他遊戲提示已翻譯；修正 zh 語言檔未嵌入 DLL；未更動遊戲文字比對、Excel 資料、正規表示式與 Hook |
| NoClippy | 完成 | 設定、技能後搖、戰鬥統計、記錄選項、狀態預測警告與指令回覆已翻譯；未更動指令參數、封包與 Hook 邏輯 |
| Pixel Perfect | 完成 | 歡迎頁、設定條件、圖形參數、匯入／匯出、通知、編輯器與說明已翻譯；未更動設定格式與繪圖邏輯 |
| Price Insight | 已完成 | 2.11.3.1；設定介面與市場佈告板物品說明繁中化 |
| Wrath Combo | 待處理 | 大型硬編碼 UI |
| Splatoon | 已完成 | 3.8.2.2；保留 301 個查詢鍵，只轉換 `==` 右側顯示值 |
| AutoRetainer | 待複核 | 已有局部台服文字修正 |
| NecroLens | 待處理 | 需建立 zh-TW 資源 |
| TextAdvance | 已完成 | 3.2.4.8；介面、通知與聊天狀態繁中化；`Lang.cs` 功能比對字串保持不動 |
| Lifestream | 待複核 | 已有局部台服文字修正 |
| YesAlready | 待處理 | 大型硬編碼 UI |
| LazyLoot | 已完成 | 5.3.2.5；設定、限制規則、指令說明、狀態列、擲骰結果與診斷訊息已翻譯；未更動 `need`／`greed`／`pass` 等指令參數、設定格式與擲骰邏輯 |
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
| MidiBard 2 | 已完成 | 3.2.1.3；zh-Hant 介面鍵 213/213，補齊 14 個缺漏字串 |
| Questionable | 待處理 | 大型 UI 與任務術語 |
| Gearsetter | 待處理 | 裝備與屬性術語 |
| Ice's Cosmic Exploration | 待複核 | 需盤點既有翻譯資料 |
| BOCCHI | 已完成 | 1.0.1.1；22 份 zh 語系資源完整，補齊 2 個缺漏值並轉為台灣繁中 |
| Umbra XIV | 已完成 | 3.1.7.1；`zh.json` 介面鍵 1568/1568，轉為台灣繁中 |
| MissFisher | 已完成 | 1.6.5.12；保留 556 個查詢鍵，只轉換內嵌 `lang.json` 的中文顯示值 |
| Skippy | 待處理 | 硬編碼 UI |
| AutoHook | 已完成 | 5.0.0.14；中文介面鍵 475/475，轉為台灣繁中並補齊 23 個缺漏字串 |
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
| AutoMinion | 完成 | 設定視窗、固定模式、搜尋、按鈕、指令說明與插件說明已翻譯；未更動寵物名稱、指令內容與地區 ID |
| XIV 藏寶圖工具小幫手 | 待複核 | 既有繁中介面，需術語稽核 |
| Visland | 待處理 | 大型硬編碼 UI |
| Chat 2 | 第一輪完成 | 426 個 zh-Hant 鍵齊全；清除非技術性殘留英文並校訂明顯非台灣用語 |
| Doorbell | 完成 | 設定 UI、工具提示、指令說明、狀態訊息及預設通知已翻譯 |
| MultiHit | 完成 | 設定視窗、技能群組編輯、按鈕、工具提示、對話框及指令說明已翻譯；未更動匯入格式與內部識別碼 |
| Namingway | 完成 | 套組管理、匯入／匯出、搜尋、欄位標題、指令說明與預設套組顯示名稱已翻譯；未更動技能／狀態改名內容、GUID 與 JSON 格式 |
| Mappy | 待處理 | 已翻譯 manifest；設定與地圖介面待後續處理 |
| ChatCoordinates | 待處理 | 已翻譯 manifest；指令說明與設定介面待後續處理 |
| FPS Plugin | 待處理 | 已翻譯 manifest；設定介面待後續處理 |

## 驗證要求

每一批都必須：

1. 比對翻譯資源鍵與基準語言鍵，確認無缺漏。
2. 搜尋殘留英文及簡體／異體用字並人工判定。
3. 以台服 Dalamud API13 與 TC-BASE 相依套件編譯。
4. 檢查 ZIP manifest 的 InternalName、版本與 API13。
5. 上傳 GitHub release 後重新下載並核對 SHA-256。
