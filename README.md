# 🛍️ Mino Platform 小程序

**一个轻量、精致的社交电商平台——让每一次购物都成为愉悦的发现之旅。**

---

## ✨ 核心愿景

Mino Platform 致力于连接品味相投、热爱生活和分享的人们，将购物从单纯的交易转变为充满灵感与联结的体验。

---

## 🖼️ 核心功能 - 画册模块

### 创意表达与分享
- **智能画册编辑器** – 简单易用的拖拽式编辑器，轻松创建精美画册，展示商品搭配和生活灵感
- **丰富模板库** – 涵盖穿搭、家居、旅行等多种场景的专业模板
- **社交化创作** – 邀请微信好友共同编辑画册，实时协作，共同创作
- **便捷分享** – 一键分享画册到微信聊天，生成精美海报，嵌入个人主页
- **电商无缝连接** – 画册中的商品可直接关联平台商品，支持一键购买画册推荐商品

---

## 🛠️ 技术架构

### 核心技术栈
- **微信小程序原生框架** (WXML + WXSS + JavaScript/TypeScript)
- **微信云开发** (云函数、云数据库、云存储)
- **Canvas API** (画册编辑器核心)
- **微信开放能力** (登录、分享、打印等)

---

## 📁 项目结构

```
mino-platform-miniprogram/
├── miniprogram/                    # 小程序主包
│   ├── pages/                     # 页面文件
│   │   ├── index/                 # 首页
│   │   └── album/                 # 画册模块
│   │       ├── album-home/        # 画册首页
│   │       ├── album-editor/      # 画册编辑器
│   │       ├── template-center/   # 模板中心
│   │       ├── my-albums/         # 我的画册
│   │       └── album-preview/     # 画册预览
│   ├── components/                # 公共组件
│   │   └── album-editor/          # 画册编辑器组件
│   ├── utils/                     # 工具函数
│   └── app.js                     # 小程序入口
├── cloudfunctions/                # 云函数
│   └── album/                     # 画册相关云函数
└── project.config.json            # 项目配置
```

---

## 🚦 快速开始

### 环境要求
- 微信开发者工具（最新版）
- 微信小程序AppID

### 初始化步骤

1. **项目初始化**
```bash
# 克隆项目
git clone <repository-url>
cd mino-platform-miniprogram
```

2. **云开发环境配置**
```javascript
// app.js 配置云环境
App({
  onLaunch: function () {
    wx.cloud.init({
      env: 'your-cloud-env-id',
      traceUser: true,
    })
  }
})
```

3. **开发与调试**
- 在微信开发者工具中导入项目
- 配置云环境ID
- 部署云函数
- 运行调试

*Mino Platform —— 从用画册记录生活，发现美好开始。🛍️🖼️*