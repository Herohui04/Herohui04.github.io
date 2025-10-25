# 个人静态网站

基于 GitHub Pages 的现代化个人网站，采用纯 HTML、CSS 和 JavaScript 构建。

## ✨ 特性

- 🎨 **现代化设计** - 简洁美观的界面设计
- 📱 **完全响应式** - 适配所有设备尺寸
- ⚡ **高性能** - 纯静态文件，加载速度快
- 🎯 **SEO 友好** - 优化的搜索引擎支持
- 🌙 **主题切换** - 支持明暗主题
- 📧 **联系表单** - 内置联系表单功能
- 🚀 **自动部署** - GitHub Actions 自动部署

## 🚀 快速开始

### 1. Fork 或克隆仓库

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

### 2. 自定义内容

编辑以下文件来自定义您的网站：

- `index.html` - 修改网站内容和结构
- `styles.css` - 调整样式和主题
- `script.js` - 添加交互功能
- `_config.yml` - 配置网站基本信息

### 3. 部署到 GitHub Pages

#### 方法一：使用 GitHub Actions（推荐）

1. 将代码推送到 GitHub 仓库
2. 在仓库设置中启用 GitHub Pages
3. 选择 "GitHub Actions" 作为源
4. 工作流会自动部署您的网站

#### 方法二：手动部署

1. 安装 gh-pages：
```bash
npm install -g gh-pages
```

2. 部署到 GitHub Pages：
```bash
gh-pages -d .
```

## 🔧 部署故障排除

### 常见问题

#### 1. 依赖锁定文件错误
如果遇到 "Dependencies lock file is not found" 错误：

- 确保使用最新的工作流文件
- 检查 `.github/workflows/deploy.yml` 是否正确配置
- 如果问题持续，可以使用 `simple-deploy.yml` 作为备用方案

#### 2. GitHub Pages 权限问题
如果遇到权限错误：

1. 进入仓库设置 → Actions → General
2. 在 "Workflow permissions" 部分选择 "Read and write permissions"
3. 勾选 "Allow GitHub Actions to create and approve pull requests"

#### 3. 部署失败
如果部署失败：

1. 检查 Actions 日志中的具体错误信息
2. 确保所有必需文件（index.html, styles.css, script.js）都存在
3. 验证文件路径和名称是否正确

### 备用部署方案

如果主要工作流有问题，可以：

1. 删除 `.github/workflows/deploy.yml`
2. 重命名 `simple-deploy.yml` 为 `deploy.yml`
3. 重新推送代码

## 📁 项目结构

```
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # JavaScript 功能
├── _config.yml         # Jekyll 配置
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions 工作流
└── README.md           # 项目说明
```

## 🎨 自定义指南

### 修改个人信息

1. **网站标题和描述**：编辑 `index.html` 中的 `<title>` 和 `<meta name="description">`
2. **个人介绍**：修改 `#about` 部分的内容
3. **项目展示**：更新 `#projects` 部分的项目信息
4. **联系信息**：修改 `#contact` 部分的联系方式

### 样式定制

在 `styles.css` 中修改 CSS 变量来自定义主题：

```css
:root {
    --primary-color: #2563eb;    /* 主色调 */
    --secondary-color: #64748b;  /* 次要色调 */
    --accent-color: #f59e0b;     /* 强调色 */
    /* 更多变量... */
}
```

### 添加新功能

在 `script.js` 中添加新的 JavaScript 功能：

```javascript
// 添加新的交互功能
function yourNewFunction() {
    // 您的代码
}
```

## 📱 响应式设计

网站采用移动优先的响应式设计：

- **桌面端**：完整的多列布局
- **平板端**：适配中等屏幕
- **移动端**：单列布局，优化的触摸体验

## 🔧 技术栈

- **HTML5** - 语义化标记
- **CSS3** - 现代样式特性
- **JavaScript ES6+** - 现代 JavaScript
- **GitHub Pages** - 免费托管
- **GitHub Actions** - 自动部署

## 📈 性能优化

- ✅ 纯静态文件，无服务器依赖
- ✅ 优化的图片加载
- ✅ 最小化 CSS 和 JavaScript
- ✅ 浏览器缓存优化
- ✅ 懒加载支持

## 🛠️ 开发工具

### 本地开发

使用简单的 HTTP 服务器进行本地开发：

```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js
npx serve .

# 使用 Live Server (VS Code 扩展)
# 右键 index.html -> Open with Live Server
```

### 代码格式化

推荐使用 Prettier 进行代码格式化：

```bash
npm install -g prettier
prettier --write "*.{html,css,js}"
```

## 📝 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开 Pull Request

## 📞 支持

如果您遇到任何问题或有建议，请：

- 提交 [Issue](https://github.com/yourusername/your-repo-name/issues)
- 发送邮件至 your.email@example.com
- 在 [Discussions](https://github.com/yourusername/your-repo-name/discussions) 中讨论

## 🙏 致谢

- 感谢 [GitHub Pages](https://pages.github.com/) 提供免费托管
- 感谢 [GitHub Actions](https://github.com/features/actions) 提供自动部署
- 感谢所有开源贡献者

---

⭐ 如果这个项目对您有帮助，请给它一个星标！
