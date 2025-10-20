# 支援 / Support / サポート

---

> **OshiUta** 是一款由個人開發的應用程式，  
> 可透過 YouTube 內嵌播放器播放直播存檔中的特定片段。  
> 本頁說明應用程式的使用方式與 CSV 檔案格式。

---

## 🇹🇼 繁體中文（Traditional Chinese）

### 📘 關於應用程式
OshiUta 使用 YouTube 的內嵌播放器播放內容。  
**不會下載或儲存任何影片或音訊資料。**  
若因 YouTube 規格變更、權利人設定或地區限制導致無法播放，  
屬於 YouTube 平台的行為，本應用程式無法干預。

---

### 📄 CSV 格式與建立方式

OshiUta 透過 **CSV 檔案** 管理直播與歌曲資料。  
每一行代表一首歌曲在直播中的播放區段。

| 欄位名稱 | 說明 |
|-----------|------|
| **StreamDate** | 直播日期（例：2025/10/01） |
| **StreamTitle** | 直播標題 |
| **Streamer** | 主播／歌手名稱 |
| **VideoId** | YouTube 影片 ID（11 字）或完整 URL |
| **Title** | 歌曲名稱 |
| **Artist** | 原唱者／作曲者 |
| **StartSec** | 開始秒數（整數） |
| **EndSec** | 結束秒數（整數，**可留空**） |

#### 🔧 建立方式
- 使用 **Excel** 或 **Google 試算表** 編輯後，以「CSV UTF-8（逗號分隔）」格式匯出。  
- 或在 App 內開啟 **「建立 CSV」** 工具（設定 → 建立 CSV），自動產生正確格式。  
- 檔名可自行決定（如 `mylist.csv`, `oshi_songs.csv`），App 會自動識別。  
- 可輸入完整的 YouTube 連結（例：`https://youtu.be/abc123xyz45`），App 會自動擷取 ID。

#### ⚠️ 注意事項
- 第一行需包含欄位名稱。  
- 建議使用 **UTF-8（含 BOM）** 編碼。  
- StartSec / EndSec 為整數（單位：秒）。  
- **EndSec 可留空。** 未填寫時，App 會自動套用預設播放時長（如 600 秒）。

---

## 🇬🇧 English

### 📘 About the App
OshiUta uses YouTube’s embedded player for playback.  
**It does not download or store any video or audio data.**  
If playback becomes unavailable due to YouTube’s specification changes,  
content owner restrictions, or regional limitations,  
such behavior is controlled by YouTube and beyond the app’s scope.

---

### 📄 CSV Format and How to Create

OshiUta manages stream and song data via **CSV files**.  
Each line represents one song segment within a live stream.

| Column | Description |
|---------|-------------|
| **StreamDate** | Date of stream (e.g. 2025/10/01) |
| **StreamTitle** | Stream title |
| **Streamer** | Streamer / Singer |
| **VideoId** | YouTube video ID (11 chars) or full URL |
| **Title** | Song title |
| **Artist** | Original artist |
| **StartSec** | Start time (seconds) |
| **EndSec** | End time (seconds, *optional*) |

#### 🔧 How to Create
- Use **Excel** or **Google Sheets**, then export as “CSV UTF-8 (comma separated)”.  
- Or use the in-app **CSV Creator** (Settings → Create CSV) for automatic formatting.  
- Any filename is fine (`mylist.csv`, `oshi_songs.csv`).  
- Full YouTube URLs are accepted; the app will extract the video ID automatically.

#### ⚠️ Notes
- Include a header row with the column names.  
- Use **UTF-8 with BOM** for Excel compatibility.  
- `StartSec` / `EndSec` are integers (seconds).  
- If `EndSec` is blank, the app applies the default playback duration (e.g. 600 sec).

---

## 🇯🇵 日本語（Japanese）

### 📘 アプリについて
OshiUta は YouTube の埋め込みプレーヤーを利用して再生を行います。  
**動画や音声データをダウンロード・保存することはありません。**  
YouTube 側の仕様変更や権利者の設定、地域制限などにより再生できない場合がありますが、  
それは YouTube 側の挙動であり、本アプリから制御することはできません。

---

### 📄 CSV フォーマットと作成方法

OshiUta は歌枠や配信アーカイブの情報を **CSV ファイル** で管理します。  
1行が1曲を表し、開始・終了秒数で再生区間を指定します。

| カラム名 | 説明 |
|-----------|------|
| **StreamDate** | 配信日（例：2025/10/01） |
| **StreamTitle** | 配信タイトル |
| **Streamer** | 配信者名／歌い手名 |
| **VideoId** | YouTube の動画ID（11文字）またはURL |
| **Title** | 曲名 |
| **Artist** | 原曲アーティスト名 |
| **StartSec** | 再生開始秒（整数） |
| **EndSec** | 再生終了秒（整数・**空欄でも可**） |

#### 🔧 作成方法
- **Excel** や **Google スプレッドシート** で上記の列を作成し、  
  「CSV UTF-8 (カンマ区切り)」形式で保存します。  
- アプリ内の **「CSV作成ツール」**（設定 → CSV作成）を使うと、  
  入力した日付・タイトル・URL・時刻から自動で整形されます。  
- ファイル名は自由に決めて構いません（例：`mylist.csv`, `oshi_songs.csv`）。  
- YouTube欄には **フルURL** を入れてもOK。アプリが自動で動画IDを抽出します。

#### ⚠️ 注意点
- 1行目は必ずヘッダ（上記カラム名）を含めてください。  
- 文字コードは **UTF-8（BOM付き）** を推奨します。  
- StartSec / EndSec は整数（秒単位）。  
- **EndSec が空欄の場合**、設定の「デフォルト再生時間」が適用されます（例：600秒）。

---

© 2025 taida-agency Development Team.  
All rights reserved.  
[🔗 回首頁 / Back to Home / ホームに戻る](index.md)
