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
| Boss Mod | 0.1.4.1 | Boss 機制輔助 | 已發布；台服 7.3 安全物品同步，移除不穩定 Hook |
| Bossmod Reborn | 7.3.8.2 | 技能範圍與戰鬥輔助 | 已發布；台服 7.3 安全物品同步，移除不穩定 Hook |
| Rotation Solver Reborn | 7.3.5.0 | 技能循環 | 已發布；台服 7.3／API13 安全節點 |
| Splatoon | 3.8.2.2 | 場景繪製點、線、面 | 已發布；301 個中文介面值轉為台灣繁中 |
| Wrath Combo | 1.0.1.18 | 整合連段 | 已發布；使用真正相容台服 API13 的 2025-08-05 節點 |
| AntiAfkKick | 2.1.0.10 | 防止閒置斷線 | 已發布；繁中插件說明，插件本身無設定介面 |
| AutoRetainer | 4.5.1.22 | 雇員相關功能 | 已發布；含繁中公會工坊／組件用語修正 |
| Saucy | 1.4.2.9 | 金碟相關功能 | 已發布；完成 zh-TW 主介面與九宮幻卡資源翻譯 |
| NoClippy | 0.5.0.20 | 改善技能延遲 | 已發布；完成 zh-TW 介面翻譯 |
| NecroLens | 1.0.8.11 | 深層迷宮輔助 | 已發布；包含台服 API13 型別相容修補 |
| MidiBard 2 | 3.2.1.3 | 樂器演奏 | 已發布；API14 型別誤用前的安全節點；補齊 zh-TW 介面資源 |
| GatherBuddy Reborn | 7.3.5.1 | 採集輔助 | 已發布；AtmoOmen 7.3.5 節點、繁中語言資料與 AutoHook IPC 載入順序容錯 |
| Artisan | 4.0.4.9 | 生產輔助 | 已發布；修正缺少熱鍵列時的空參考錯誤 |
| Burning Down the House | 1.7.1.0 | 房屋裝修 | 已發布；安全範圍內 API13 上游版本 |
| Raphael.Dalamud | 0.0.5.0 | 生產求解器／依賴庫 | 已發布 |
| Something Need Doing | 0.0.0.0 | 巨集擴展 | 已發布 |
| TextAdvance | 3.2.4.8 | 對話自動處理 | 已發布、繁中介面 |
| Lifestream | 2.5.2.4 | 傳送輔助 | 已發布；修正繁中「移動到公會工坊」辨識 |
| vnavmesh | 1.1.2.1 | 尋路與移動工具 | 已發布；API14 切換前最後一個正式 tag |
| AutoDuty | 0.0.0.0 | 副本自動化框架 | 已發布 API13 |
| Pixel Perfect | 3.3.2.1 | 顯示角色碰撞圈 | 已發布；完成 zh-TW 介面翻譯 |
| LazyLoot | 5.3.2.5 | 戰利品擲骰輔助 | 已發布；完成 zh-TW 介面、指令說明與診斷訊息翻譯 |
| Questionable | 13.68.129.3 | 任務輔助 | 已發布；略過台服資料中的無效副本地區參照 |
| YesAlready | 0.0.0.0 | 自動確認對話 | 已發布 API13 |
| Price Insight | 2.11.3.1 | 顯示市場價格 | 已發布、繁中介面 |
| Gearsetter | 4.0 | 裝備升級建議 | 已發布；正式 API13 tag |
| Ice's Cosmic Exploration | 0.0.73.40 | 宇宙探索採集、生產與任務輔助 | 已發布；含台服 API13 物件識別與 ECommons 相容修補 |
| Better Occult Crescent & Chest Helper Interface | 1.0.1.1 | 蜃景新月島寶箱、兔子與遭遇輔助 | 已發布；由官方 1.0.1 API13 節點重新編譯；完整 zh-TW 介面 |
| Umbra XIV | 3.1.7.1 | 自訂工具列與世界標記 | 已發布；使用 API14 介面變更前的 API13 節點；完整 zh-TW 介面 |
| MissFisher | 1.6.5.12 | 釣魚輔助 | 已發布；完整移除上游建置保護器的啟動與每日到期檢查；內嵌台灣繁中介面 |
| Skippy | 1.2.2.8 | 主線隨機任務過場跳過輔助 | 已發布；SkipCutscene 的後繼插件 |
| AutoHook | 5.0.0.14 | 釣魚與刺魚輔助 | 已發布；補齊 GatherBuddy 7.3.5 所需 IPC，含台服 API13 `DataId` 相容修補與完整繁中介面 |
| Avarice | 2.1.1.7 | 身位與距離提示 | 已發布；含台服 API13 編譯修補 |
| Orbwalker | 1.0.1.6 | 施法移動控制 | 已發布 API13 |
| Palace Pal | 4.14.0.0 | 深層迷宮陷阱與寶藏提示 | 已發布 API13；需要 Splatoon |
| Pandora's Box | 1.6.3.18 | 多項便利功能合集 | 已發布；使用 API14 屬性切換前的 API13 節點 |
| Marketbuddy | 0.2.4.0 | 市場上架與調價輔助 | 已發布 API13 |
| JobBars | 1.3.2.1 | 職業量譜、團隊增益與減傷追蹤 | 已發布；台服 7.3／API13 安全節點 |
| NotificationMaster | 2.1.1.11 | 遊戲事件與背景通知 | 已發布；台服 7.3／API13 安全節點 |
| CBT | 69.103.0.0 | Automaton 多功能自動化與便利調整 | 已發布；v69.103 台服 API13 相容修正版 |
| GatheringPathRenderer | 0.10 | 顯示採集節點路徑與位置 | 已發布；Questionable 開發工具，台服 API13 相容修正版 |
| Deliveroo | 7.4 | 軍隊籌備品自動繳納輔助 | 已發布；官方 API13 節點 |
| Chilled Leves | 1.0.1.18 | 理符任務選擇、自動執行與繳交輔助 | 已發布；需要 vnavmesh |
| Explorer's Icebox | 1.0.4.5 | 無人島採集與升級輔助 | 已發布；需要 vnavmesh 與 visland |
| Easier Faux Hollows | 0.0.0.10 | 幻巧拼圖已知圖樣求解器 | 已發布；原生 API13 安全節點 |
| Hyperborea | 1.0.0.31 | 區域探索與團體姿勢輔助 | 已發布；原生 API13 安全節點 |
| AutoMinion | 1.0.0.2 | 進入房屋時收起寵物，離開時重新召喚 | 已發布；完成 zh-TW 介面翻譯；由較早來源移植，風險較高 |
| XIV 藏寶圖工具小幫手 | 0.1.9.1 | 繁中藏寶圖組隊協作與網頁同步 | 已發布；自有專案由 API12 實際移植至 API13 |
| Visland | 0.0.0.137 | 無人島採集、工坊排程與活動自動化 | 已發布；原生 API13 安全節點並完成 `BaseId` 相容修正 |
| Chat 2 | 1.32.0.1 | 高度自訂的遊戲聊天視窗替代方案 | 已發布；完成 zh-TW 介面第一輪校訂，並更新已知有漏洞的 MessagePack／SQLite 依賴 |
| Doorbell | 1.0.4.1 | 有人進出房屋時播放門鈴提示音 | 已發布；完成 zh-TW 介面翻譯 |
| MultiHit | 0.0.4.1 | 將傷害浮動文字依動畫拆分為多段 | 已發布；完成 zh-TW 介面翻譯 |
| Namingway | 1.1.17.1 | 自訂技能與狀態效果顯示名稱 | 已發布；完成 zh-TW 介面翻譯 |
| Mappy | 3.1.6.11 | 強化版遊戲地圖 | 已發布；台服 7.3／API13 安全節點 |
| ChatCoordinates | 2.1.2.10 | 將聊天座標設為地圖旗標 | 已發布；完成 zh-TW 設定、說明與錯誤訊息翻譯 |
| FPS Plugin | 1.7.0.5 | 顯示遊戲 FPS | 已發布；完成 zh-TW 設定介面與狀態提示翻譯 |
| Craftimizer | 2.8.0.1 | 製作模擬、巨集產生與技能建議 | 已發布；台服 7.3／API13 安全節點 |
| SortaKinda | 2.1.1.7 | 自訂物品欄排序 | 已發布；完成 zh-TW 介面翻譯 |

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
