# newimages

kui.name 新聞 AI 生成配圖 (webp)。由 kui_img_github.py 自動推送。

## 容量與限制

實測 2026-11-23：521 個檔 / 29.9 MiB（244 則新聞的 hero 1024w + 縮圖 320w，另 32 張原文圖）。
GitHub 側 packed size 28.6 MB。每則新聞含 git 歷史約佔 250 KB。

| 項目 | GitHub 限制 |
|---|---|
| 單檔 (git push) | >50 MiB 警告，>100 MiB 拒收 |
| 單檔 (網頁上傳) | 25 MiB |
| Repo 大小 | 建議 <1 GB；<5 GB 強烈建議 |
| Git LFS 單檔 | 2 GB (Free/Pro)、4 GB (Team)、5 GB (Enterprise) |
| Release 附件 | 單檔 <2 GiB，每個 release 最多 1000 個 |
| GitHub Pages | 站台 1 GB、流量 100 GB/月 (軟限)、10 builds/小時 |
| REST API | 未認證 60 次/小時、已認證 5000 次/小時 |
| 帶寬 | 冇公開上限；AUP §9 保留 throttle file hosting / 停權 |

圖片 1 GB 大約等於 4,000 則新聞（每則 250 KB 含歷史）。
依現時出圖速度，1 GB 約 3–5 星期到達，所以呢個 repo 唔係長期圖床。

來源：
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github
- https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage
- https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
- https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases
- https://docs.github.com/en/rest/using-the-rest-api/rate-limits-for-the-rest-api
- https://docs.github.com/en/site-policy/acceptable-use-policies/github-acceptable-use-policies
