# Suzy Portfolio

Product Manager & UX/UI Designer portfolio — static HTML website.

## 資料夾結構

```
portfolio/
├── index.html               # 首頁（Hero / About / Work / Skills / Contact）
├── css/
│   └── style.css            # 所有頁面共用樣式
├── js/
│   └── main.js              # （選用）互動效果
├── images/
│   ├── projects/            # 各專案截圖，命名規則：project-1-cover.jpg
│   └── about/               # 個人照片等
└── work/
    ├── project-template.html  # 複製這個來新增專案
    ├── project-1.html
    ├── project-2.html
    └── ...
```

## 新增專案頁面

1. 複製 `work/project-template.html` → 重新命名（例：`work/project-5.html`）
2. 填入專案標題、描述、角色、時間等資訊
3. 把截圖放進 `images/projects/`
4. 把 `<img>` 的 `src` 換成正確路徑（注意是 `../images/projects/xxx.jpg`）
5. 在 `index.html` 的 Work 區新增對應卡片，`href` 指向新頁面

## 推上 GitHub Pages

```bash
git init
git add .
git commit -m "init portfolio"
git branch -M main
git remote add origin https://github.com/你的帳號/portfolio.git
git push -u origin main
```

然後在 GitHub repo → Settings → Pages → Branch: main → Save，
幾分鐘後就會有 `https://你的帳號.github.io/portfolio/` 可以分享。
