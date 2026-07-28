# API13 Source Audit

稽核截止點為 2025-12-16 23:59:59 UTC。`已確認 API13` 只代表來源 manifest 已確認，仍需使用台服 API13 環境完成編譯與執行驗證。

| 插件 | 上游 | 截止 commit | 日期（UTC） | 初步結果 |
|---|---|---|---|---|
| Bossmod／Boss Mod | `awgil/ffxiv_bossmod` | `83776902` | 2025-12-16 | API 由建置產生，待編譯確認 |
| Bossmod Reborn | `FFXIV-CombatReborn/BossmodReborn` | `83776902` | 2025-12-16 | 與經典版同 commit，需確認 fork 差異 |
| Rotation Solver Reborn | `FFXIV-CombatReborn/RotationSolverReborn` | `f24bf4bc` | 2025-12-15 | 已確認 API13 |
| Splatoon | `PunishXIV/Splatoon` | `f7434a3d` | 2025-12-08 | 已確認 API13 |
| Wrath Combo | `MeowZWR/WrathCombo` | `dff5e3c0` | 2025-12-16 | 此節點已是 API14，需找更早 API13 commit |
| AntiAfkKick | `NightmareXIV/AntiAfkKick` | `7a0ebaa8` | 2025-08-07 | API13 編譯成功；發布 2.1.0.9 |
| AutoRetainer | `PunishXIV/AutoRetainer` | `f04642ff` | 2025-12-12 | 已確認 API13 |
| Saucy | `PunishXIV/Saucy` | `8e8d5949` | 2025-08-15 | API13 編譯成功；台服修正 `cycleapple/Saucy@a79b1c5`；發布 1.4.2.8 |
| NoClippy | `UnknownX7/NoClippy` | `d32ae7af` | 2025-08-09 | API13 編譯成功；發布 0.5.0.19 |
| NecroLens | `Jukkales/NecroLens` | `d6646478` | 2025-11-26 | 已確認 API13 |
| GatherBuddy Reborn | `AtmoOmen/GatherBuddyReborn` | `f77e7a44` | 2025-12-16 | 已確認 API13 |
| Artisan | `MeowZWR/Artisan` | `e4a0ddaf` | 2025-12-13 | 已確認 API13；上游已封存 |
| Burning Down the House | `LeonBlade/BDTHPlugin` | `ba39d13c` | 2025-09-30 | 已確認 API13，來源版本為 1.7.1 |
| Raphael.Dalamud | `Dalamud-DailyRoutines/Raphael.Dalamud` | `de11e646` | 2025-09-16 | 待確認產生後 manifest |
| Something Need Doing | `Jaksuhn/SomethingNeedDoing` | `11422e55` | 2025-11-28 | 待確認產生後 manifest |
| TextAdvance | `NightmareXIV/TextAdvance` | `5716d5a4` | 2025-11-22 | 已確認 API13 |
| Lifestream | `NightmareXIV/Lifestream` | `acf27d27` | 2025-12-16 | 已確認 API13 |
| vnavmesh | `awgil/ffxiv_navmesh` | `5f512e57` | 2025-12-15 | API 由建置產生，含原生元件 |
| AutoDuty | `ffxivcode/AutoDuty` | `a7d1eca8` | 2025-12-08 | manifest 使用建置變數，待編譯確認 |
| Pixel Perfect | `Haplo064/PixelPerfect` | `b371fe07` | 2025-08-07 | API13 編譯成功；發布 3.3.2.0 |
| LazyLoot | `PunishXIV/LazyLoot` | `d685ef0c` | 2025-11-19 | manifest 使用建置變數，待編譯確認 |
| YesAlready | `PunishXIV/YesAlready` | `ca2288dd` | 2025-11-10 | 待確認產生後 manifest |
| Price Insight | `Kouzukii/ffxiv-priceinsight` | `3c1c16d7` | 2025-08-07 | API13 編譯成功；發布 2.11.3.0 |
| MidiBard 2 | `midibard.org` | — | — | 閉源／需取得官方 API13 發布包 |
| Questionable | `git.carvel.li/liza/Questionable` | — | — | 待稽核非 GitHub 上游 |
| Gearsetter | `git.carvel.li/liza/Gearsetter` | — | — | 待稽核非 GitHub 上游 |
