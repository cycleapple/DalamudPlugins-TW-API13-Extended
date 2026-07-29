# API13 Source Audit

稽核截止點為 2025-12-16 23:59:59 UTC。`已確認 API13` 只代表來源 manifest 已確認，仍需使用台服 API13 環境完成編譯與執行驗證。

| 插件 | 上游 | 截止 commit | 日期（UTC） | 初步結果 |
|---|---|---|---|---|
| Bossmod／Boss Mod | `awgil/ffxiv_bossmod` | `381151125` | 2025-11-29 | API13 編譯成功；`cycleapple/ffxiv_bossmod@1460e54d9` 修正台服型別與 C# 建置相容性，發布 0.1.4.0。後續開始使用 API14 `IPlayerState` |
| Bossmod Reborn | `FFXIV-CombatReborn/BossmodReborn` | `9222b6062` / tag `7.3.8.1` | 2025-11-24 | API13 編譯成功；`cycleapple/BossmodReborn@6338acdaa` 改用台服 ClientStructs 組件並修正 Dalamud 型別，發布 7.3.8.1。7.3.8.2 起已使用 API14 型別 |
| Rotation Solver Reborn | `FFXIV-CombatReborn/RotationSolverReborn` | `4907d030` / tag `7.3.5.0` | 2025-10-07 | API13 編譯成功；`cycleapple/RotationSolverReborn@8b9fb1d7` 鎖定 net9 相容 Lumina.Excel，發布 7.3.5.0。較晚的 7.3.8.x 雖標 API13，已使用 API14 型別 |
| Splatoon | `PunishXIV/Splatoon` | `ae37f2b` / tag `3.8.1.5` | 2025-08-28 | `cycleapple/Splatoon@f0c759f` 保留 301 個查詢鍵並將顯示值轉為台灣繁中；API13 編譯成功，發布 3.8.2.2 |
| Wrath Combo | `MeowZWR/WrathCombo` | `3b968ca32` | 2025-08-05 | API13 編譯成功；`cycleapple/WrathCombo@59b67130e` 發布 1.0.1.18。12 月節點雖仍標 API13，但已使用新版 Dalamud 型別，不相容台服 API13 |
| AntiAfkKick | `NightmareXIV/AntiAfkKick` | `7a0ebaa8` | 2025-08-07 | `cycleapple/AntiAfkKick@8689ea7` 僅翻譯插件安裝頁說明；插件本身無設定介面；API13 編譯 0 警告、0 錯誤，發布 2.1.0.10 |
| AutoRetainer | `PunishXIV/AutoRetainer` | `1e4e6b6` / tag `4.5.1.12` | 2025-08-15 | API13 編譯成功；`cycleapple/AutoRetainer@9ec26a1` 修正繁中公會工坊／組件用語，發布 4.5.1.22 |
| Saucy | `PunishXIV/Saucy` | `8e8d5949` | 2025-08-15 | 台服修正 `cycleapple/Saucy@a79b1c5`；`cycleapple/Saucy@5c751d1` 翻譯主介面與九宮幻卡 zh 資源，並修正語言檔未嵌入 DLL 的問題；API13 編譯成功（8 個上游警告、0 錯誤），發布 1.4.2.9 |
| NoClippy | `UnknownX7/NoClippy` | `d32ae7af` | 2025-08-09 | `cycleapple/NoClippy@934ab0f` 僅翻譯設定、技能後搖、戰鬥統計、記錄選項、狀態預測警告與指令回覆；API13 編譯 0 警告、0 錯誤，發布 0.5.0.20 |
| NecroLens | `Jukkales/NecroLens` | `d6646478` | 2025-11-26 | API13 編譯成功；`cycleapple/NecroLens@98cd7c2` 修正 `BaseId` 相容性並發布 1.0.8.11 |
| GatherBuddy Reborn | `AtmoOmen/GatherBuddyReborn` | `a34733dc` / tag `7.3.5.0` | 2025-12-02 | 位於安全日期範圍且 manifest 為 API13；`cycleapple/GatherBuddyReborn@9841d23` 加入台服繁中資料 fallback、`DataId` 相容修補及 AutoHook IPC 載入順序容錯，發布 7.3.5.1 |
| Artisan | `MeowZWR/Artisan` | `e4a0ddaf` | 2025-12-13 | API13 編譯成功；`cycleapple/Artisan@4c90707` 修正 `BaseId` 相容性，發布實際組件版本 4.0.4.8；上游已封存 |
| Burning Down the House | `LeonBlade/BDTHPlugin` | `ba39d13c` | 2025-09-30 | API13 編譯成功；發布 1.7.1.0 |
| Raphael.Dalamud | `Dalamud-DailyRoutines/Raphael.Dalamud` | `de11e646` | 2025-09-16 | API13 編譯成功；發布 0.0.5.0 |
| Something Need Doing | `Jaksuhn/SomethingNeedDoing` | `11422e55` | 2025-11-28 | API13 編譯成功；發布 0.0.0.0 |
| TextAdvance | `cycleapple/TextAdvance` (`api13-tw`) | `f8a7cf5` | 2025-11-22 基底 | API13 編譯成功；繁中介面發布 3.2.4.8 |
| Lifestream | `NightmareXIV/Lifestream` | `305dfbf9` / tag `2.5.2.3` | 2025-08-07 | API13 編譯成功；`cycleapple/Lifestream@e6f5ec0` 修正繁中「移動到公會工坊」選單辨識，發布 2.5.2.4 |
| vnavmesh | `awgil/ffxiv_navmesh` | `5f512e5` / tag `v1.1.2.1` | 2025-12-15 | API13 編譯成功；`cycleapple/ffxiv_navmesh@8d90451` 發布 1.1.2.1。上游於 12 月 17 日才切換 API14 |
| AutoDuty | `ffxivcode/AutoDuty` | `a7d1eca8` | 2025-12-08 | API13 編譯成功；實際組件版本 0.0.0.0 |
| Pixel Perfect | `Haplo064/PixelPerfect` | `b371fe07` | 2025-08-07 | `cycleapple/PixelPerfect@80adfa2` 僅翻譯歡迎頁、設定、圖形參數、匯入／匯出通知、編輯器與說明；API13 編譯成功（4 個上游 nullable 警告、0 錯誤），發布 3.3.2.1 |
| LazyLoot | `PunishXIV/LazyLoot` | `d685ef0c` | 2025-11-19 | `cycleapple/LazyLoot@994d7ad` 完成設定介面、指令說明、狀態列、擲骰結果與診斷訊息繁中化；保留指令參數、設定格式與擲骰邏輯；台服 API13 編譯成功（2 個既有警告、0 錯誤），發布 5.3.2.5 |
| YesAlready | `PunishXIV/YesAlready` | `ca2288dd` | 2025-11-10 | API13 編譯成功；上游 manifest 版本為 0.0.0.0 |
| Price Insight | `cycleapple/ffxiv-priceinsight` (`api13-tw`) | `b90564e` | 2025-08-07 基底 | API13 編譯成功；繁中介面發布 2.11.3.1 |
| MidiBard 2 | `reckhou/MidiBard2` | `1665029` | 2025-11-30 | API13 編譯成功；`cycleapple/MidiBard2@d141b5d` 修正 SDK 與台服組件路徑並補齊 zh-TW 介面資源，發布 3.2.1.3。下一提交開始誤用 API14 `IPlayerState` |
| Questionable | `PunishXIV/Questionable` | `34735346f` / tag `v13.68.129.2` | 2025-12-15 | API13 編譯成功；`cycleapple/Questionable@f71531737` 適配台服 TC-BASE。程式內放棄任務因缺少安全原生介面而停用，其餘核心功能保留 |
| Gearsetter | `VeraNala/Gearsetter` | `21a2b8c` / tag `v4.0` | 2025-08-10 | API13 編譯成功；`cycleapple/Gearsetter@api13-tw` 發布 4.0，使用原始鎖定的 `qstxiv/LLib@f1716ee` |
| Ice's Cosmic Exploration | `LeontopodiumNivale14/Ices-Cosmic-Exploration` | `f3b7a696c9` | 2025-12-15 | `cycleapple/Ices-Cosmic-Exploration@9ced6b4` 將 ECommons 鎖回台服 API13 相容節點、以 `DataId` 取代後期 `BaseId` 並改用 `Player.JobId`，發布 0.0.73.40 |
| BOCCHI | `OhKannaDuh/BOCCHI` | `01d22a8565` / release `1.0.1` | 2025-12-07 | 原始碼與 manifest 均為 API13；`cycleapple/BOCCHI@4ccbbd1` 更新 legacy NuGet 鎖定資料、修正實際組件版本，並將 22 份中文語系資源轉為台灣繁中，發布 1.0.1.1 |
| Umbra XIV | `una-xiv/umbra` | `2d165ce` | 2025-10-08 | `Dalamud.NET.Sdk/13.0.0`；`cycleapple/umbra@ba18260` 將 1568 個既有中文介面鍵轉為台灣繁中並以台服 API13 編譯，發布 3.1.7.1。後期提交開始使用台服 API13 不存在的 `BaseId` 與 `IObjectTable.LocalPlayer` |
| MissFisher | `BlackCleaverLoli/MissFisher` | `93487c5` | 2025-12-13 | 上游只發布 1.6.5.9 二進位套件、未公開原始碼；該 DLL 被未註冊版 .NET Reactor 注入 14 天到期例外及完整授權重驗流程。`cycleapple/MissFisher@4545b74` 提供可重現的 Mono.Cecil 最小修補器，1.6.5.12 同時停用單一日期檢查與共用授權評估入口，並將內嵌 `lang.json` 的 556 個中文顯示值轉為台灣繁中；其他插件 IL 保留 |
| Skippy | `BoxuChan/Skippy` | `61c7c4f` | 2025-08-12 | 上游 manifest 與 Packager 均為 API13；`cycleapple/Skippy@e0a99f3` 修正組件版本與 repo 版本不一致，台服 API13 編譯成功，發布 1.2.2.8 |
| AutoHook | `PunishXIV/AutoHook` | `081cab55` / tag `v5.0.0.23` | 2025-12-03 | 位於安全日期範圍且 manifest 為 API13；包含 GatherBuddy 7.3.5 所需的 `GetPluginState`、`GetAutoStartFishing` 與 `SetAutoStartFishing` IPC；`cycleapple/AutoHook@16103ca` 套用台服 `DataId` 相容修補及完整 zh-TW 介面，發布 5.0.0.14 |
| Avarice | `PunishXIV/Avarice` | `0c831ce` | 2025-09-02 | `cycleapple/Avarice@c7fd996` 使用 API13 相依節點並移除未使用的 Windows Forms using，台服 API13 0 警告、0 錯誤，發布 2.1.1.7 |
| Orbwalker | `PunishXIV/Orbwalker` | `caf40f9` | 2025-09-13 | SDK 與 manifest 均為 API13；台服 API13 編譯成功，發布 1.0.1.6 |
| Palace Pal | `PunishXIV/PalacePal` | `bac8abe` | 2025-10-09 | SDK 13.1、manifest API13；台服 API13 編譯成功，發布 4.14.0.0 |
| Pandora's Box | `PunishXIV/PandorasBox` | `01f457f` | 2025-10-12 | API13 編譯成功，發布 1.6.3.18；10 月 31 日後的提交開始改用台服 API13 不存在的 `IPartyMember.EntityId` 與 `BaseId` |
| Marketbuddy | `PunishXIV/Marketbuddy` | `cf9d24d` | 2025-08-07 | DalamudPackager 13.0.0 並直接連結台服 API13 DLL 編譯成功，發布 0.2.4.0 |
| JobBars | `0ceal0t/JobBars` | `48cbbce` | 2025-08-16 | SDK 與 manifest 均為 API13；`cycleapple/JobBars@api13-tw` 使用原始鎖定的 KamiToolKit 節點，以台服 API13 編譯成功並發布 1.3.2.1 |
| NotificationMaster | `NightmareXIV/NotificationMaster` | `8674bc5` | 2025-11-05 | manifest 與 DalamudPackager 為 API13、ECommons 鎖定 `3.0.0.18-api13`；`cycleapple/NotificationMaster@api13-tw` 使用原始 NotificationMasterAPI 子模組，以台服 API13 編譯成功並發布 2.1.1.11 |
| CBT（Automaton） | `Jaksuhn/ffxiv-bundleoftweaks` | `80d0545` / tag `v69.103` | 2025-11-16 | 11 月 16 日稍後開始引用台服 API13 不存在的 `TerritoryIntendedUse`，11 月底又改用較新 `AgentReturn`；`cycleapple/ffxiv-bundleoftweaks@c6baead` 將 `BaseId`／`IPartyMember.EntityId` 對應回 API13 介面，以台服 DLL 編譯成功並發布 69.103.0.0 |
| GatheringPathRenderer | `PunishXIV/Questionable` | `34735346f` / tag `v13.68.129.2` | 2025-12-15 | 與 Questionable 使用同一 API13 安全基線；`cycleapple/Questionable@b4303ebb8` 將獨立採集路徑工具的 `IGameObject.BaseId` 對應回台服 API13 `DataId`，編譯 0 警告、0 錯誤並發布 0.10 |
| Deliveroo | `VeraNala/Deliveroo` | `76abfc8` / tag `v7.4` | 2025-08-07 | 上游明確標記「7.4 API13」；鎖定 `qstxiv/LLib@f1716ee`，`cycleapple/Deliveroo@926d453` 以台服 API13 DLL 編譯成功（僅 1 個上游複雜度警告）並發布 7.4 |
| Chilled Leves | `LeontopodiumNivale14/ChilledLeves` | `28d3025` | 2025-10-22 | SDK 13，鎖定上游 ECommons 子模組；`cycleapple/ChilledLeves@a7c46bc` 以台服 API13 DLL 編譯成功（8 個上游警告、0 錯誤）並發布 1.0.1.18 |
| Explorer's Icebox | `LeontopodiumNivale14/Explorers-Icebox` | `816a5ba` | 2025-11-19 | SDK 13，鎖定 ECommons 與 Pictomancy 子模組；`cycleapple/Explorers-Icebox@37840d1` 以 .NET 10 編譯器和台服 API13 DLL 編譯成功（7 個主專案上游警告、0 錯誤）並發布 1.0.4.5 |
| Easier Faux Hollows | `awgil/vfaux` | `77b8b67d` / tag `v0.0.0.10` | 2025-10-31 | 原生 SDK / API13 安全節點；`cycleapple/vfaux@0f85fd5` 補正套件版本並以台服 API13 依賴編譯，0 警告、0 錯誤；發布 0.0.0.10 |
| Hyperborea | `kawaii/Hyperborea` | `21f6fa50` | 2025-11-12 | 原生 manifest API13 安全節點；`cycleapple/Hyperborea@api13-tw` 以台服 API13 依賴編譯，13 個上游警告、0 錯誤；發布 1.0.0.31 |
| AutoMinion | `Asuna/AutoMinion` | `07fb9427` | 2025-03-27 | 上游在指定日期範圍內沒有節點；`cycleapple/AutoMinion@c22463b` 將 SDK、Packager、ImGui binding 與 ECommons 實際移植至 API13；`cycleapple/AutoMinion@e1e208b` 僅翻譯設定、搜尋、按鈕、指令說明與 manifest；16 個上游警告、0 錯誤；較高風險，發布 1.0.0.2 |
| XIV 藏寶圖工具小幫手 | `cycleapple/xiv-party-treasure-helper` | `aaa94f7` | 2026-04-27 | 自有 API12 專案；`cycleapple/xiv-party-treasure-helper@a99571a` 將 SDK、Packager、ImGui binding 與台服依賴實際移植至 API13，0 警告、0 錯誤；發布 0.1.9.1 |
| Visland | `awgil/ffxiv_visland` | `f7f40e1` / tag `v0.0.0.137` | 2025-08-09 | 上游 API13 安全節點；`cycleapple/ffxiv_visland@46ed315` 補正版本與 manifest、將 `DataId` 更新為 API13 `BaseId`，並鎖定 `cycleapple/AutoRetainerAPI@c3689ae`；台服 API13 編譯 0 警告、0 錯誤，發布 0.0.0.137 |
| Chat 2 | `Infiziert90/ChatTwo` | `956e57a` | 2025-11-17 | 上游 API13 安全節點；`cycleapple/ChatTwo@b1861f3` 更新有漏洞的依賴，`cycleapple/ChatTwo@a341033` 僅修改 zh-Hant 資源與語言顯示名稱；主插件以台服 API13 編譯成功（15 個上游警告、0 錯誤），發布 1.32.0.1 |
| Doorbell | `Aida-Enna/Doorbell` | `0a01851` | 2025-08-09 | 上游明確更新 7.3 並使用 SDK 13；`cycleapple/Doorbell@9b59581` 僅翻譯設定視窗、指令說明、狀態訊息與預設通知文字；台服 API13 編譯 0 警告、0 錯誤，發布 1.0.4.1 |
| MultiHit | `Bluefissure/MultiHit` | `72d95e8f65` | 2025-08-18 | 上游原生 `Dalamud.NET.Sdk/13.0.0` 節點；`cycleapple/MultiHit@1357aab` 僅翻譯顯示文字、說明與通知，以台服 API13 編譯成功（340 個上游平台／nullable 警告、0 錯誤），發布 0.0.4.1 |
| Namingway | `reiichi001/NamingWay` | `f7987e3257` | 2025-03-29 | 指定日期範圍內沒有 API13 節點；`cycleapple/NamingWay@079d4c7` 將 SDK、ImGui binding、list clipper 與 texture handle 實際移植至 API13；`cycleapple/NamingWay@968bfb9` 僅翻譯介面與預設套組顯示名稱；1 個上游 nullable 警告、0 錯誤，發布 1.1.17.1 |
