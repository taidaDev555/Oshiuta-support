# 支援 / Support / サポート

---

OshiUta 使用 YouTube 的內嵌播放器播放內容，  
**不會下載或儲存任何影片或音訊資料。**  
若因 YouTube 平台的規格變更、權利人設定或地區限制導致無法播放，  
屬於 YouTube 平台的行為，本應用程式無法干預。

## CSV 格式與建立方式

OshiUta 透過 **CSV 檔案** 來管理直播與歌曲資料。  
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

### 如何建立 CSV

- 可使用 **Excel** 或 **Google 試算表** 編輯後，以「CSV UTF-8（逗號分隔）」格式匯出。  
- 也可在 App 中開啟 **「建立 CSV」** 工具（設定 → 建立 CSV），自動產生正確格式。  
- **檔名可自行決定**，例如 `mylist.csv`、`oshi_songs.csv`，  
  App 會自動識別並匯入。  
- **可輸入完整的 YouTube 連結**（如  
  `https://youtu.be/abc123xyz45` 或 `https://www.youtube.com/watch?v=abc123xyz45`），  
  App 會自動擷取影片 ID。


### 🧰 Online CSV Maker

You can also use the online tool to create a CSV file directly in your browser:  
(English / 中文 / 日本語 supported)

[OshiUta CSV Maker (open in new tab)](tools/csv-maker.html){:target="_blank" rel="noopener"}


### 注意事項

- CSV 檔首行必須包含標題列（欄位名稱）。  
- 建議使用 **UTF-8（含 BOM）** 編碼，以確保與 Excel 相容。  
- StartSec / EndSec 為整數（單位：秒）。  
- **EndSec 可留空。**  
  若未填寫，App 將自動套用預設播放時長（例如 600 秒）。

---


OshiUta uses YouTube’s embedded player for playback.  
**It does not download or store any video or audio data.**  
If playback becomes unavailable due to YouTube’s specification changes,  
content owner restrictions, or regional limitations,  
such behavior is controlled by YouTube and beyond the app’s scope.

## CSV Format and How to Create

OshiUta manages stream and song information using a **CSV file**.  
Each line represents one song segment within a YouTube stream.


| Column | Description |
|---------|-------------|
| **StreamDate** | Date of stream (e.g. 2025/10/01) |
| **StreamTitle** | Stream title |
| **Streamer** | Singer / Streamer |
| **VideoId** | YouTube video ID (11 characters) or full URL |
| **Title** | Song title |
| **Artist** | Original artist |
| **StartSec** | Start time in seconds |
| **EndSec** | End time in seconds (**can be left blank**) |

### How to Create

- Use **Excel** or **Google Sheets**, then export as “CSV UTF-8 (comma separated)”.  
- Or use the in-app **CSV Creator** (Settings → Create CSV) to automatically format the file.  
- The **file name can be anything you like** (for example `mylist.csv` or `oshi_songs.csv`).  
  The app will recognize and import it automatically.  
- You may enter a **full YouTube URL** such as  
  `https://youtu.be/abc123xyz45` or `https://www.youtube.com/watch?v=abc123xyz45`;  
  the app automatically extracts the video ID.

### 🧰 Online CSV Maker

You can also use the online tool to create a CSV file directly in your browser:  
(English / 中文 / 日本語 supported)

[OshiUta CSV Maker (open in new tab)](tools/csv-maker.html){:target="_blank" rel="noopener"}

### Notes

- Always include the header row with the column names.  
- Encoding should be **UTF-8 with BOM** (for Excel compatibility).  
- StartSec / EndSec must be integers (seconds).  
- **EndSec can be left empty.**  
  If omitted, the app uses the default playback duration (e.g. 600 seconds).

---


OshiUta は YouTube の埋め込みプレーヤーを利用して再生を行います。  
**動画や音声データをダウンロード・保存することはありません。**  
YouTube 側の仕様変更や権利者の設定、地域制限などにより再生できない場合がありますが、  
それは YouTube プラットフォーム側の挙動であり、本アプリから制御することはできません。

## CSV フォーマットと作成方法

OshiUta は、歌枠や配信アーカイブの情報を **CSV ファイル** で管理します。  
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

### 作成方法

- **Excel** や **Google スプレッドシート** で上記の列を作成し、  
  「CSV UTF-8 (カンマ区切り)」形式で保存します。  
- アプリ内の **「CSV作成ツール」**（設定 → CSV作成）を使うと、  
  入力した日付・タイトル・URL・時刻から自動で整形できます。  
- ファイル名は **任意の名前で構いません**（例：`mylist.csv`、`oshi_songs.csv` など）。  
  アプリでインポート時に自動的に読み込めます。  
- YouTube欄には **フルURL（例：`https://youtu.be/abc123xyz45` や `https://www.youtube.com/watch?v=abc123xyz45`）** を入力しても問題ありません。  
  アプリ側で動画IDを自動抽出します。

### 🧰 Online CSV Maker

You can also use the online tool to create a CSV file directly in your browser:  
(English / 中文 / 日本語 supported)

[OshiUta CSV Maker (open in new tab)](tools/csv-maker.html){:target="_blank" rel="noopener"}

### 注意点

- CSVの最初の行には必ずヘッダ（上記カラム名）を含めてください。  
- 文字コードは **UTF-8（BOM付き）** を推奨します（Excel互換）。  
- StartSec / EndSec は整数（秒単位）で指定してください。  
- **EndSec は空欄でも構いません。**  
  その場合、アプリ設定の「デフォルト再生時間」（例：600秒）が自動的に適用されます。

---

© 2025 taida-agency Development Team. All rights reserved.
