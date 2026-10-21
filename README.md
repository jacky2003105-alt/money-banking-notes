# 貨幣銀行學筆記

七章課程筆記與 135 題課本習題及參考解答。白板指定的 48 題以 ★ 標示，排在各章習題最前面並保留原題號。入口為 `index.html`。

保留功能：章節下拉切換、跨章頁面連結、習題答案顯示／隱藏、原始簡報圖片放大、經濟學重繪圖、整章與整份習題 PDF 下載、手機版閱讀。這是純靜態網站，不必安裝 Node.js、設定資料庫或執行建置指令。

## 用 GitHub Desktop 上傳（建議）

1. 在 GitHub 登入後建立新儲存庫，例如 `money-banking-notes`。使用免費帳號部署 Pages 時選 **Public**，勾選 **Add a README file** 後建立。Public 代表儲存庫內容及網站將公開。
2. 安裝並登入 [GitHub Desktop](https://desktop.github.com/)。選 **File → Clone Repository**，選取剛建立的儲存庫，再選本機儲存位置。
3. 將本資料夾「裡面」的檔案複製到剛下載的儲存庫根目錄。確認打開儲存庫第一層就看得到 `index.html`，而不是外面再包一層 `money-banking-notes`。需一併放入 `exercises.html`、`assets`、`pdf`、本 README 及 `.nojekyll`。Mac Finder 可按 **Command＋Shift＋.** 顯示 `.nojekyll` 隱藏檔。
4. 回 GitHub Desktop，於 Summary 輸入「加入貨幣銀行學筆記」，按 **Commit to main**，再按 **Push origin**。
5. 回 GitHub 儲存庫的 **Settings → Pages**。在 **Build and deployment** 下，Source 選 **Deploy from a branch**，Branch 選 **main**，資料夾選 **/(root)**，按 **Save**。
6. 等部署完成，Pages 設定頁會提供 **Visit site**。網址通常是 `https://你的帳號.github.io/money-banking-notes/`。請開這個網站網址閱讀，不是儲存庫的檔案預覽頁。

## 檔案擺放

```text
儲存庫根目錄/
├── index.html
├── exercises.html
├── .nojekyll
├── README.md
├── assets/
│   ├── slides/
│   └── diagrams/
└── pdf/
    ├── chapter-01.pdf
    ├── chapter-02.pdf
    ├── chapter-03.pdf
    ├── chapter-04.pdf
    ├── chapter-05.pdf
    ├── chapter-06.pdf
    ├── chapter-08.pdf
    └── exercises.pdf
```

不要把 ZIP 壓縮檔直接上傳當成網站。必須先解壓縮並上傳裡面的檔案，也不要只上傳 index.html。

若偏好 GitHub 網頁上傳，官方上限為每次 100 個檔案、單一檔案 25 MiB。本網站圖片超過 100 張，因此需要分批並保持資料夾路徑。使用 GitHub Desktop 可避免逐批處理。此包所有單一檔案均小於 25 MiB。

## 更新與檢查

日後更新時，用新版本覆蓋儲存庫中對應檔案，完成 Commit 與 Push 即可重新部署。保留目前的相對路徑，不要把 assets 或 pdf 移到別處。

上線後切換每個章節，開啟習題，測試隱藏／顯示答案及 PDF 下載。若圖片或 PDF 出現 404，先檢查是否漏傳資料夾或多包了一層目錄。若首頁 404，檢查 index.html 是否在 main 的根目錄，並查看 Actions 中 Pages 的部署結果。

## 官方說明

- [從 GitHub Desktop 複製儲存庫](https://docs.github.com/en/desktop/adding-and-cloning-repositories/cloning-and-forking-repositories-from-github-desktop)
- [GitHub Desktop 提交與推送](https://docs.github.com/en/desktop/overview/creating-your-first-repository-using-github-desktop)
- [GitHub Pages 來源設定](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [GitHub Pages 入口檔案](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [上傳檔案限制](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
