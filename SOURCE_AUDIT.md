# API13 Source Audit

稽核截止點為 2025-12-16 23:59:59 UTC。`已確認 API13` 只代表來源 manifest 已確認，仍需使用台服 API13 環境完成編譯與執行驗證。

| 插件 | 上游 | 截止 commit | 日期（UTC） | 初步結果 |
|---|---|---|---|---|
| Bossmod／Boss Mod | `awgil/ffxiv_bossmod` | `381151125` | 2025-11-29 | API13 編譯成功；`cycleapple/ffxiv_bossmod@2d2c09056de23d599e3e2811088186c2692e6204` 保留台服 7.3 相容修正並完成一般使用者介面 zh-TW；0 警告、0 錯誤，發布 0.1.4.3。後續開始使用 API14 `IPlayerState` |
| Bossmod Reborn | `FFXIV-CombatReborn/BossmodReborn` | `9222b6062` / tag `7.3.8.1` | 2025-11-24 | API13 編譯成功；`cycleapple/BossmodReborn@b838d4ccc` 保留台服 ClientStructs、Dalamud 型別修正與完整 zh-TW，回移朱雀幻巧戰、UWU 提示、隊伍同步及 M07N 空值防護，並修正 API13 隊伍角色分配與重複玩家欄位；API13 Release 建置 0 警告、0 錯誤，發布 7.3.8.8。後續主線已使用 API14 型別 |
| Rotation Solver Reborn | `FFXIV-CombatReborn/RotationSolverReborn` | `4907d030` / tag `7.3.5.0` | 2025-10-07 | `cycleapple/RotationSolverReborn@939b5182c6aea1df9076e89edeb030e399b638dc` 保留 net9 相容 Lumina.Excel 並完成一般使用者介面 zh-TW；API13 建置 0 錯誤、1 個既有 XML 註解警告，發布 7.3.5.3。較晚的 7.3.8.x 雖標 API13，已使用 API14 型別 |
| Splatoon | `PunishXIV/Splatoon` | `ae37f2b` / tag `3.8.1.5` | 2025-08-28 | `cycleapple/Splatoon@d1873a6` 保留 301 個查詢鍵、台服 7.3 MapEffect 修正與功能邏輯，完成一般使用者介面 zh-TW；API13 建置 0 錯誤、3 個既有參考警告，發布 3.8.2.5 |
| Wrath Combo | `MeowZWR/WrathCombo` | `3b968ca32` | 2025-08-05 | 保留 API13 戰鬥邏輯，參考 `1.0.1.20-cn` 與 `1.0.4.19-cn` 的在地化資源補齊功能清單及職業設定 zh-TW；將未翻譯的 combo metadata 與繁中顯示名稱分離，修正 Questionable 透過 IPC 啟動戰鬥時缺少 `SingleTarget` 分類的例外；API13 Release 建置 0 錯誤，發布 1.0.1.24。12 月節點雖仍標 API13，但已使用新版 Dalamud 型別，不相容台服 API13 |
| MapLinker | `Bluefissure/MapLinker` | `466c7c7753bf45590e504c6b32e0667b1750dabf` | 2025-08-17 | `cycleapple/MapLinker@8ef3ab1eec6c5fedacfca0b3a0293d90db4433fb` 完成一般使用者介面 zh-TW；保留聊天類型、指令 token、地圖連結解析、設定鍵與功能流程，發布 1.1.11.2 |
| AntiAfkKick | `NightmareXIV/AntiAfkKick` | `7a0ebaa8` | 2025-08-07 | `cycleapple/AntiAfkKick@8689ea7` 僅翻譯插件安裝頁說明；插件本身無設定介面；API13 編譯 0 警告、0 錯誤，發布 2.1.0.10 |
| AutoRetainer | `PunishXIV/AutoRetainer` | `1e4e6b6` / tag `4.5.1.12` | 2025-08-15 | `cycleapple/AutoRetainer@6afc52e` 保留繁中公會工坊／組件功能比對，並參考 AutoRetainerLocalizer zh-TW 補齊物品欄整理、工房航線工具、浮層、通知、操作選單與登入覆蓋層服務帳戶選擇；以 .NET SDK 10.0.302 建置（40 個既有警告、0 錯誤），發布 4.5.1.29 |
| Saucy | `PunishXIV/Saucy` | `8e8d5949` | 2025-08-15 | 台服修正 `cycleapple/Saucy@a79b1c5`；`cycleapple/Saucy@5c751d1` 翻譯主介面與九宮幻卡 zh 資源，並修正語言檔未嵌入 DLL 的問題；API13 編譯成功（8 個上游警告、0 錯誤），發布 1.4.2.9 |
| NoClippy | `UnknownX7/NoClippy` | `d32ae7af` | 2025-08-09 | `cycleapple/NoClippy@934ab0f` 僅翻譯設定、技能後搖、戰鬥統計、記錄選項、狀態預測警告與指令回覆；API13 編譯 0 警告、0 錯誤，發布 0.5.0.20 |
| NecroLens | `Jukkales/NecroLens` | `d6646478` | 2025-11-26 | `cycleapple/NecroLens@aad2e7b` 保留 `BaseId` API13 修正，完成 92 鍵 zh-TW 資源並補齊本地化協助與匿名資料收集介面；台服 API13 建置 0 警告、0 錯誤並發布 1.0.8.13 |
| GatherBuddy Reborn | `AtmoOmen/GatherBuddyReborn` | `a34733dc` / tag `7.3.5.0` | 2025-12-02 | 位於安全日期範圍且 manifest 為 API13；`cycleapple/GatherBuddyReborn@81c2f89d` 保留台服繁中 fallback、`DataId`、AutoHook IPC 容錯、時間文字編碼與區域資料修正；參考 `aliceric27/DalamudPlugins-TW` 移植分級防卡死及定期指令，並修正升級措施未受近端失敗次數限制、區域中心不重設、Lifestream 僅固定等待，以及強制傳送後同幀仍繼續採集等缺口；API13 Release 建置 0 錯誤，發布 7.3.5.7 |
| Artisan | `MeowZWR/Artisan` + `4liang0121/Artisan@6d10618` | `e4a0ddaf` | 2026-08-21 | `cycleapple/Artisan@fdf0e35` 保留台服 API13、Raphael 生命週期與宇宙配方選取修正；重新實作具配方／求解器／消耗品驗證及完整清除生命週期的暫時 IPC，並採用預設關閉的附近玩家巨集延遲。排除玩具性共通巨集及未具來源的 Raphael binary 更新；封裝內 binary SHA-256 與 4.0.4.24 相同；API13 Release 建置 0 錯誤，發布 4.0.4.25；上游已封存 |
| Burning Down the House | `LeonBlade/BDTHPlugin` | `ba39d13c` | 2025-09-30 | `cycleapple/BDTHPlugin@e1f7d27` 補齊指令說明、家具清單標題與座標欄位，保留 ImGui ID 與放置邏輯；台服 API13 建置 0 警告、0 錯誤並發布 1.7.1.2 |
| Raphael.Dalamud | `Dalamud-DailyRoutines/Raphael.Dalamud` | `de11e646` | 2025-09-16 | `cycleapple/Raphael.Dalamud@583151a` 完成 manifest zh-TW；台服 API13 建置 0 警告、0 錯誤並發布 0.0.5.1 |
| Something Need Doing | `Jaksuhn/SomethingNeedDoing` | `11422e55` | 2025-11-28 | `cycleapple/SomethingNeedDoing@0d05161` 完成主要 zh-TW 介面；台服 API13 建置僅 2 個 AutoRetainerAPI 既有參考警告、0 錯誤並發布 0.0.0.1 |
| TextAdvance | `cycleapple/TextAdvance` (`api13-tw`) | `f8a7cf5` | 2025-11-22 基底 | API13 編譯成功；繁中介面發布 3.2.4.8 |
| Lifestream | `NightmareXIV/Lifestream` | API13 相容節點 | 2025 | `cycleapple/Lifestream@8d1b5f7` 保留台服世界 ID 與名稱解析修正；參考 `aliceric27/DalamudPlugins-TW` 移植 `/li ren` 返回住所並互動傳喚鈴，以及 Custom Alias 等待、自訂 Slash 指令；另加入無可用住所提示、傳喚鈴 30 秒逾時停止及指令格式／長度驗證，並維持既有 enum 數值避免舊設定錯位；API13 Release 建置 25 個既有警告、0 錯誤，發布 2.5.3.9 |
| vnavmesh | `awgil/ffxiv_navmesh` | `5f512e5` / tag `v1.1.2.1` | 2025-12-15 | API13 編譯成功；`cycleapple/ffxiv_navmesh@93b4eac` 完成主要介面 zh-TW，改依有效 layout 模型逐對建立月面 Cosmoliner 連線，並只在三個外圈站點皆存在時加入 SS 與隧道間的雙向連線；API13 Release 建置 0 錯誤，發布 1.1.2.5。上游於 12 月 17 日才切換 API14 |
| AutoDuty | `ffxivcode/AutoDuty` | `a7d1eca8` | 2025-12-08 | `cycleapple/AutoDuty@6577a44` 保留路徑分頁容錯、zh-TW 介面與 RSR IPC 修正；參考 `aliceric27/DalamudPlugins-TW` 移植持久化副本排程器，並與既有記憶體 Playlist 分離；只有 `DutyCompleted` 才計數，加入兩秒事件去重、停止後續跑、整份循環、全清單執行前驗證及進副本時重套指定路徑；API13 Release 建置 67 個既有警告、0 錯誤，發布 0.0.0.9 |
| Pixel Perfect | `Haplo064/PixelPerfect` | `b371fe07` | 2025-08-07 | `cycleapple/PixelPerfect@80adfa2` 僅翻譯歡迎頁、設定、圖形參數、匯入／匯出通知、編輯器與說明；API13 編譯成功（4 個上游 nullable 警告、0 錯誤），發布 3.3.2.1 |
| LazyLoot | `PunishXIV/LazyLoot` | `d685ef0c` | 2025-11-19 | `cycleapple/LazyLoot@994d7ad` 完成設定介面、指令說明、狀態列、擲骰結果與診斷訊息繁中化；保留指令參數、設定格式與擲骰邏輯；台服 API13 編譯成功（2 個既有警告、0 錯誤），發布 5.3.2.5 |
| YesAlready | `PunishXIV/YesAlready` | `ca2288dd` | 2025-11-10 | `cycleapple/YesAlready@619d0a3` 建立 API13 fork 並完成主要 zh-TW 介面；建置僅 4 個既有 nullable／unused 警告、0 錯誤並發布 0.0.0.1 |
| Price Insight | `cycleapple/ffxiv-priceinsight` (`api13-tw`) | `b90564e` | 2025-08-07 基底 | API13 編譯成功；繁中介面發布 2.11.3.1 |
| MidiBard 2 | `reckhou/MidiBard2` | `1665029` | 2025-11-30 | API13 編譯成功；`cycleapple/MidiBard2@d141b5d` 修正 SDK 與台服組件路徑並補齊 zh-TW 介面資源，發布 3.2.1.3。下一提交開始誤用 API14 `IPlayerState` |
| Questionable | `PunishXIV/Questionable` | `34735346f` / tag `v13.68.129.2` | 2025-12-15 | `cycleapple/Questionable@2e935d9e8` 保留 TC-BASE 相容修正並完成使用者介面 zh-TW；將 2025-10-23 新版 RSR 的 `TargetOnly` IPC 合約回配至台服安全版 RSR 7.3.5（`Manual=2`），並讓 Pandora 選用 IPC 未就緒時安靜重試；API13 Release 建置 0 錯誤、5 個既有警告，發布 13.68.129.7 |
| Gearsetter | `VeraNala/Gearsetter` | `21a2b8c` / tag `v4.0` | 2025-08-10 | 使用原始鎖定的 `qstxiv/LLib@f1716ee`；`cycleapple/Gearsetter@357ce36` 完成主要 zh-TW 介面，台服 API13 建置 0 警告、0 錯誤並發布 4.0.0.1 |
| Ice's Cosmic Exploration | `cycleapple/Ices-Cosmic-Exploration` + `4liang0121/Ices-Cosmic-Exploration@21a4935` | `92a01bd` | 2026-08-21 | 保留 ECommons、台服 API13、zh-TW、任務預設與既有復原修正；採用 Agenda、任務偏好／停止條件、超時計分、後續任務、旅行規劃、採集角度資料及唯讀路線稽核。製作設定改接安全且可清除的 Artisan IPC；據點回程與緊急傳送預設關閉，56 份路線 YAML 已解析及範圍驗證。排除 fork 的舊暫時 IPC 與玩具性共通巨集；API13 Release 建置 0 錯誤，發布 0.0.73.52 |
| BOCCHI | `OhKannaDuh/BOCCHI` | `01d22a8565` / release `1.0.1` | 2025-12-07 | 原始碼與 manifest 均為 API13；`cycleapple/BOCCHI@4ccbbd1` 更新 legacy NuGet 鎖定資料、修正實際組件版本，並將 22 份中文語系資源轉為台灣繁中，發布 1.0.1.1 |
| Umbra XIV | `una-xiv/umbra` | `2d165ce` | 2025-10-08 | `Dalamud.NET.Sdk/13.0.0`；`cycleapple/umbra@ba18260` 將 1568 個既有中文介面鍵轉為台灣繁中並以台服 API13 編譯，發布 3.1.7.1。後期提交開始使用台服 API13 不存在的 `BaseId` 與 `IObjectTable.LocalPlayer` |
| MissFisher | `BlackCleaverLoli/MissFisher` | `80274683` | 2026-07-30 | `cycleapple/MissFisher@18f70b2` 改以上游正式 API13 版 1.6.5.11 DLL 為基底，保留官方驗證流程；回移 GatherBuddy Reborn 安裝／載入偵測及 `GatherBuddyReborn` 正確內部名稱，僅以 Mono.Cecil 置換 585 組台灣繁中資源並標記 1.6.5.13 |
| Skippy | `BoxuChan/Skippy` | `61c7c4f` | 2025-08-12 | 上游 manifest 與 Packager 均為 API13；`cycleapple/Skippy@4bad10c` 完成 zh-TW 回饋與指令說明，台服 API13 建置 0 警告、0 錯誤並發布 1.2.2.9 |
| AutoHook | `PunishXIV/AutoHook` | `081cab55` / tag `v5.0.0.23` | 2025-12-03 | 位於安全日期範圍且 manifest 為 API13；包含 GatherBuddy 7.3.5 所需的 `GetPluginState`、`GetAutoStartFishing` 與 `SetAutoStartFishing` IPC；`cycleapple/AutoHook@16103ca` 套用台服 `DataId` 相容修補及完整 zh-TW 介面，發布 5.0.0.14 |
| Avarice | `PunishXIV/Avarice` | `0c831ce` | 2025-09-02 | `cycleapple/Avarice@86f3ef1` 使用 API13 相依節點並完成主要 zh-TW 介面；建置僅 6 個既有 ECommons 警告、0 錯誤，發布 2.1.1.8 |
| Orbwalker | `PunishXIV/Orbwalker` | `caf40f9` | 2025-09-13 | SDK 與 manifest 均為 API13；`cycleapple/Orbwalker@07bec91` 完成主要 zh-TW 介面，建置僅 1 個既有 nullable 警告、0 錯誤並發布 1.0.1.7 |
| Palace Pal | `PunishXIV/PalacePal` | `bac8abe` | 2025-10-09 | SDK 13.1、manifest API13；`cycleapple/PalacePal@44afb5b` 新增完整 zh-TW 資源，台服 API13 建置及套件資源驗證成功，發布 4.14.0.1 |
| Pandora's Box | `PunishXIV/PandorasBox` | `01f457f` | 2025-10-12 | 採用 API14 屬性切換前的 API13 節點；`cycleapple/PandorasBox@dfb297a` 完成主要 zh-TW 介面，建置僅 84 個上游既有警告、0 錯誤並發布 1.6.3.19 |
| Marketbuddy | `PunishXIV/Marketbuddy` | `cf9d24d` | 2025-08-07 | DalamudPackager 13.0.0；`cycleapple/Marketbuddy@29f1e6a` 完成主要 zh-TW 介面，台服 API13 建置 0 警告、0 錯誤並發布 0.2.4.1 |
| JobBars | `0ceal0t/JobBars` | `48cbbce` | 2025-08-16 | SDK 與 manifest 均為 API13；`cycleapple/JobBars@api13-tw` 使用原始鎖定的 KamiToolKit 節點，以台服 API13 編譯成功並發布 1.3.2.1 |
| NotificationMaster | `NightmareXIV/NotificationMaster` | `8674bc5` | 2025-11-05 | manifest 與 DalamudPackager 為 API13、ECommons 鎖定 `3.0.0.18-api13`；`cycleapple/NotificationMaster@api13-tw` 使用原始 NotificationMasterAPI 子模組，以台服 API13 編譯成功並發布 2.1.1.11 |
| CBT（Automaton） | `Jaksuhn/ffxiv-bundleoftweaks` | `80d0545` / tag `v69.103` | 2025-11-16 | `cycleapple/ffxiv-bundleoftweaks@bec5da9` 保留 `BaseId`／`IPartyMember.EntityId` API13 修正並完成主要 zh-TW 介面；建置僅 3 個既有相依警告、0 錯誤並發布 69.103.0.1 |
| GatheringPathRenderer | `PunishXIV/Questionable` | `34735346f` / tag `v13.68.129.2` | 2025-12-15 | 與 Questionable 使用同一 API13 安全基線；`cycleapple/Questionable@5c74be2cf` 保留台服 `DataId` 修正並完成獨立工具 zh-TW 介面，API13 建置成功並發布 0.10.0.1 |
| Deliveroo | `VeraNala/Deliveroo` | `76abfc8` / tag `v7.4` | 2025-08-07 | 上游明確標記「7.4 API13」；`cycleapple/Deliveroo@46dd632` 完成 zh-TW 介面並以台服 API13 DLL 建置成功，發布 7.4.0.1 |
| Chilled Leves | `LeontopodiumNivale14/ChilledLeves` | `28d3025` | 2025-10-22 | SDK 13，鎖定上游 ECommons 子模組；`cycleapple/ChilledLeves@70db34a` 補完 zh-TW 並修正 vnavmesh IPC 啟動競態，以台服 API13 DLL 建置成功（8 個既有警告、0 錯誤）並發布 1.0.1.22 |
| Explorer's Icebox | `LeontopodiumNivale14/Explorers-Icebox` | `816a5ba` | 2025-11-19 | SDK 13，鎖定 ECommons 與 Pictomancy 子模組；`cycleapple/Explorers-Icebox@c8c71dd` 完成 zh-TW 介面，主專案以既有相依輸出建置成功並發布 1.0.4.6；solution 仍有上游 ECommons/Pictomancy pack 問題 |
| Easier Faux Hollows | `awgil/vfaux` | `77b8b67d` / tag `v0.0.0.10` | 2025-10-31 | 原生 SDK / API13 安全節點；`cycleapple/vfaux@0f85fd5` 補正套件版本並以台服 API13 依賴編譯，0 警告、0 錯誤；發布 0.0.0.10 |
| Hyperborea | `kawaii/Hyperborea` | `21f6fa50` | 2025-11-12 | 原生 manifest API13 安全節點；`cycleapple/Hyperborea@api13-tw` 以台服 API13 依賴編譯，13 個上游警告、0 錯誤；發布 1.0.0.31 |
| AutoMinion | `Asuna/AutoMinion` | `07fb9427` | 2025-03-27 | 上游在指定日期範圍內沒有節點；`cycleapple/AutoMinion@c22463b` 將 SDK、Packager、ImGui binding 與 ECommons 實際移植至 API13；`cycleapple/AutoMinion@e1e208b` 僅翻譯設定、搜尋、按鈕、指令說明與 manifest；16 個上游警告、0 錯誤；較高風險，發布 1.0.0.2 |
| XIV 藏寶圖工具小幫手 | `cycleapple/xiv-party-treasure-helper` | `aaa94f7` | 2026-04-27 | 自有 API12 專案；`cycleapple/xiv-party-treasure-helper@054af73` 保留 API13 移植與 zh-TW 介面，新增可自訂聊天頻道及獨立的解碼後自動開地圖打旗標選項，0 警告、0 錯誤；發布 0.1.9.4 |
| Visland | `awgil/ffxiv_visland` | `f7f40e1` / tag `v0.0.0.137` | 2025-08-09 | 上游 API13 安全節點；`cycleapple/ffxiv_visland@006b620` 完成主要 zh-TW 介面，並將上一版誤植的 API14 `BaseId` 恢復為 API13 等價 `DataId`（16 處），台服 API13 建置 0 警告、0 錯誤並發布 0.0.0.138 |
| Chat 2 | `Infiziert90/ChatTwo` | `956e57a` | 2025-11-17 | 上游 API13 安全節點；`cycleapple/ChatTwo@b1861f3` 更新有漏洞的依賴，`cycleapple/ChatTwo@09814af` 第二輪補齊資料庫瀏覽／維護、搜尋、字體重設與內建 Web 聊天介面 zh-TW；主插件以台服 API13 編譯成功（15 個上游警告、0 錯誤），發布 1.32.0.2 |
| Doorbell | `Aida-Enna/Doorbell` | `0a01851` | 2025-08-09 | 上游明確更新 7.3 並使用 SDK 13；`cycleapple/Doorbell@9b59581` 僅翻譯設定視窗、指令說明、狀態訊息與預設通知文字；台服 API13 編譯 0 警告、0 錯誤，發布 1.0.4.1 |
| MultiHit | `Bluefissure/MultiHit` | `72d95e8f65` | 2025-08-18 | 上游原生 `Dalamud.NET.Sdk/13.0.0` 節點；`cycleapple/MultiHit@1357aab` 僅翻譯顯示文字、說明與通知，以台服 API13 編譯成功（340 個上游平台／nullable 警告、0 錯誤），發布 0.0.4.1 |
| Namingway | `reiichi001/NamingWay` | `f7987e3257` | 2025-03-29 | 指定日期範圍內沒有 API13 節點；`cycleapple/NamingWay@079d4c7` 將 SDK、ImGui binding、list clipper 與 texture handle 實際移植至 API13；`cycleapple/NamingWay@968bfb9` 僅翻譯介面與預設套組顯示名稱；1 個上游 nullable 警告、0 錯誤，發布 1.1.17.1 |
| Mappy | `harbingerftw/Mappy` | `9e9e4a3` | 2025-09-12 | 原生 `Dalamud.NET.Sdk/13.0.0` 安全節點；`cycleapple/Mappy@f7691eb` 完成設定、地圖工具列、右鍵選單、座標列、搜尋、任務／危命任務／旗標視窗與標記提示繁中化；保留地圖座標換算、標記資料、遊戲地名與設定鍵；台服 API13 編譯成功（3 個既有 API13 棄用警告、0 錯誤），發布 3.1.6.12 |
| ChatCoordinates | `kissorjeyabalan/dalamud-chatcoordinates` | `1303b7e` | 2025-08-09 | 上游提交明確標記 Dalamud SDK 13；`cycleapple/dalamud-chatcoordinates@eeb5db3` 完成設定、指令說明、聊天提示與錯誤訊息繁中化，並採用官方台服地名「雷克蘭德」作為範例；未更動座標解析、分隔符號與傳送參數；台服 API13 編譯 0 警告、0 錯誤，發布 2.1.2.10 |
| FPS Plugin | `Caraxi/FPSPlugin` | `9eaf5e4` | 2025-08-08 | 上游 API13 安全節點；`cycleapple/FPSPlugin@a14f297` 完成設定介面、DTR 工具提示、平均／最低標籤與指令說明繁中化；保留指令參數與 FPS 計算邏輯；台服 API13 編譯 0 警告、0 錯誤，發布 1.7.0.5 |
| Craftimizer | `WorkingRobot/Craftimizer` | `88a1be2` | 2025-10-20 | 指定日期範圍內最後的原生 SDK 13 節點；`cycleapple/Craftimizer@6edb361` 完成主要 zh-TW 介面，建置僅 7 個既有分析警告、0 錯誤並發布 2.8.0.2 |
| SortaKinda | `MidoriKami/SortaKinda` | `e5b566d` | 2025-08-13 | 原生 SDK 13 節點；鎖定的 KamiToolKit 使用已禁止的 `byte LabelId` 多載，`cycleapple/KamiToolKit@76dacbc` 僅將三處參數修正為 API13 要求的 `ushort`；`cycleapple/SortaKinda@api13-tw` 保留完整 zh-TW 介面，將原生物品欄排序由並行背景 Task 改為 framework thread 依序執行，合併重複請求並加入 ItemOrderModule、InventoryManager、容器與欄位邊界防護；台服 API13 編譯 0 警告、0 錯誤，發布 2.1.1.8 |
| QoL Bar | `UnknownX7/QoLBar` | `7ee0a6e` | 2025-08-11 | 指定日期範圍內的原生 SDK13／FFXIV 7.3 節點；`cycleapple/QoLBar@77ed099` 保留 `AddonConfig.ActiveDataSet` 相容修正與完整 zh-TW 介面，另以 `AddDalamudDefaultFont` 取代台服執行環境中用途不符的硬編碼 Noto 字型資產；指令語法、條件 ID、IPC、匯出格式與設定序列化未變更；台服 API13 編譯成功（2 個既有未指派欄位警告、0 錯誤），發布 2.3.3.8 |
| IINACT | `PlusoneChiang/IINACT` | 上游正式版 1.13.9.6 | 2026-07-31 | 清單直接引用 `https://plusonechiang.github.io/IINACT/repo.json` 所列 GitHub Release、來源與圖示；本倉庫不再 fork、修改、重編、中文化或發布自建替代套件 |
| LMeter | `juicefish/LMeter_TC` | `3bee085` | 2026-07-28 | 使用者指定的台服 API13 分支，原始 repo.json 宣告 API13 1.13.0.1；`cycleapple/LMeter_TC@1052d57` 修正可覆寫的 Dalamud 路徑、更新 fork 資訊與繁中 manifest，並完成設定、統計欄位、右鍵選單與提示的 zh-TW 介面翻譯；IPC 名稱、ACT 欄位、格式標籤、設定鍵與計算邏輯維持不變；台服 API13 編譯 0 警告、0 錯誤，發布 1.13.0.3 |
| Distance | `PunishedPineapple/Distance` | `aa7027c352` | 2025-08-07 | API13 更新後的正式節點；`cycleapple/Distance@api13-tw` 以台服 Dalamud 13.0.0.8／.NET 9 重建成功，1 警告、0 錯誤，發布 1.1.3.3 |
| EnemyListHP | `NightmareXIV/EnmityHp` | `1f587890e4` | 2025-08-07 | 上游 7.3／API13 節點；`cycleapple/EnmityHp@api13-tw` 以台服 Dalamud 13.0.0.8 重建成功，1 警告、0 錯誤，發布 2.0.1.7 |
| ReAction | `UnknownX7/ReAction` | `f539d8ea69` | 2025-08-11 | 上游 7.3 修正後的 SDK13 節點；`cycleapple/ReAction@api13-tw` 重建成功，僅保留上游警告，發布 1.3.4.2 |
| Radar Plugin | `KangasZ/RadarPlugin` | `461df22fe2` | 2025-10-09 | 採用有完整原始碼的 Radar Plugin API13 節點，不使用僅提供 API10 二進位檔的 akira0245 鏡像；`cycleapple/RadarPlugin@api13-tw` 重建成功，發布 2.1.8.1 |
| ReMakePlace Plugin | `ReMakePlace/plugin` | `f9b5648e18` | 2025-12-02 | API14 更新前最後一批 API13 變更；`cycleapple/ReMakePlacePlugin@179bd50` 明確化 ECommons ref lambda 型別，並將 API13.1 才有的 `IObjectTable.LocalPlayer` 改回 API13.0.0.8 可用的 `IClientState.LocalPlayer`；功能流程不變，重建成功，發布 7.3.3.0 |
| DozeAnywhere | `Warpholomey/DozeAnywhere` | `00c6ab37db` | 2025-08-09 | 上游明確標示 Dalamud API13 的節點；`cycleapple/DozeAnywhere@api13-tw` 以台服 API13 重建 0 警告、0 錯誤，發布 13.1.0.0 |
| Cammy | `UnknownX7/Cammy` | `d015ed2725` | 2025-08-11 | 上游 7.3 修正後的 SDK13 節點；連同固定版 Hypostasis 子模組重建成功，發布 2.1.0.13 |
| Gauge-O-Matic | `ItsBexy/GaugeOMatic` | `4e889d0a1c` | 2025-09-03 | 上游 7.31／SDK13.1 節點；對台服 Dalamud 13.0.0.8 重建成功，2 個過時 API 警告、0 錯誤，發布 0.8.2.1 |
| EngageTimer | `xorus/EngageTimer` | `d436096f67` | 2025-08-08 | 上游 SDK13 更新節點；對台服 Dalamud 13.0.0.8 重建 0 警告、0 錯誤，發布 2.4.4.0 |
| BigPlayerDebuffs | `rgd87/BigPlayerDebuffs` | `a948648cd4` | 2025-08-08 | API13 更新後的版本節點；對台服 API13 重建成功，警告為上游平台分析提示，發布 1.1.0.13 |
| Better Mount Roulette | `CMDRNuffin/BetterMountRoulette` | `98d2574` | 2025-08-10 | 沒有採用 2025-11 後依賴 `IPlayerState` 的 API13.1 節點，改採可直接對台服 Dalamud 13.0.0.8 重建的最後安全節點；`cycleapple/BetterMountRoulette@api13-tw` 0 警告、0 錯誤，發布 1.0.0.0 |
| Submarine Tracker | `Infiziert90/SubmarineTracker` | `7167f242` | 2025-11-17 | API14 切換前最後的 SDK13 節點；`cycleapple/SubmarineTracker@44f1f54` 將 MessagePack 3.1.4 更新為無已知 NuGet 漏洞的 3.1.8，台服 Dalamud 13.0.0.8 編譯成功（4 個既有 nullable／未使用欄位警告、0 錯誤），發布 2.0.2.1 |
| Party Icons | `nebel/xivPartyIcons`（`shdwp/xivPartyIcons` fork 家族） | `22e5bb8a` | 2025-08-07 | 原始 `shdwp` 倉庫停在 2023 年 net7，採用同一 fork 家族中明確標示 API13 的維護節點；`cycleapple/xivPartyIcons@34de4cc` 以台服 Dalamud 13.0.0.8 編譯成功（4 個既有 nullable／未使用變數警告、0 錯誤），發布 1.2.3.2 |
| RezPls | `Ottermandias/RezPls` | `53cffe4b` | 2025-09-06 | 截止日期內最後的 SDK13 節點；上游於 2025-12-18 才發布後續版本並切換新版 SDK；`cycleapple/RezPls@fef85ac` 以台服 Dalamud 13.0.0.8 編譯成功，0 警告、0 錯誤，NuGet 漏洞掃描零筆，發布 1.5.2.1 |
| FlyTextFilter | `Aireil/FlyTextFilter` | `8b9ff55` | 2025-08-06 | 上游在 2025-08-05 依序完成台服 7.3 signature、SDK13、FlyTextKind 與 ImGui bindings 修正，隔日發布 4.4.0.0；2025-12-18 才切換 API14。`cycleapple/FlyTextFilter@64bc27c` 完成全部可見 zh-TW 介面，以台服 API13 建置 0 警告、0 錯誤並發布 4.4.0.3 |
| Allagan Market | `Critical-Impact/AllaganMarket` | `334b5036b` | 2025-10-17 | 指定日期窗內最後版本，已包含 API13 遷移與 MarketPriceUpdater hook 簽章修正；`cycleapple/AllaganMarket@88ec1706` 新增 269 組 zh-TW 資源並保持 14 個 CSV 欄位識別為英文，以台服 Dalamud 13.0.0.8 編譯成功（155 個既有警告、0 錯誤），封裝四個 AllaganLib DLL 並發布 1.2.0.8 |
| Allagan Tools | `Critical-Impact/InventoryTools` | `c542405ba` / tag `13.1.9` | 2025-11-25 | 指定日期窗內最後正式 API13 tag，包含非英文語言與 history 載入修正；`cycleapple/InventoryTools@0f9b9ba` 搭配 `cycleapple/CriticalCommonLib@de2e398` 回移上游僱員市集掃描修正，改由 API13 ClientStructs 讀取掛賣價格並移除易失效的價格封包 Hook；API13 完整重建 0 錯誤，發布 1.13.1.13 |
| Allagan Item Search | `Critical-Impact/AllaganItemSearch` | `b98604801` | 2025-08-09 | 指定日期窗內唯一提交且明確標記 API13；無原生 hook 或 git submodule；`cycleapple/AllaganItemSearch@ec56178e` 新增 236 個 zh-TW 資源鍵並覆蓋 119/119 renderer 名稱，以台服 Dalamud 13.0.0.8 編譯成功（862 個既有 nullable／StyleCop 警告、0 錯誤），發布 1.0.0.4 |
| Title Edit | `RokasKil/TitleEdit` | `22610f1e` | 2025-12-07 | 採用上游 v3.0.6.2 的 API13 節點；`cycleapple/TitleEdit@64aa036` 完成全部可見 zh-TW 介面，並保留 `IsMountUnlocked` 台服 API13 ClientStructs 相容修正，建置 0 警告、0 錯誤並發布 3.0.6.22 |
| MonsterDex | `wolfcomp/MonsterDex` | `3241c74e` | 2025-10-29 | 採用上游 v2.13.6 API13 發布節點；`cycleapple/MonsterDex@cbe5f57` 搭配 `api13-tw-l10n@262a33e` 完成 zh-TW 介面與資料分支，發布 2.13.6.2 |
| High FPS Physics Fix | `LunaYup/xivlauncher_physics_plugin` | `7cadd26f` | 2025-08-06 | 採用切換至 Dalamud.NET.Sdk 後的 API13 節點；`cycleapple/xivlauncher_physics_plugin@82249e88` 加入繁中介面，發布 8.3.0.1 |
| Orchestrion Plugin | `perchbirdd/OrchestrionPlugin` | `3496bbec` | 2025-08-07 | 採用完成 7.3 更新後的 API13 節點；`cycleapple/OrchestrionPlugin@9272d64` 完成 115 鍵 zh-TW 介面並發布 2.2.0.13 |
| CrossUp | `ItsBexy/CrossUp` | `96daa53b` | 2025-09-03 | 採用上游 1.7.1.1 的 7.31／API13 節點；`cycleapple/CrossUp@c66ec1f` 完成 121 鍵 zh-TW 介面並發布 1.7.1.14 |
| TriadBuddy | `MgAl2O4/FFTriadBuddyDalamud` | `acb68f2d` | 2025-08-11 | 採用 API13／7.3 安全節點；`cycleapple/FFTriadBuddyDalamud@9dbf132` 修復中文亂碼並完成 64 鍵 zh-TW，發布 1.13.0.2 |
| MeterWay | `CondeSaheki/MeterWay` | `67036051` | 2025-04-12 | 安全日期窗內沒有上游提交，採用最後正式版 v1.0.16；`cycleapple/MeterWay@3413abf` 在最小 API13 移植上完成深層 zh-TW 介面，建置 0 警告、0 錯誤並發布 1.0.17.2 |
| Death Recap | `Kouzukii/ffxiv-deathrecap` | `fdc149f4` | 2025-08-10 | 採用上游 API13 更新後的安全節點；`cycleapple/ffxiv-deathrecap@c95d352` 完成主要 zh-TW 介面並發布 1.13.2.3 |
| Teleporter | `pohky/TeleporterPlugin` | `98a943a9` | 2025-08-07 | 上游於 `21434980` 明確更新 API13，下一次 API14 更新為 2025-12-17；`cycleapple/TeleporterPlugin@199a31a` 完成 zh-TW 介面，並將 API13 Sanitizer 不支援的繁中、簡中及其他擴充語言安全映射至非破壞性英文路徑；0 警告、0 錯誤，發布 2.0.2.11 |
| DailyDuty | `MidoriKami/DailyDuty` | `bff73018` | 2025-08-22 | 採用 API13 安全節點並固定台服相容 KamiToolKit；`cycleapple/DailyDuty@0c4ba7a0` 完成 216 鍵 zh-TW 資源並發布 5.3.2.14 |
| ezMiniCactpot | `MidoriKami/MiniCactpotSolver` | `761b4e22` | 2025-08-26 | 採用修正 LoadConfigFile 後的 API13 節點及相容 KamiToolKit；`cycleapple/EzMiniCactpot@eef2252` 完成 zh-TW 介面並發布 3.0.0.4 |
| PingPlugin | `karashiiro/PingPlugin` | `5c0df982` | 2025-08-07 | 採用上游最後 API13 安全節點；`cycleapple/PingPlugin@f6a8386` 保留台服 TCP handshake 量測並完整校訂 zh-TW 介面，發布 2.9.0.2 |
| Sonar | `FFXIV-Sonar/SonarDistrib` | `4e798c2c37` | 2025-12-12 | 位於安全日期範圍內，原始專案使用 `Dalamud.NET.Sdk/13.1.0`，基準版本 0.7.4.2；`cycleapple/SonarDistrib@9c4c1d9` 完成可見介面與音效名稱 zh-TW 翻譯並升版至 0.7.4.4。此歷史節點的 MessagePack 3.1.4 與 SignalR MessagePack 9.0.10 會產生已知弱點警告，為避免破壞 Sonar 服務協定未擅自升級 |
| Waymark Preset Plugin | `Infiziert90/WaymarkPresetPlugin` | `bb2277a7ed` | 2025-08-07 | 上游 API13／1.5.5.0 節點；`cycleapple/WaymarkPresetPlugin@api13-tw` 以台服 Dalamud API13 重建成功 |
| Honorific | `Caraxi/Honorific` | `9364d4c085` | 2025-12-10 | 上游 SDK13.1 節點；`cycleapple/Honorific@897ea5a` 將 `IPlayerState.ContentId` 與 `IObjectTable.LocalPlayer` 安全映射至台服 API13 的 `IClientState`，重建成功並發布 1.7.1.3 |
| NOTED | `Tischel/NOTED` | `0be8c4835f` | 2025-08-09 | 上游 API13／1.6.0.0 節點；`cycleapple/NOTED@api13-tw` 以台服 Dalamud API13 重建成功 |
| Flash on Tell | `reiichi001/Dalamud-FlashOnTellPlugin` | `594d7df644` | 2025-08-06 | 上游 API13／0.0.9.0 節點；`cycleapple/Dalamud-FlashOnTellPlugin@api13-tw` 重建成功 |
| Custom Resolution | `0x0ade/DP-CustomResolution` | `fd83a52b1b` | 2025-12-15 | 位於安全日期範圍內的 API13／1.0.1.0 節點；鏡像至 `cycleapple/DP-CustomResolution@api13-tw` 後以台服 API13 重建成功 |
| Market Board | `fmauNeko/MarketBoardPlugin` | `6ee22ef827` | 2025-08-07 | tag 1.11.0 的 API13 節點；`cycleapple/MarketBoardPlugin@api13-tw` 重建並封裝 1.11.0.0 |
| Peeping Tom | `pyreymo/PeepingTom`（`thakyZ/PeepingTom` 維護分支） | `3898b2f3fb` | 2025-12-05 | 原倉庫停在 2023 年，採用保留完整功能的維護節點；`cycleapple/PeepingTom@9028ee2` 將 SDK15 API 安全回移至 API13 並固定鎖檔，重建成功，發布 1.7.13.1 |
| Eureka Linker | `Infiziert90/EurekaTrackerAutoPopper` | `ecd774f834` | 2025-11-23 | 上游 API13／1.5.9.5 節點；`cycleapple/EurekaTrackerAutoPopper@api13-tw` 重建成功 |
| Hunt Buddy | `SheepGoMeh/HuntBuddy` | `768413a68d` | 2025-08-08 | 上游 API13／1.2.2.0 節點；`cycleapple/HuntBuddy@api13-tw` 重建成功 |
| ZodiacBuddy | `foophoof/ZodiacBuddy` | `2ac308a0b6` | 2025-10-01 | 上游 SDK13.1／1.13.0.2 節點；`cycleapple/ZodiacBuddy@api13-tw` 可直接對台服 API13 重建成功 |
| EasyEyes | `mouuff/EasyEyes` | `fdab548c03` | 2025-08-31 | 與 PluginDistD17 指定資產相符的 API13／1.3.1.1 原始碼節點；`cycleapple/EasyEyes@api13-tw` 重建成功 |
| Fungah | `img02/Fungah-Totally-Safe-Spot` | `fe7a4548cd` | 2025-08-10 | 與 PluginDistD17 指定資產相符的 API13／1.0.0.7 原始碼節點；`cycleapple/Fungah-Totally-Safe-Spot@api13-tw` 重建成功 |
| Visibility | `SheepGoMeh/VisibilityPlugin` | `b4d18ae2bc` | 2025-08-08 | 上游 API13／1.1.9.1 節點；`cycleapple/VisibilityPlugin@9917750` 明確化台服 ClientStructs 的 `BattleNpcSubKind` 型別歧義，重建成功並發布 1.1.9.2 |
| Enemy List Debuffs | `mouuff/EnemyListDebuffs` | `3de258de9f` | 2025-08-09 | 與 PluginDistD17 指定資產相符的 API13／1.13.0.0 原始碼節點；`cycleapple/EnemyListDebuffs@api13-tw` 重建成功 |
| Penny Pincher | `tesu/PennyPincher` | `b26e81e0be` | 2025-08-09 | 上游 API13／1.8.0.6 節點；`cycleapple/PennyPincher@api13-tw` 重建成功 |
| Housemate | `perchbirdd/Housemate` | `1a097d3fc3` | 2025-08-07 | 上游 API13／1.0.3.4 節點；`cycleapple/Housemate@api13-tw` 重建成功 |
| Brio | `Etheirys/Brio` | `6d4e3bd` | 2026-08-18 | `cycleapple/Brio@api13-tw` 明確解除新建 GPose actor 的 Penumbra cutscene parent，檢查 collection／design IPC 回傳碼並發布 0.5.2.3；台服 API13 建置成功（既有 MessagePack 弱點與 3 個程式警告，0 錯誤） |
| Glamourer | `Ottermandias/Glamourer` | `97cd7f7` | 2026-08-20 | `cycleapple/Glamourer@api13-tw` 搭配 `cycleapple/Penumbra.GameData@d610cb7`，以物件索引取得 actor 時即時補入識別碼快取，修正 Brio／Ktisis 等工具新建 actor 後的 `Affecting nothing`；發布 1.5.0.15，台服 API13 建置 0 警告、0 錯誤 |
