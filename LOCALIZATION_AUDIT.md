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
| Splatoon | 已完成 | 3.8.2.3；保留 301 個查詢鍵，只轉換 `==` 右側顯示值；延伸 MapEffect multisig 已針對台服 7.3 修正 |
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
| JobBars | 已完成 | 1.3.2.3；完成主要設定、各職業量譜細項與自訂冷卻對話框；保留與設定值相連的 enum 名稱 |
| NotificationMaster | 已完成 | 2.1.1.13；完成主要設定、聊天規則、狩獵目標與實際通知介面；保留 HTTP／XivChatType 等功能識別值 |
| CBT / Automaton | 待處理 | 大型模組化 UI |
| GatheringPathRenderer | 待處理 | 硬編碼 UI |
| Deliveroo | 待處理 | 硬編碼 UI |
| Chilled Leves | 已完成 | 1.0.1.20；完成主要與工作清單進階介面；保留純 Debug 與品牌／格式名稱 |
| Explorer's Icebox | 待處理 | 硬編碼 UI |
| Easier Faux Hollows | 待處理 | 硬編碼 UI |
| Hyperborea | 已完成 | 1.0.0.33；完成主要設定與區域編輯器；保留 opcode／MapEffect／CFC 等底層術語 |
| AutoMinion | 完成 | 設定視窗、固定模式、搜尋、按鈕、指令說明與插件說明已翻譯；未更動寵物名稱、指令內容與地區 ID |
| XIV 藏寶圖工具小幫手 | 待複核 | 既有繁中介面，需術語稽核 |
| Visland | 待處理 | 大型硬編碼 UI |
| Chat 2 | 第一輪完成 | 426 個 zh-Hant 鍵齊全；清除非技術性殘留英文並校訂明顯非台灣用語 |
| Doorbell | 完成 | 設定 UI、工具提示、指令說明、狀態訊息及預設通知已翻譯 |
| MultiHit | 完成 | 設定視窗、技能群組編輯、按鈕、工具提示、對話框及指令說明已翻譯；未更動匯入格式與內部識別碼 |
| Namingway | 完成 | 套組管理、匯入／匯出、搜尋、欄位標題、指令說明與預設套組顯示名稱已翻譯；未更動技能／狀態改名內容、GUID 與 JSON 格式 |
| Mappy | 完成 | 3.1.6.12；設定、地圖工具列、右鍵選單、座標列、地圖搜尋、任務／危命任務／旗標視窗、標記提示與劇透警告已翻譯；未更動地圖座標換算、標記資料、遊戲地名與設定鍵 |
| ChatCoordinates | 完成 | 2.1.2.10；設定、指令說明、聊天提示、錯誤訊息與範例已翻譯；官方地名採用「雷克蘭德」；未更動座標解析、分隔符號與傳送參數 |
| FPS Plugin | 完成 | 1.7.0.5；設定介面、字型選項、DTR 工具提示、平均／最低標籤與指令說明已翻譯；未更動指令參數與 FPS 計算邏輯 |
| Craftimizer | 待處理 | 已翻譯 manifest；大型製作模擬與巨集介面待後續處理 |
| SortaKinda | 完成 | 2.1.1.7；排序規則、篩選器、設定視窗、物品欄按鈕、工具提示、通知與教學頁已翻譯；未更動規則序列化格式、內部識別碼、正規表示式內容與物品搬動邏輯 |
| QoL Bar | 完成 | 2.3.3.7；已翻譯主設定、快捷列／捷徑編輯、條件組、職業與區域條件、備份、圓盤選單、圖示瀏覽器、快捷鍵、提示與錯誤訊息；指令語法、條件 ID、IPC、匯出資料與設定序列化未變更 |
| IINACT | 部分完成 | 1.13.9.3；採用使用者指定的台服 API13 分支並翻譯 manifest；上游已有部分繁中語言調整，完整介面仍待稽核 |
| LMeter | 完成 | 1.13.0.3；已翻譯設定、設定檔、長條、文字、字型、顯示條件、ACT 連線狀態、統計視窗與右鍵選單；IPC 端點、ACT 欄位、格式標籤、設定資料與計算邏輯未變更 |
| Distance | 已完成 | 1.1.3.6；完成主要與進階 Widget／Arc／名牌介面；純 Debug 視窗保留英文 |
| EnemyListHP | 已完成 | 2.0.1.8；完成設定介面與 manifest |
| ReAction | 已完成 | 1.3.4.4；完成主要、Help、連段、快捷欄與佇列介面；內部 log／debug 保留英文 |
| Radar Plugin | 已完成 | 2.1.8.3；完成主要與進階雷達介面；MobEdit 診斷欄位與內部 debug 保留英文 |
| ReMakePlace Plugin | 已完成 | 7.3.4.0；完成房屋配置介面翻譯，保留家具 fixture 與功能判斷值 |
| DozeAnywhere | 已完成 | 13.1.0.1；完成可見介面與通知翻譯 |
| Cammy | 已完成 | 2.1.0.14；完成預設、鏡頭、自由鏡頭與進階設定介面 |
| Gauge-O-Matic | 已完成 | 0.8.2.3；完成 Help、Preset、職業調整、tooltip 與 widget 進階介面；功能分支鍵保持英文 |
| EngageTimer | 已完成 | 2.4.4.1；完成 zh-TW／zh-Hant 語系支援並補齊設定介面 |
| BigPlayerDebuffs | 已完成 | 1.1.0.14；完成設定、命令說明與 manifest |
| Better Mount Roulette | 已完成 | 1.0.0.2；完成主要設定、坐騎群組、角色管理、命令說明與錯誤回饋；命令 token 保持原樣 |
| Submarine Tracker | 待處理 | 本批先完成 API13 安全節點、依賴漏洞修正與繁中 repo 說明；插件內部介面尚未進行 zh-TW 翻譯 |
| Party Icons | 待處理 | 本批先完成 API13 編譯與繁中 repo 說明；插件設定介面尚未進行 zh-TW 翻譯 |
| RezPls | 待處理 | 本批先完成 API13 編譯與繁中 repo 說明；插件設定介面尚未進行 zh-TW 翻譯，未更動復活、狀態效果判斷或介面覆蓋邏輯 |

## 驗證要求

每一批都必須：

1. 比對翻譯資源鍵與基準語言鍵，確認無缺漏。
2. 搜尋殘留英文及簡體／異體用字並人工判定。
3. 以台服 Dalamud API13 與 TC-BASE 相依套件編譯。
4. 檢查 ZIP manifest 的 InternalName、版本與 API13。
5. 上傳 GitHub release 後重新下載並核對 SHA-256。
