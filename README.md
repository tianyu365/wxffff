# 🌐 网页嵌入器

一个简单而强大的网页嵌入工具，可以通过URL参数快速嵌入任何网页。

## ✨ 功能特点

- 🚀 **快速嵌入**：通过URL参数直接嵌入网页
- 🔗 **分享链接**：自动生成可分享的嵌入链接
- 📱 **响应式设计**：完美支持桌面端和移动端
- 🎨 **现代UI**：美观的渐变设计和流畅动画
- 🔒 **安全编码**：使用Base64编码保护URL参数
- ⚡ **即开即用**：无需复杂配置，部署即可使用

## 🚀 快速开始

### 1. 部署到GitHub Pages

1. Fork 这个仓库
2. 在仓库设置中启用 GitHub Pages
3. 选择主分支作为源
4. 访问 `https://你的用户名.github.io/仓库名`

### 2. 使用方法

#### 基本使用
1. 访问你的网站首页
2. 在输入框中输入要嵌入的网页URL
3. 点击"嵌入网页"按钮查看效果
4. 点击"生成分享链接"获取可分享的链接

#### URL参数方式
直接访问：`你的域名/?i=编码后的URL`

例如：
```
https://yourusername.github.io/?i=aHR0cHM6Ly9leGFtcGxlLmNvbQ==
```

## 📖 使用示例

### 嵌入网页
```
输入URL: https://www.baidu.com
结果: 网页将在iframe中显示
```

### 生成分享链接
```
原始URL: https://www.github.com
编码后: aHR0cHM6Ly93d3cuZ2l0aHViLmNvbQ==
分享链接: https://yourusername.github.io/?i=aHR0cHM6Ly93d3cuZ2l0aHViLmNvbQ==
```

## 🛠️ 技术实现

### 核心技术
- **HTML5**：语义化标签和现代标准
- **CSS3**：Flexbox布局、渐变背景、动画效果
- **JavaScript**：ES6+语法、URL参数处理、Base64编码
- **GitHub Pages**：静态网站托管

### 关键功能
1. **URL参数解析**：自动检测并解析`?i=`参数
2. **Base64编码/解码**：安全的URL参数处理
3. **URL验证**：确保输入的是有效URL
4. **错误处理**：友好的错误提示和404页面
5. **剪贴板操作**：一键复制分享链接

## 📁 文件结构

```
├── index.html          # 主页面
├── 404.html           # 404错误页面
├── README.md          # 说明文档
└── _config.yml        # Jekyll配置（可选）
```

## 🎨 自定义样式

你可以通过修改CSS来自定义外观：

```css
/* 修改主题色 */
body {
    background: linear-gradient(135deg, #你的颜色1 0%, #你的颜色2 100%);
}

/* 修改按钮样式 */
.btn {
    background: linear-gradient(135deg, #你的颜色1 0%, #你的颜色2 100%);
}
```

## 🔧 高级配置

### 自定义域名
1. 在仓库根目录创建 `CNAME` 文件
2. 在文件中写入你的自定义域名
3. 在域名服务商处配置CNAME记录

### 添加自定义功能
可以在 `index.html` 的JavaScript部分添加更多功能：

```javascript
// 添加自定义处理逻辑
function customHandler(url) {
    // 你的自定义代码
}
```

## 🐛 常见问题

### Q: 某些网站无法嵌入？
A: 这是因为目标网站设置了X-Frame-Options头，禁止被嵌入。这是正常的安全机制。

### Q: 如何支持更多URL格式？
A: 可以修改 `isValidUrl` 函数来支持更多URL格式。

### Q: 如何添加密码保护？
A: 可以在URL参数中添加密码验证逻辑。

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 🤝 贡献

欢迎提交Issue和Pull Request！

## 📞 支持

如有问题，请提交Issue或联系开发者。

---

⭐ 如果这个项目对你有帮助，请给个Star！
