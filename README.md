海報參考模板
========================

## 安裝

1. 欲使用此 R Markdown 模板需先安裝 [`pagedown`](https://github.com/rstudio/pagedown) 套件：

    ```r
    install.packages("pagedown")
    ```

2. 此外，欲輸出 PDF 檔，電腦上需有 chrome 瀏覽器


## 將海報輸出成 HTML 與 PDF

此 repo 有兩種海報的模板，分別在 `template1/` 與 `template2/` 裡。

將工作目錄設在模板的資料夾後 (`template1/` 或 `template2`)，即可透過下方指令輸出 PDF (以 `template1` 為例)：

```r
# 輸出成 template1.html, 可以使用 RStudio knit button 取代
rmarkdown::render("template1.Rmd")

# 透過 chrome 將 template1.html 輸出成 template1.pdf
pagedown::chrome_print("template1.html")
```

## 模板說明

- [點此](https://pagedown.rbind.io/poster-relaxed)看 `template1` 的輸出樣式 (可用 chrome 儲存成 PDF)
- [點此](https://pagedown.rbind.io/poster-jacobs)看 `template2` 的輸出樣式 (可用 chrome 儲存成 PDF)

關於模板的詳細說明，請閱讀 `pagedown` [說明文件](https://pagedown.rbind.io/)或套件 [GitHub 頁面](https://github.com/rstudio/pagedown)。
