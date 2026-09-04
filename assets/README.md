# 素材放置說明

猜歌題目可無限次播放。播放題目音檔時，網站會同步播放 `../guess/bgm.mp3`；左上角「聲音：開／關」可同時控制題目音檔與 BGM。

請將素材放在以下位置，檔名可在 `script.js` 最上方的 `CONFIG` 設定區修改。網站每次開始挑戰時，會從 `CONFIG.questionBank` 隨機抽出 3 題。

- `../guess/level-1.mp3`：第一關混音
- `../guess/level-2-a.mp3`、`../guess/level-2-b.mp3`：第二關隨機版本
- `../guess/level-3.mp3`：第三關混音
- `../guess/bgm.mp3`：播放題目音檔時同步播放的背景音樂
- `recruitment-qr.svg`：招生表單 QR Code 預留圖，可替換成正式 QR Code

招生表單網址位於 `script.js` 最上方的 `recruitmentConfig.formUrl`。

可選的樂器圖片資料夾：

- `instruments/flute.png`
- `instruments/clarinet.png`
- `instruments/saxophone.png`
- `instruments/trumpet.png`
- `instruments/french-horn.png`
- `instruments/trombone.png`
- `instruments/tuba.png`
- `instruments/percussion.png`

結果頁目前使用 `assets/instruments/` 內的 SVG 樂器插畫；圖片不存在時會退回顯示 emoji。

## 開啟方式

直接雙擊上一層的 `index.html` 即可使用。若瀏覽器限制本機音檔播放，可在「管樂」資料夾開啟終端機後執行：

```text
python -m http.server 8000
```

接著用瀏覽器開啟 `http://localhost:8000`。
