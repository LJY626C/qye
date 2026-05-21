# 智能企业建站系统

一个基于Tauri 2.0的智能企业建站桌面应用，支持创建工业制造、科技互联网、商贸服务三种类型的企业网站。

## 功能特性

- 🔐 密码登录 (默认密码: 123456)
- 🏢 企业信息填写 (公司名称、简介、联系方式、Logo、轮播图)
- 📋 行业选择 (工业制造、科技互联网、商贸服务)
- 🎨 模板选择 (每个行业提供3种精美模板)
- 👀 实时预览 (支持PC端和移动端预览)
- 💾 网站导出 (ZIP格式打包下载)
- 📱 响应式设计

## 技术栈

- **前端**: HTML + Tailwind CSS + Vanilla JavaScript
- **桌面框架**: Tauri 2.0
- **打包工具**: Vite
- **ZIP生成**: JSZip

## 项目结构

```
/workspace/
├── index.html          # 主应用入口
├── package.json        # 项目配置
├── vite.config.js      # Vite配置
├── README.md          # 项目说明
└── src-tauri/         # Tauri Rust后端
    ├── Cargo.toml
    ├── tauri.conf.json
    └── src/
        └── main.rs
```

## 快速开始

### 前置要求

1. 安装 [Node.js](https://nodejs.org/) (16+ 版本)
2. 安装 [Rust](https://www.rust-lang.org/tools/install)
3. 安装 Tauri CLI:
```bash
npm install -g @tauri-apps/cli@2.0.0
```

### 安装依赖

```bash
npm install
```

### 开发模式

```bash
npm run tauri dev
```

### 构建生产版本

```bash
npm run tauri build
```

## 使用说明

1. **登录系统**
   - 输入密码 `123456` 登录

2. **创建新网站**
   - 点击"创建新网站"按钮
   - 填写企业信息
   - 选择行业
   - 选择模板
   - 生成网站

3. **预览与导出**
   - 在预览页面可以切换PC/移动端预览
   - 点击"导出网站"按钮下载ZIP文件

## 默认模板

项目包含3个行业的基础模板：
- **工业制造** - 蓝色主题
- **科技互联网** - 紫色主题  
- **商贸服务** - 绿色主题

## 数据存储

- 所有网站数据存储在浏览器的 localStorage 中
- 导出的网站为纯静态HTML文件，可直接部署到任何Web服务器

## 注意事项

- 这是一个单页面应用，所有逻辑在前端实现
- Tauri框架用于提供桌面应用体验
- 如需集成真实的文件系统API，请参考Tauri文档

## 许可证

MIT
