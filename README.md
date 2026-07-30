# DalamudPlugins-TW-API13-Extended

> [!WARNING]
> 本倉庫收錄的插件相對高風險，部分功能涉及遊戲記憶體 Hook、自動化操作或非官方介面。遊戲、Dalamud 或台服客戶端更新後，插件可能立即失效、造成遊戲崩潰、角色操作異常或資料損壞。使用第三方插件亦可能違反遊戲服務條款並帶來帳號處分風險。請自行評估並承擔使用風險，重要設定務必先行備份；遊戲更新後，在相容性重新確認前請停用本倉庫插件。

台服 FFXIV 使用的 Dalamud API13 擴充插件倉庫。本倉庫與外觀插件用的
[DalamudPlugins-TW](https://github.com/cycleapple/DalamudPlugins-TW) 分開維護。

## 安裝網址

在 Dalamud 的「自訂插件儲存庫」加入：

```text
https://raw.githubusercontent.com/cycleapple/DalamudPlugins-TW-API13-Extended/main/repo.json
```

## 支持維護

如果這個插件倉庫對你有幫助，歡迎[請我喝一杯咖啡](https://portaly.cc/thecy) ☕

## 收錄範圍

| 插件 | 目標版本 | 用途 | 狀態 |
|---|---:|---|---|
| Boss Mod | 0.1.4.3 | Boss 機制輔助 | 已發布；一般使用者介面 zh-TW 完成 |
| Bossmod Reborn | 7.3.8.5 | 技能範圍與戰鬥輔助 | 已發布；一般使用者介面 zh-TW 完成 |
| Rotation Solver Reborn | 7.3.5.3 | 技能循環 | 已發布；使用者介面 zh-TW 完成 |
| Splatoon | 3.8.2.5 | 場景繪製點、線、面 | 已發布；使用者介面 zh-TW 完成；保留台服 7.3 MapEffect hooks |
| Wrath Combo | 1.0.1.24 | 整合連段 | 已發布；補齊功能清單與職業設定 zh-TW；修正繁中名稱影響 Questionable 戰鬥 IPC 分類 |
| AntiAfkKick | 2.1.0.10 | 防止閒置斷線 | 已發布；繁中插件說明，插件本身無設定介面 |
| AutoRetainer | 4.5.1.29 | 雇員相關功能 | 已發布；補齊物品欄整理清單、工房航線工具、浮層、通知、操作選單與登入覆蓋層服務帳戶選擇等 zh-TW 介面 |
| Saucy | 1.4.2.9 | 金碟相關功能 | 已發布；完成 zh-TW 主介面與九宮幻卡資源翻譯 |
| NoClippy | 0.5.0.20 | 改善技能延遲 | 已發布；完成 zh-TW 介面翻譯 |
| NecroLens | 1.0.8.13 | 深層迷宮輔助 | 已發布；92 個介面資源鍵已完整轉為台灣繁中，並補上本地化協助與匿名資料收集說明；保留 API13 型別相容修補 |
| MidiBard 2 | 3.2.1.3 | 樂器演奏 | 已發布；API14 型別誤用前的安全節點；補齊 zh-TW 介面資源 |
| GatherBuddy Reborn | 7.3.5.4 | 採集輔助 | 已發布；修正下次時間欄位的 GBK／UTF-8 亂碼，時間單位與狀態顯示正常 |
| Artisan | 4.0.4.18 | 生產輔助 | 已發布；修正素材清單即時更新、半成品抵扣統計及快速編輯造成的舊資料覆蓋 |
| Burning Down the House | 1.7.1.2 | 房屋裝修 | 已發布；補齊指令說明、家具清單標題與座標欄位 |
| Raphael.Dalamud | 0.0.5.1 | 生產求解器／依賴庫 | 已發布；無設定視窗，已完成 manifest zh-TW 翻譯 |
| Something Need Doing | 0.0.0.1 | 巨集擴展 | 已發布；完成設定、說明、彈窗與 manifest zh-TW 翻譯 |
| TextAdvance | 3.2.4.8 | 對話自動處理 | 已發布、繁中介面 |
| Lifestream | 2.5.3.8 | 傳送輔助 | 已發布；台服世界選單直接依 ID 顯示，修正巴哈姆特因同名舊資料遭排除 |
| vnavmesh | 1.1.2.3 | 尋路與移動工具 | 已發布；完成主要介面 zh-TW；依 festival/layout 階段套用月面客製路徑，修正台服 7.3 月面 polygon 對應失敗 |
| AutoDuty | 0.0.0.7 | 副本自動化框架 | 已發布 API13；修正 Rotation Solver Reborn AutoDuty 模式 IPC 值錯位，並完成一般使用者介面 zh-TW |
| Pixel Perfect | 3.3.2.1 | 顯示角色碰撞圈 | 已發布；完成 zh-TW 介面翻譯 |
| LazyLoot | 5.3.2.5 | 戰利品擲骰輔助 | 已發布；完成 zh-TW 介面、指令說明與診斷訊息翻譯 |
| Questionable | 13.68.129.6 | 任務輔助 | 已發布；使用者介面 zh-TW 完成 |
| YesAlready | 0.0.0.1 | 自動確認對話 | 已發布；完成主設定、各分頁、Bothers 說明與提示 zh-TW 翻譯 |
| Price Insight | 2.11.3.1 | 顯示市場價格 | 已發布、繁中介面 |
| Gearsetter | 4.0.0.1 | 裝備升級建議 | 已發布；完成設定、裝備比較、屬性與提示 zh-TW 翻譯 |
| Ice's Cosmic Exploration | 0.0.73.43 | 宇宙探索採集、生產與任務輔助 | 已發布；修正台服研究威 NPC ID 不一致時無法主動互動與交貨；一般使用者介面 zh-TW 完成 |
| Better Occult Crescent & Chest Helper Interface | 1.0.1.1 | 蜃景新月島寶箱、兔子與遭遇輔助 | 已發布；由官方 1.0.1 API13 節點重新編譯；完整 zh-TW 介面 |
| Umbra XIV | 3.1.7.1 | 自訂工具列與世界標記 | 已發布；使用 API14 介面變更前的 API13 節點；完整 zh-TW 介面 |
| MissFisher | 1.6.5.13 | 釣魚輔助 | 已發布；回移上游 GatherBuddy Reborn 識別與啟用名稱修正；585 組內嵌介面資源為台灣繁中 |
| Skippy | 1.2.2.9 | 主線隨機任務過場跳過輔助 | 已發布；完成指令說明與聊天回饋 zh-TW 翻譯 |
| AutoHook | 5.0.0.14 | 釣魚與刺魚輔助 | 已發布；補齊 GatherBuddy 7.3.5 所需 IPC，含台服 API13 `DataId` 相容修補與完整繁中介面 |
| Avarice | 2.1.1.8 | 身位與距離提示 | 已發布；完成主要設定、設定檔、統計與視覺回饋 zh-TW 翻譯 |
| Orbwalker | 1.0.1.7 | 施法移動控制 | 已發布；完成主要設定、移動、顯示層、職業與按鍵 zh-TW 翻譯 |
| Palace Pal | 4.14.0.1 | 深層迷宮陷阱與寶藏提示 | 已發布；116/116 個介面資源鍵完整 zh-TW；需要 Splatoon |
| Pandora's Box | 1.6.3.19 | 多項便利功能合集 | 已發布；約 55 個功能名稱與說明、分類、搜尋及停用原因完成 zh-TW 翻譯 |
| Marketbuddy | 0.2.4.1 | 市場上架與調價輔助 | 已發布；完成主要介面 zh-TW 翻譯 |
| JobBars | 1.3.2.3 | 職業量譜、團隊增益與減傷追蹤 | 已發布；完成 zh-TW 主要與進階介面；台服 API13 安全節點 |
| NotificationMaster | 2.1.1.13 | 遊戲事件與背景通知 | 已發布；完成 zh-TW 主要與進階介面；台服 API13 安全節點 |
| CBT | 69.103.0.1 | Automaton 多功能自動化與便利調整 | 已發布；完成主設定、模組、追蹤器與通知 zh-TW 翻譯 |
| GatheringPathRenderer | 0.10.0.1 | 顯示採集節點路徑與位置 | 已發布；完成主要介面 zh-TW 翻譯；Questionable 開發工具 |
| Deliveroo | 7.4.0.1 | 軍隊籌備品自動繳納輔助 | 已發布；完成設定、繳納視窗、提示與聊天說明 zh-TW 翻譯 |
| Chilled Leves | 1.0.1.22 | 理符任務選擇、自動執行與繳交輔助 | 已發布；修正 vnavmesh IPC 尚未就緒時的視窗渲染錯誤；需要 vnavmesh |
| Explorer's Icebox | 1.0.4.6 | 無人島採集與升級輔助 | 已發布；完成主操作與除錯選單 zh-TW 翻譯；需要 vnavmesh 與 visland |
| Easier Faux Hollows | 0.0.0.11 | 幻巧拼圖已知圖樣求解器 | 已發布；完成 zh-TW 拼圖、設定與偵錯介面；原生 API13 安全節點 |
| Hyperborea | 1.0.0.33 | 區域探索與團體姿勢輔助 | 已發布；完成 zh-TW 主要與區域編輯介面；原生 API13 安全節點 |
| AutoMinion | 1.0.0.2 | 進入房屋時收起寵物，離開時重新召喚 | 已發布；完成 zh-TW 介面翻譯；由較早來源移植，風險較高 |
| XIV 藏寶圖工具小幫手 | 0.1.9.4 | 繁中藏寶圖組隊協作與網頁同步 | 已發布；座標訊息可自訂聊天頻道；解碼寶圖後可自動開啟地圖並設定旗標 |
| Visland | 0.0.0.138 | 無人島採集、工坊排程與活動自動化 | 已發布；完成採集路線、工房、穀倉、耕地、放牧地與出口交易 zh-TW 翻譯 |
| Chat 2 | 1.32.0.2 | 高度自訂的遊戲聊天視窗替代方案 | 已發布；補齊資料庫維護、搜尋、字體重設與內建 Web 聊天介面 zh-TW |
| Doorbell | 1.0.4.1 | 有人進出房屋時播放門鈴提示音 | 已發布；完成 zh-TW 介面翻譯 |
| MultiHit | 0.0.4.1 | 將傷害浮動文字依動畫拆分為多段 | 已發布；完成 zh-TW 介面翻譯 |
| Namingway | 1.1.17.1 | 自訂技能與狀態效果顯示名稱 | 已發布；完成 zh-TW 介面翻譯 |
| Mappy | 3.1.6.12 | 強化版遊戲地圖 | 已發布；完成 zh-TW 介面翻譯 |
| ChatCoordinates | 2.1.2.10 | 將聊天座標設為地圖旗標 | 已發布；完成 zh-TW 設定、說明與錯誤訊息翻譯 |
| FPS Plugin | 1.7.0.5 | 顯示遊戲 FPS | 已發布；完成 zh-TW 設定介面與狀態提示翻譯 |
| Craftimizer | 2.8.0.2 | 製作模擬、巨集產生與技能建議 | 已發布；完成設定、巨集、製作筆記與製作輔助 zh-TW 翻譯 |
| SortaKinda | 2.1.1.7 | 自訂物品欄排序 | 已發布；完成 zh-TW 介面翻譯 |
| QoL Bar | 2.3.3.7 | 自訂指令與插件快捷列 | 已發布；台服 7.3／API13 相容修正；完成 zh-TW 介面翻譯 |
| IINACT | 1.13.9.5 | ACT 相容戰鬥資料解析 | 已發布；補齊解析篩選名稱與主視窗初始化進度 |
| LMeter | 1.13.0.3 | 遊戲內 ACT 戰鬥統計介面 | 已發布；完成 zh-TW 介面翻譯；搭配 IINACT 使用 |
| Distance | 1.1.3.6 | 顯示目前目標距離 | 已發布；完成 zh-TW 主要與進階介面；官方 API13 節點 |
| EnemyListHP | 2.0.1.8 | 在敵對列表顯示 HP | 已發布；完成 zh-TW 介面；官方 7.3／API13 節點 |
| ReAction | 1.3.4.4 | 戰鬥操作便利調整 | 已發布；完成 zh-TW 主要與進階介面；涉及戰鬥 Hook，風險較高 |
| Radar Plugin | 2.1.8.3 | 顯示周圍敵人與互動物件 | 已發布；完成 zh-TW 主要與進階介面；具透視性質，風險高 |
| ReMakePlace Plugin | 7.3.4.0 | 房屋布置配置工具 | 已發布；完成 zh-TW 介面；修正台服 API13 建置相容性 |
| DozeAnywhere | 13.1.0.1 | 在更多地點坐下或睡覺 | 已發布；完成 zh-TW 介面；涉及姿勢限制修改，風險較高 |
| Cammy | 2.1.0.14 | 進階鏡頭與鏡位調整 | 已發布；完成 zh-TW 介面；涉及記憶體修改，風險較高 |
| Gauge-O-Matic | 0.8.2.3 | 自訂增益與職業量譜提示 | 已發布；完成 zh-TW 主要與進階介面；7.31／API13 節點 |
| EngageTimer | 2.4.4.1 | 顯示完整戰鬥倒數與戰鬥時間 | 已發布；完成 zh-TW 介面；官方 API13 節點 |
| BigPlayerDebuffs | 1.1.0.14 | 放大自己施加的狀態圖示 | 已發布；完成 zh-TW 介面；官方 API13 節點 |
| Better Mount Roulette | 1.0.0.2 | 可自訂規則的隨機坐騎 | 已發布；完成 zh-TW 介面；採用相容台服 API13 的安全節點 |
| Submarine Tracker | 2.0.2.2 | 追蹤部隊潛水艇航程、返航時間與收益 | 已發布；完成 463/463 個 zh-TW 資源鍵、指令與未資源化介面；已更新有漏洞的 MessagePack 依賴 |
| Party Icons | 1.2.3.3 | 依職業或團隊位置調整玩家名牌 | 已發布；完成 zh-TW 設定、名牌、團隊站位與升級指南介面 |
| RezPls | 1.5.2.3 | 標示正在復活、已有復活效果及可解除的負面狀態 | 已發布；完整 zh-TW 介面與指令說明；API13 安全日期範圍內最後節點 |
| FlyTextFilter | 4.4.0.3 | 過濾並調整戰鬥浮動文字 | 已發布；完成設定、類型表、匯入匯出、位置、黑名單與說明介面的 zh-TW 翻譯 |
| MapLinker | 1.1.11.2 | 記錄與搜尋聊天中的地圖連結 | 已發布；完整繁中介面；採用 2025-08-17 的正式 API13 節點 |
| Allagan Market | 1.2.0.8 | 整理僱員上架、銷售紀錄與市場壓價資訊 | 已發布；269 組 zh-TW 資源；CSV 欄位識別保持英文；台服 Universalis 資料可能不完整 |
| Allagan Tools | 1.13.1.13 | 跨角色追蹤、搜尋、篩選並整理庫存 | 已發布；648 個實際介面鍵零缺漏、1,465 筆有效 zh-TW 資源；修正目前角色的僱員掛賣未寫入庫存追蹤與物品提示 |
| Allagan Item Search | 1.0.0.4 | 依條件搜尋與篩選遊戲物品 | 已發布；236 個 zh-TW 資源鍵及 119/119 renderer 名稱 |
| Title Edit | 3.0.6.22 | 建立、分享並切換自訂標題與角色選擇畫面 | 已發布；完成進階預設編輯、群組、場景通知與偵錯視窗 zh-TW 翻譯；保留 API13 坐騎解鎖修正 |
| MonsterDex | 2.13.6.2 | 顯示深層迷宮魔物資料與攻略提示 | 已發布；完成設定、樓層、提示與深層迷宮術語的 zh-TW 翻譯 |
| High FPS Physics Fix | 8.3.0.1 | 改善高 FPS 下的動作物理表現 | 已發布；採用 2025-08-06 的 API13 安全節點，含繁中介面 |
| Orchestrion Plugin | 2.2.0.13 | 瀏覽、辨識及變更遊戲內背景音樂 | 已發布；115/115 個介面語系鍵完成 zh-TW 翻譯 |
| CrossUp | 1.7.1.14 | 自訂十字快捷欄外觀、位置與擴展操作 | 已發布；121/121 個介面語系鍵完成 zh-TW 翻譯 |
| TriadBuddy | 1.13.0.2 | 九宮幻卡對戰求解、牌組分析與收藏輔助 | 已發布；修復原中文亂碼並完成 64/64 個 zh-TW 語系鍵 |
| MeterWay | 1.0.17.2 | 搭配 IINACT 或 ACT 顯示即時戰鬥統計 | 已發布；完成 Lazer／Mogu／Vision、動態 Lua 與主要設定 zh-TW 翻譯 |
| Death Recap | 1.13.2.3 | 顯示死亡前的傷害、治療、增益、減益與護盾紀錄 | 已發布；完成設定、主視窗、篩選、提示與通知的 zh-TW 翻譯 |
| Teleporter | 2.0.2.10 | 以聊天指令依以太之光或區域名稱傳送，支援自訂別名 | 已發布；修正台服繁中語言的 Sanitizer 啟動錯誤 |
| DailyDuty | 5.3.2.14 | 追蹤每日與每週任務完成狀態 | 已發布；216/216 個資源鍵完成 zh-TW 翻譯 |
| ezMiniCactpot | 3.0.0.4 | 標示仙人微彩的最佳翻牌位置與選線 | 已發布；完成設定、提示與插件說明的 zh-TW 翻譯 |
| PingPlugin | 2.9.0.2 | 顯示目前遊戲伺服器的網路延遲 | 已發布；完整台灣繁中介面；保留台服專用 TCP handshake 量測 |
| Sonar | 0.7.4.4 | 自動傳送與接收狩獵及 FATE 通報 | 已發布；完成主要介面與音效名稱 zh-TW 翻譯；會連線社群服務，且歷史 API13 相依套件含已知安全性警告，風險較高 |

Questionable 的台服建置停用了程式內「放棄任務」原生命令；需要放棄任務時請使用遊戲任務日誌。此限制不影響任務路徑、對話、傳送或 vnavmesh 導航。

## 版本原則

- 以 2025 年 8 月 5 日至 2025 年 12 月 16 日的 API13 時期為主要查找範圍
- 必須由來源、manifest 或實際組件確認 `DalamudApiLevel = 13`
- 使用台服 API13 Dalamud 與相符的 FFXIVClientStructs 重新編譯
- 含原生 DLL、導航資料或私有依賴的插件必須額外驗證，不只確認 managed DLL
- API14 來源不能只把 manifest 數字改成 13
- 每個正式資產使用唯一檔名與 SHA-256，避免 GitHub/CDN 快取舊檔

詳細來源節點請見 [SOURCE_AUDIT.md](SOURCE_AUDIT.md)。

繁中介面翻譯範圍、禁止修改項目與逐插件進度請見 [LOCALIZATION_AUDIT.md](LOCALIZATION_AUDIT.md)。

## 風險說明

部分插件會自動執行戰鬥、移動、任務、生產或其他遊戲操作。此倉庫只處理 API13 與台服客戶端相容性，不代表這些功能符合遊戲服務條款；請自行評估使用風險。

## 參考

- [aliceric27/DalamudPlugins-TW](https://github.com/aliceric27/DalamudPlugins-TW)
- [台服 Dalamud](https://github.com/yanmucorp/Dalamud)
- [台服 FFXIVClientStructs TC-BASE](https://github.com/yanmucorp/FFXIVClientStructs/tree/TC-BASE)
