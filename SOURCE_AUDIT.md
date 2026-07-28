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
| AutoRetainer | `PunishXIV/AutoRetainer` | `1e4e6b6` / tag `4.5.1.12` | 2025-08-15 | API13 編譯成功；實際組件版本 4.5.1.21 |
| Saucy | `PunishXIV/Saucy` | `8e8d5949` | 2025-08-15 | API13 編譯成功；台服修正 `cycleapple/Saucy@a79b1c5`；發布 1.4.2.8 |
| NoClippy | `UnknownX7/NoClippy` | `d32ae7af` | 2025-08-09 | API13 編譯成功；發布 0.5.0.19 |
| NecroLens | `Jukkales/NecroLens` | `d6646478` | 2025-11-26 | API13 編譯成功；`cycleapple/NecroLens@98cd7c2` 修正 `BaseId` 相容性並發布 1.0.8.11 |
| GatherBuddy Reborn | `AtmoOmen/GatherBuddyReborn` | `f77e7a44` | 2025-12-16 | API13 編譯成功；`cycleapple/GatherBuddyReborn@46666db` 修正 `BaseId` 相容性、更新 MessagePack 至 3.1.8，發布 7.2.5.1 |
| Artisan | `MeowZWR/Artisan` | `e4a0ddaf` | 2025-12-13 | API13 編譯成功；`cycleapple/Artisan@4c90707` 修正 `BaseId` 相容性，發布實際組件版本 4.0.4.8；上游已封存 |
| Burning Down the House | `LeonBlade/BDTHPlugin` | `ba39d13c` | 2025-09-30 | API13 編譯成功；發布 1.7.1.0 |
| Raphael.Dalamud | `Dalamud-DailyRoutines/Raphael.Dalamud` | `de11e646` | 2025-09-16 | API13 編譯成功；發布 0.0.5.0 |
| Something Need Doing | `Jaksuhn/SomethingNeedDoing` | `11422e55` | 2025-11-28 | API13 編譯成功；發布 0.0.0.0 |
| TextAdvance | `NightmareXIV/TextAdvance` | `5716d5a4` | 2025-11-22 | API13 編譯成功；發布 3.2.4.7 |
| Lifestream | `NightmareXIV/Lifestream` | `305dfbf9` / tag `2.5.2.3` | 2025-08-07 | API13 編譯成功；2.5.1.15 為 API12，故發布首批 API13 版本 2.5.2.3 |
| vnavmesh | `awgil/ffxiv_navmesh` | `5f512e57` | 2025-12-15 | API 由建置產生，含原生元件 |
| AutoDuty | `ffxivcode/AutoDuty` | `a7d1eca8` | 2025-12-08 | API13 編譯成功；實際組件版本 0.0.0.0 |
| Pixel Perfect | `Haplo064/PixelPerfect` | `b371fe07` | 2025-08-07 | API13 編譯成功；發布 3.3.2.0 |
| LazyLoot | `PunishXIV/LazyLoot` | `d685ef0c` | 2025-11-19 | API13 編譯成功；發布 5.3.2.4 |
| YesAlready | `PunishXIV/YesAlready` | `ca2288dd` | 2025-11-10 | API13 編譯成功；上游 manifest 版本為 0.0.0.0 |
| Price Insight | `Kouzukii/ffxiv-priceinsight` | `3c1c16d7` | 2025-08-07 | API13 編譯成功；發布 2.11.3.0 |
| MidiBard 2 | `midibard.org` | — | — | 閉源／需取得官方 API13 發布包 |
| Questionable | `git.carvel.li/liza/Questionable` | — | — | 待稽核非 GitHub 上游 |
| Gearsetter | `git.carvel.li/liza/Gearsetter` | — | — | 待稽核非 GitHub 上游 |
