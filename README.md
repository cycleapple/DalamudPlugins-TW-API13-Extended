# DalamudPlugins-TW-API13-Extended

台服 FFXIV 使用的 Dalamud API13 擴充插件倉庫。本倉庫與外觀插件用的
[DalamudPlugins-TW](https://github.com/cycleapple/DalamudPlugins-TW) 分開維護。

目前正在逐項稽核與重新編譯，尚未驗證的插件不會加入 `repo.json`。參考倉庫提供的是 API12 二進位檔，因此不會直接複製或只修改 manifest 冒充 API13。

## 安裝網址

在 Dalamud 的「自訂插件儲存庫」加入：

```text
https://raw.githubusercontent.com/cycleapple/DalamudPlugins-TW-API13-Extended/main/repo.json
```

`repo.json` 只會列出已完成 API13 編譯驗證的插件，其餘項目會分批加入。

## 收錄範圍

| 插件 | 目標版本 | 用途 | 狀態 |
|---|---:|---|---|
| Bossmod／Boss Mod | 0.1.4.0 | Boss 機制輔助 | 已發布；台服 7.3／API13 相容修補 |
| Bossmod Reborn | 7.3.8.1 | 技能範圍與戰鬥輔助 | 已發布；最後一個未使用 API14 型別的正式 tag |
| Rotation Solver Reborn | 7.3.5.0 | 技能循環 | 已發布；台服 7.3／API13 安全節點 |
| Splatoon | 3.8.2.1 | 場景繪製點、線、面 | 已發布（來源 tag 3.8.1.5 的實際組件版本） |
| Wrath Combo | 1.0.1.18 | 整合連段 | 已發布；使用真正相容台服 API13 的 2025-08-05 節點 |
| AntiAfkKick | 2.1.0.9 | 防止閒置斷線 | 已發布 |
| AutoRetainer | 4.5.1.21 | 雇員相關功能 | 已發布（首批可驗證 API13 tag） |
| Saucy | 1.4.2.8 | 金碟相關功能 | 已發布；含 API13 編譯修正 |
| NoClippy | 0.5.0.19 | 改善技能延遲 | 已發布 |
| NecroLens | 1.0.8.11 | 深層迷宮輔助 | 已發布；包含台服 API13 型別相容修補 |
| MidiBard 2 | 3.1.0.0 | 樂器演奏 | 閉源／需確認 API13 發布包 |
| GatherBuddy Reborn | 7.2.5.1 | 採集輔助 | 已發布；含台服 API13 型別修補與 MessagePack 安全更新 |
| Artisan | 4.0.4.8 | 生產輔助 | 已發布；含台服 API13 型別相容修補 |
| Burning Down the House | 1.7.1.0 | 房屋裝修 | 已發布；安全範圍內 API13 上游版本 |
| Raphael.Dalamud | 0.0.5.0 | 生產求解器／依賴庫 | 已發布 |
| Something Need Doing | 0.0.0.0 | 巨集擴展 | 已發布 |
| TextAdvance | 3.2.4.7 | 對話自動處理 | 已發布 |
| Lifestream | 2.5.2.3 | 傳送輔助 | 已發布（2.5.1.15 為 API12） |
| vnavmesh | 1.1.2.1 | 尋路與移動工具 | 已發布；API14 切換前最後一個正式 tag |
| AutoDuty | 0.0.0.0 | 副本自動化框架 | 已發布 API13 |
| Pixel Perfect | 3.3.2.0 | 顯示角色碰撞圈 | 已發布 |
| LazyLoot | 5.3.2.4 | 戰利品擲骰輔助 | 已發布 |
| Questionable | 5.23 | 任務輔助 | 非 GitHub 上游，稽核中 |
| YesAlready | 0.0.0.0 | 自動確認對話 | 已發布 API13 |
| Price Insight | 2.11.3.0 | 顯示市場價格 | 已發布 |
| Gearsetter | 3.1 | 裝備升級建議 | 非 GitHub 上游，稽核中 |

Bossmod 與 Boss Mod 是同一個 `awgil/ffxiv_bossmod` 來源，在正式 manifest 中只會保留一筆，避免 Dalamud 顯示重複插件。

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
