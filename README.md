# 图片去背景工具 (Cloudflare Pages 版本)

纯前端实现，直接调用 Remove.bg API，部署到 Cloudflare Pages。

## ✨ 功能

- 🎯 纯前端，无后端
- 💾 不存储图片，全部在内存处理
- 🔑 API Key 本地存储（localStorage）
- 📱 响应式设计
- 🚀 一键部署到 Cloudflare Pages

## 🚀 部署到 Cloudflare Pages

### 方法 1：使用 Wrangler CLI (推荐)

1. 安装 Wrangler：
```bash
npm install -g wrangler
```

2. 登录 Cloudflare：
```bash
wrangler login
```

3. 部署：
```bash
cd bg-remover-cf
wrangler pages deploy . --project-name bg-remover
```

### 方法 2：通过 Cloudflare Dashboard 上传

1. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. 进入 Workers & Pages → Create application → Pages
3. 上传 `bg-remover-cf` 文件夹
4. 等待部署完成

## 📝 使用说明

1. 访问部署后的网站
2. 输入你的 Remove.bg API Key（在 [这里](https://www.remove.bg/dashboard#api-key) 获取）
3. 上传图片
4. 点击"去除背景"
5. 下载结果

## 🎨 本地预览

直接在浏览器中打开 `index.html` 即可预览。

## 🔑 获取 Remove.bg API Key

1. 访问 https://www.remove.bg/dashboard#api-key
2. 注册/登录账号
3. 创建 API Key
4. 免费额度：每月 50 张
