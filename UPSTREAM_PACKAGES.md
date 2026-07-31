# 直接採用上游套件

下列插件直接使用其他來源提供的正式版本。本倉庫只在 `repo.json` 轉載其版本資訊與下載連結，不接管原始碼或二進位檔。

| 插件 | 來源 | 插件倉庫 | 本倉庫規則 |
|---|---|---|---|
| IINACT | `PlusoneChiang/IINACT` | `https://plusonechiang.github.io/IINACT/repo.json` | 不自行 fork、修改、重編、中文化或發布替代 ZIP；只同步該來源的正式 manifest |

## 同步規則

1. 更新前必須讀取外部 `repo.json`，不可自行推算版本或下載網址。
2. `AssemblyVersion`、API 等級、來源、下載連結及圖示必須與外部 manifest 一致。
3. 不得將 `DownloadLinkInstall`、`DownloadLinkTesting` 或 `DownloadLinkUpdate` 改回本倉庫 Release。
4. 不得以本倉庫既有 fork 或歷史 ZIP 覆蓋上游版本。
5. 上游版本若暫時失效，只記錄相容性狀態，不擅自修補後發布。
