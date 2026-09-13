# My Projects

项目代码仓库。静态页面通过 GitHub Pages 自动部署。

## 在线访问

部署完成后：

```
https://<你的用户名>.github.io/my-projects/
```

## 目录约定

```
my-projects/
├── index.html              # 站点首页（Pages 入口）
├── <子项目名>/             # 任意子目录，自动可通过 /<子项目名>/ 访问
└── .github/workflows/      # 自动部署配置，一般不用改
```

## 本地预览

```bash
python -m http.server 8000
# 浏览器打开 http://localhost:8000
```

## 发布流程

```bash
git add .
git commit -m "更新内容"
git push
```

push 到 `main` 分支后，GitHub Actions 自动构建并发布，约 30-60 秒生效。

> 页面未更新时先按 `Ctrl + F5` 强制刷新，排除浏览器缓存。

## 启用 Pages（首次）

仓库 → Settings → Pages → Source 选择 **GitHub Actions**。
