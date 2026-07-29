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
| Bossmod／Boss Mod | 0.1.4.1 | Boss 機制輔助 | 已發布；台服 7.3 安全物品同步，移除不穩定 Hook |
| Bossmod Reborn | 7.3.8.2 | 技能範圍與戰鬥輔助 | 已發布；台服 7.3 安全物品同步，移除不穩定 Hook |
| Rotation Solver Reborn | 7.3.5.0 | 技能循環 | 已發布；台服 7.3／API13 安全節點 |
| Splatoon | 3.8.2.1 | 場景繪製點、線、面 | 已發布（來源 tag 3.8.1.5 的實際組件版本） |
| Wrath Combo | 1.0.1.18 | 整合連段 | 已發布；使用真正相容台服 API13 的 2025-08-05 節點 |
| AntiAfkKick | 2.1.0.9 | 防止閒置斷線 | 已發布 |
| AutoRetainer | 4.5.1.22 | 雇員相關功能 | 已發布；含繁中公會工坊／組件用語修正 |
| Saucy | 1.4.2.8 | 金碟相關功能 | 已發布；含 API13 編譯修正 |
| NoClippy | 0.5.0.19 | 改善技能延遲 | 已發布 |
| NecroLens | 1.0.8.11 | 深層迷宮輔助 | 已發布；包含台服 API13 型別相容修補 |
| MidiBard 2 | 3.2.1.2 | 樂器演奏 | 已發布；API14 型別誤用前的安全節點 |
| GatherBuddy Reborn | 7.2.5.2 | 採集輔助 | 已發布；支援繁中語言資料與安全語言 fallback |
| Artisan | 4.0.4.9 | 生產輔助 | 已發布；修正缺少熱鍵列時的空參考錯誤 |
| Burning Down the House | 1.7.1.0 | 房屋裝修 | 已發布；安全範圍內 API13 上游版本 |
| Raphael.Dalamud | 0.0.5.0 | 生產求解器／依賴庫 | 已發布 |
| Something Need Doing | 0.0.0.0 | 巨集擴展 | 已發布 |
| TextAdvance | 3.2.4.7 | 對話自動處理 | 已發布 |
| Lifestream | 2.5.2.4 | 傳送輔助 | 已發布；修正繁中「移動到公會工坊」辨識 |
| vnavmesh | 1.1.2.1 | 尋路與移動工具 | 已發布；API14 切換前最後一個正式 tag |
| AutoDuty | 0.0.0.0 | 副本自動化框架 | 已發布 API13 |
| Pixel Perfect | 3.3.2.0 | 顯示角色碰撞圈 | 已發布 |
| LazyLoot | 5.3.2.4 | 戰利品擲骰輔助 | 已發布 |
| Questionable | 13.68.129.3 | 任務輔助 | 已發布；略過台服資料中的無效副本地區參照 |
| YesAlready | 0.0.0.0 | 自動確認對話 | 已發布 API13 |
| Price Insight | 2.11.3.0 | 顯示市場價格 | 已發布 |
| Gearsetter | 4.0 | 裝備升級建議 | 已發布；正式 API13 tag |
| Ice's Cosmic Exploration | 0.0.73.40 | 宇宙探索採集、生產與任務輔助 | 已發布；含台服 API13 物件識別與 ECommons 相容修補 |
| BOCCHI | 1.0.1.0 | 蜃景新月島寶箱、兔子與遭遇輔助 | 已發布；由官方 1.0.1 API13 節點重新編譯 |
| Umbra XIV | 3.1.7.0 | 自訂工具列與世界標記 | 已發布；使用 API14 介面變更前的 API13 節點 |
| MissFisher | 1.6.5.9 | 釣魚輔助 | 已發布；上游僅提供 API13 時期二進位套件，未聲稱重新編譯 |
| Skippy | 1.2.2.8 | 主線隨機任務過場跳過輔助 | 已發布；SkipCutscene 的後繼插件 |
| AutoHook | 5.0.0.12 | 釣魚與刺魚輔助 | 已發布；含台服 API13 `DataId` 相容修補 |
| Avarice | 2.1.1.7 | 身位與距離提示 | 已發布；含台服 API13 編譯修補 |
| Orbwalker | 1.0.1.6 | 施法移動控制 | 已發布 API13 |
| Palace Pal | 4.14.0.0 | 深層迷宮陷阱與寶藏提示 | 已發布 API13；需要 Splatoon |
| Pandora's Box | 1.6.3.18 | 多項便利功能合集 | 已發布；使用 API14 屬性切換前的 API13 節點 |
| Marketbuddy | 0.2.4.0 | 市場上架與調價輔助 | 已發布 API13 |

Bossmod 與 Boss Mod 是同一個 `awgil/ffxiv_bossmod` 來源，在正式 manifest 中只會保留一筆，避免 Dalamud 顯示重複插件。

Questionable 的台服建置停用了程式內「放棄任務」原生命令；需要放棄任務時請使用遊戲任務日誌。此限制不影響任務路徑、對話、傳送或 vnavmesh 導航。

Puni.sh 官方核心倉庫目前列出的 14 個插件，在本倉庫中均已有對應 API13 版本。這項覆蓋只指 Puni.sh 官方核心清單，不包含目錄中其他作者自行維護的第三方倉庫。

## 版本原則

- 以 2025 年 8 月 5 日至 2025 年 12 月 16 日的 API13 時期為主要查找範圍
- 必須由來源、manifest 或實際組件確認 `DalamudApiLevel = 13`
- 使用台服 API13 Dalamud 與相符的 FFXIVClientStructs 重新編譯
- 含原生 DLL、導航資料或私有依賴的插件必須額外驗證，不只確認 managed DLL
- API14 來源不能只把 manifest 數字改成 13
- 每個正式資產使用唯一檔名與 SHA-256，避免 GitHub/CDN 快取舊檔

詳細來源節點請見 [SOURCE_AUDIT.md](SOURCE_AUDIT.md)。

## 風險說明

部分插件會自動執行戰鬥、移動、任務、生產或其他遊戲操作。此倉庫只處理 API13 與台服客戶端相容性，不代表這些功能符合遊戲服務條款；請自行評估使用風險。

## 參考

- [aliceric27/DalamudPlugins-TW](https://github.com/aliceric27/DalamudPlugins-TW)
- [台服 Dalamud](https://github.com/yanmucorp/Dalamud)
- [台服 FFXIVClientStructs TC-BASE](https://github.com/yanmucorp/FFXIVClientStructs/tree/TC-BASE)
