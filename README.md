# 結晶生成與最佳化 V0.51

更新時間：2026/10/03 17:03（台灣時間）

## 使用方式

1. 開啟 `index.html`，設定等級、武器與戒指。
2. 切換至「傳說結晶生成」，選擇42～60顆與最多三排指定詞條。
3. 勾選1～24顆，按「儲存勾選並前往最佳化」。
4. 第一頁會自動載入勾選結晶，不足24顆的欄位留空；按「進行計算」選出最多12顆。

第一頁的裝備設定會保留。原有儲存／載入、JSON匯出／匯入也可使用。「載入生成結晶」可再次載入最後一次傳送的勾選內容。兩頁需在同一網站、同一瀏覽器中開啟，才能共用儲存資料。

## 詞條範圍

| 詞條 | 範圍 | 間隔 |
|---|---|---|
| 魔力 | 200～400 | 10 |
| 魔攻% | 3～5% | 1% |
| 爆擊機率 | 14～16% | 1% |
| 爆擊傷害 | 10～14% | 1% |
| 冷卻時間減免 | 固定2秒 | — |
| 熟練度 | 7～11% | 1% |
| 最大HP | 300～500 | 1 |
| 最大HP% | 5～8% | 1% |

舊資料的1秒冷卻詞條會轉為2秒；其餘不符合範圍的資料會顯示錯誤，不會直接改值。各詞條的生成機率與原檔相同。計算公式、冷卻轉換倍率、等差減傷及106萬／140萬判定均沿用原檔。

## 上傳到 GitHub Pages

1. 解壓縮ZIP，把 `index.html`、`generator.html`、`.nojekyll`、`README.md` 放到儲存庫最外層。不要上傳ZIP本身，也不要把整個資料夾再套一層。
2. 在該儲存庫開啟 **Settings → Pages**。
3. **Source** 選 **Deploy from a branch**，分支選 **main**，資料夾選 **/(root)**，按 **Save**。若儲存庫使用其他分支名稱，選實際存放檔案的分支。
4. 等GitHub完成發布，再開啟Pages顯示的網站網址。

純HTML，不需要安裝套件或執行建置。每個HTML也可單獨開啟；本機檔案網址下的跨頁儲存取決於瀏覽器，GitHub Pages上則使用同一網站的儲存空間。

GitHub官方說明：
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
