# 臺灣電腦及資訊服務業營業額 HTML 儀表板

## 檔案

- `index.html`：單頁儀表板，可直接用瀏覽器開啟，也可用本機伺服器開啟。
- `data.csv`：已整理好的資料欄位，可匯入 Google Sheet。

## Google Sheet 介接方式

1. 將 `data.csv` 匯入 Google Sheet。
2. 在 Google Sheet 右上角按「共用」。
3. 將「一般存取權」改為「知道連結的任何人」，權限維持「檢視者」。
4. 儀表板可使用 Google Sheet 的 `gviz` 連結讀取資料。

目前已設定的資料來源：

```text
https://docs.google.com/spreadsheets/d/1fR-Jx86Zs1cDT_WGuwenN-zegntq3jLgmioqzK6Q7qE/gviz/tq?gid=0
```

需要的欄位如下：

```text
year,western_year,period,revenue_100m,yoy_pct,driver,source_note,type
```

`type` 可填：

- `annual`：年度資料
- `quarterly`：季度資料

若 Google Sheet 載入失敗，儀表板會自動保留內建資料，不會空白。
