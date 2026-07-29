# API13 Source Audit

稽核截止點為 2025-12-16 23:59:59 UTC。`已確認 API13` 只代表來源 manifest 已確認，仍需使用台服 API13 環境完成編譯與執行驗證。

| 插件 | 上游 | 截止 commit | 日期（UTC） | 初步結果 |
|---|---|---|---|---|
| Bossmod／Boss Mod | `awgil/ffxiv_bossmod` | `381151125` | 2025-11-29 | API13 編譯成功；`cycleapple/ffxiv_bossmod@1460e54d9` 修正台服型別與 C# 建置相容性，發布 0.1.4.0。後續開始使用 API14 `IPlayerState` |
| Bossmod Reborn | `FFXIV-CombatReborn/BossmodReborn` | `9222b6062` / tag `7.3.8.1` | 2025-11-24 | API13 編譯成功；`cycleapple/BossmodReborn@6338acdaa` 改用台服 ClientStructs 組件並修正 Dalamud 型別，發布 7.3.8.1。7.3.8.2 起已使用 API14 型別 |
| Rotation Solver Reborn | `FFXIV-CombatReborn/RotationSolverReborn` | `4907d030` / tag `7.3.5.0` | 2025-10-07 | API13 編譯成功；`cycleapple/RotationSolverReborn@8b9fb1d7` 鎖定 net9 相容 Lumina.Excel，發布 7.3.5.0。較晚的 7.3.8.x 雖標 API13，已使用 API14 型別 |
| Splatoon | `PunishXIV/Splatoon` | `ae37f2b` / tag `3.8.1.5` | 2025-08-28 | API13 編譯成功；來源 tag 的實際組件版本為 3.8.2.1 |
| Wrath Combo | `MeowZWR/WrathCombo` | `3b968ca32` | 2025-08-05 | API13 編譯成功；`cycleapple/WrathCombo@59b67130e` 發布 1.0.1.18。12 月節點雖仍標 API13，但已使用新版 Dalamud 型別，不相容台服 API13 |
| AntiAfkKick | `NightmareXIV/AntiAfkKick` | `7a0ebaa8` | 2025-08-07 | API13 編譯成功；發布 2.1.0.9 |
| AutoRetainer | `PunishXIV/AutoRetainer` | `1e4e6b6` / tag `4.5.1.12` | 2025-08-15 | API13 編譯成功；`cycleapple/AutoRetainer@9ec26a1` 修正繁中公會工坊／組件用語，發布 4.5.1.22 |
| Saucy | `PunishXIV/Saucy` | `8e8d5949` | 2025-08-15 | API13 編譯成功；台服修正 `cycleapple/Saucy@a79b1c5`；發布 1.4.2.8 |
| NoClippy | `UnknownX7/NoClippy` | `d32ae7af` | 2025-08-09 | API13 編譯成功；發布 0.5.0.19 |
| NecroLens | `Jukkales/NecroLens` | `d6646478` | 2025-11-26 | API13 編譯成功；`cycleapple/NecroLens@98cd7c2` 修正 `BaseId` 相容性並發布 1.0.8.11 |
| GatherBuddy Reborn | `AtmoOmen/GatherBuddyReborn` | `f77e7a44` | 2025-12-16 | API13 編譯成功；`cycleapple/GatherBuddyReborn@46666db` 修正 `BaseId` 相容性、更新 MessagePack 至 3.1.8，發布 7.2.5.1 |
| Artisan | `MeowZWR/Artisan` | `e4a0ddaf` | 2025-12-13 | API13 編譯成功；`cycleapple/Artisan@4c90707` 修正 `BaseId` 相容性，發布實際組件版本 4.0.4.8；上游已封存 |
| Burning Down the House | `LeonBlade/BDTHPlugin` | `ba39d13c` | 2025-09-30 | API13 編譯成功；發布 1.7.1.0 |
| Raphael.Dalamud | `Dalamud-DailyRoutines/Raphael.Dalamud` | `de11e646` | 2025-09-16 | API13 編譯成功；發布 0.0.5.0 |
| Something Need Doing | `Jaksuhn/SomethingNeedDoing` | `11422e55` | 2025-11-28 | API13 編譯成功；發布 0.0.0.0 |
| TextAdvance | `NightmareXIV/TextAdvance` | `5716d5a4` | 2025-11-22 | API13 編譯成功；發布 3.2.4.7 |
| Lifestream | `NightmareXIV/Lifestream` | `305dfbf9` / tag `2.5.2.3` | 2025-08-07 | API13 編譯成功；`cycleapple/Lifestream@e6f5ec0` 修正繁中「移動到公會工坊」選單辨識，發布 2.5.2.4 |
| vnavmesh | `awgil/ffxiv_navmesh` | `5f512e5` / tag `v1.1.2.1` | 2025-12-15 | API13 編譯成功；`cycleapple/ffxiv_navmesh@8d90451` 發布 1.1.2.1。上游於 12 月 17 日才切換 API14 |
| AutoDuty | `ffxivcode/AutoDuty` | `a7d1eca8` | 2025-12-08 | API13 編譯成功；實際組件版本 0.0.0.0 |
| Pixel Perfect | `Haplo064/PixelPerfect` | `b371fe07` | 2025-08-07 | API13 編譯成功；發布 3.3.2.0 |
| LazyLoot | `PunishXIV/LazyLoot` | `d685ef0c` | 2025-11-19 | API13 編譯成功；發布 5.3.2.4 |
| YesAlready | `PunishXIV/YesAlready` | `ca2288dd` | 2025-11-10 | API13 編譯成功；上游 manifest 版本為 0.0.0.0 |
| Price Insight | `Kouzukii/ffxiv-priceinsight` | `3c1c16d7` | 2025-08-07 | API13 編譯成功；發布 2.11.3.0 |
| MidiBard 2 | `reckhou/MidiBard2` | `1665029` | 2025-11-30 | API13 編譯成功；`cycleapple/MidiBard2@6f062cb` 修正 SDK 與台服組件路徑，發布 3.2.1.2。下一提交開始誤用 API14 `IPlayerState` |
| Questionable | `PunishXIV/Questionable` | `34735346f` / tag `v13.68.129.2` | 2025-12-15 | API13 編譯成功；`cycleapple/Questionable@f71531737` 適配台服 TC-BASE。程式內放棄任務因缺少安全原生介面而停用，其餘核心功能保留 |
| Gearsetter | `VeraNala/Gearsetter` | `21a2b8c` / tag `v4.0` | 2025-08-10 | API13 編譯成功；`cycleapple/Gearsetter@api13-tw` 發布 4.0，使用原始鎖定的 `qstxiv/LLib@f1716ee` |
| Ice's Cosmic Exploration | `LeontopodiumNivale14/Ices-Cosmic-Exploration` | `f3b7a696c9` | 2025-12-15 | `cycleapple/Ices-Cosmic-Exploration@9ced6b4` 將 ECommons 鎖回台服 API13 相容節點、以 `DataId` 取代後期 `BaseId` 並改用 `Player.JobId`，發布 0.0.73.40 |
| BOCCHI | `OhKannaDuh/BOCCHI` | `01d22a8565` / release `1.0.1` | 2025-12-07 | 原始碼與 manifest 均為 API13；`cycleapple/BOCCHI@d138a58` 更新 legacy NuGet 鎖定資料並修正實際組件版本，發布 1.0.1.0 |
| Umbra XIV | `una-xiv/umbra` | `2d165ce` | 2025-10-08 | `Dalamud.NET.Sdk/13.0.0`；以台服 API13 乾淨編譯 0 警告、0 錯誤，發布 3.1.7.0。後期提交開始使用台服 API13 不存在的 `BaseId` 與 `IObjectTable.LocalPlayer` |
| MissFisher | `BlackCleaverLoli/MissFisher` | `93487c5` | 2025-12-13 | 上游只發布 1.6.5.9 二進位套件、未公開原始碼；`cycleapple/MissFisher@a60af53` 在倉庫與套件 manifest 補上 API13 宣告，DLL 保持上游原檔，無法聲稱重編譯 |
| Skippy | `BoxuChan/Skippy` | `61c7c4f` | 2025-08-12 | 上游 manifest 與 Packager 均為 API13；`cycleapple/Skippy@e0a99f3` 修正組件版本與 repo 版本不一致，台服 API13 編譯成功，發布 1.2.2.8 |
| AutoHook | `PunishXIV/AutoHook` | `e5bd183` | 2025-11-09 | `cycleapple/AutoHook@1e845af` 將後期 `BaseId` 改回台服 API13 的 `DataId`，發布 5.0.0.12 |
| Avarice | `PunishXIV/Avarice` | `0c831ce` | 2025-09-02 | `cycleapple/Avarice@c7fd996` 使用 API13 相依節點並移除未使用的 Windows Forms using，台服 API13 0 警告、0 錯誤，發布 2.1.1.7 |
| Orbwalker | `PunishXIV/Orbwalker` | `caf40f9` | 2025-09-13 | SDK 與 manifest 均為 API13；台服 API13 編譯成功，發布 1.0.1.6 |
| Palace Pal | `PunishXIV/PalacePal` | `bac8abe` | 2025-10-09 | SDK 13.1、manifest API13；台服 API13 編譯成功，發布 4.14.0.0 |
| Pandora's Box | `PunishXIV/PandorasBox` | `01f457f` | 2025-10-12 | API13 編譯成功，發布 1.6.3.18；10 月 31 日後的提交開始改用台服 API13 不存在的 `IPartyMember.EntityId` 與 `BaseId` |
| Marketbuddy | `PunishXIV/Marketbuddy` | `cf9d24d` | 2025-08-07 | DalamudPackager 13.0.0 並直接連結台服 API13 DLL 編譯成功，發布 0.2.4.0 |
