# Class 1 座位抽籤器

純 HTML / CSS / JavaScript 的座位抽籤器，不需要安裝套件。

## 使用方式

直接雙擊 `index.html` 即可開啟；若瀏覽器限制本機檔案，也可在此資料夾執行簡易伺服器：

```bash
python -m http.server 5173
```

再開啟 <http://localhost:5173>。

## 功能

- 設定座位排數、每排座位數與座號起訖範圍。
- 拖曳座號到座位；已指定座號可用座位上的 `×` 移回清單。
- 「全部隨機」會把尚未指定的座號依序滑入隨機空位。
- 未選取的座號雙擊後可選擇「其他」或「是的，已休學」，放入暫存角落；雙擊角落座號可恢復。
- 座位雙擊可淡化 / 恢復；淡化後不可放入座號。
- 每排座位中間的 `↔` 間隔可左右拖曳調整。
- 右上角可縮放座位表。

## Vercel

將 `class1` 資料夾推送到 GitHub 後，在 Vercel 匯入該 repository，Framework Preset 選 **Other**，Build Command 留空，Output Directory 使用 `.` 即可。