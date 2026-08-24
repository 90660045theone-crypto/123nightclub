# 123 NIGHT CLUB 官網・GitHub Pages 部署步驟

**對應網站版本 v6.4.6｜2026-08-24｜熱灣行銷**
照著點就好，全程免費、不用寫任何程式。

## 一、建儲存庫（做一次）

1. 登入 github.com → 右上角「＋」→ **New repository**。
2. Repository name 建議填：**你的帳號.github.io**（例：帳號是 `rewan123` 就填 `rewan123.github.io`）——這樣網址最短最乾淨：`https://rewan123.github.io/`。
   （若這名字被用過，就填 `123nightclub`，網址會變成 `https://帳號.github.io/123nightclub/`，一樣能用。）
3. 選 **Public**（免費版 Pages 必須公開）→ 按 **Create repository**。

## 二、上傳網站檔案

1. 在新儲存庫頁面點 **uploading an existing file**（或 Add file → Upload files）。
2. 把部署包解壓縮後的東西**全部拖進去**：四個 `.html`、整個 `videos/` 資料夾（用 Chrome 拖資料夾會保留結構）、`.nojekyll`、兩份說明檔。
   - `.nojekyll` 是隱藏檔，解壓後看不到它也沒關係，漏掉網站一樣會動。
   - 確認上傳清單裡看得到 `videos/intro.mp4`、`videos/intro.webm`、`videos/intro_logo.webp` 三個。
3. 下方 Commit changes 按鈕按下去。

## 三、開啟 Pages

1. 儲存庫上方 **Settings** → 左邊選單 **Pages**。
2. Source 選 **Deploy from a branch**；Branch 選 **main**、資料夾選 **/(root)** → **Save**。
3. 等 1–3 分鐘，同一頁上方會出現你的網址（例：`https://rewan123.github.io/`）。
   （若用 `你的帳號.github.io` 當儲存庫名，這步通常自動就開好了。）

## 四、上線測試（手機開網址）

1. 開 `https://你的網址/?qr=1` → 年齡門 → 點「是」→ 過場動畫 → 落首頁。✔
2. 再開一次同網址 → 不重播、不再問 18 歲。✔
3. 右上角切日文／EN 正常。✔

## 五、測完把網址傳給 Claude

拿到網址後把它貼回對話，Claude 會：
1. 產出店內用 **QR code 圖檔**（內容＝你的網址＋`?qr=1`）。
2. 之後每次改版，你只要把新檔案用同樣方式上傳覆蓋（Upload files → 拖進去 → Commit），一分鐘內全站更新，網址永遠不變。

## 六、之後想換自己的網域（選配、不急）

買好網域後：Settings → Pages → Custom domain 填網域，再到網域商後台加一筆 CNAME 指向 `你的帳號.github.io`。QR code 到時重產一張即可。
