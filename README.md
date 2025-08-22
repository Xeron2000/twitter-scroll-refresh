# Twitter Scroll Refresh

一个简单易用的用户脚本，通过在Twitter/X顶部向上滚动来快速刷新时间线，并支持快速返回页面顶部。

A simple userscript that allows you to refresh Twitter/X timeline by scrolling up at the top of the page, with quick scroll-to-top functionality.

## ✨ 功能特性 / Features

- 🔄 **智能刷新**: 在页面顶部向上滚动即可刷新时间线
- ⬆️ **快速到顶**: 按住Shift键向上滚动快速返回页面顶部
- 🎯 **精确路径**: 只在主页时间线页面生效，避免误触发
- 🌐 **双语支持**: 支持中文和英文界面
- ⚙️ **可自定义设置**: 调整滚动阈值、冷却时间等参数
- 🔔 **通知提示**: 可选的刷新状态通知
- 🐛 **调试模式**: 开发者友好的调试选项
- 🎯 **多方法兼容**: 支持多种刷新方式，确保在不同情况下都能正常工作

## 📦 安装 / Installation

1. 首先安装用户脚本管理器:
   - [Tampermonkey](https://www.tampermonkey.net/) (推荐)
   - [Greasemonkey](https://www.greasespot.net/)
   - [Violentmonkey](https://violentmonkey.github.io/)

2. 点击下面的链接安装脚本:
   [安装脚本 / Install Script](https://github.com/Xeron2000/twitter-scroll-refresh/raw/refs/heads/main/Twitter%20Scroll%20Refresh-1.4.0.user.js)

## 🚀 使用方法 / Usage

### 刷新时间线 / Refresh Timeline

1. 打开 Twitter/X 网站 (`x.com/home`)
2. 滚动到页面顶部
3. 继续向上滚动即可触发刷新

### 快速返回顶部 / Quick Scroll to Top

1. 在页面任意位置
2. 按住 **Shift** 键
3. 向上滚动鼠标滚轮
4. 即可平滑滚动到页面顶部

就这么简单！脚本会自动检测你的操作并执行相应功能。

## ⚙️ 设置 / Settings

点击用户脚本管理器中的"设置"按钮，或使用快捷菜单来访问设置面板：

### 可配置选项 / Configuration Options

- **滚动阈值** (Scroll Threshold): 触发刷新的滚动敏感度 (默认: 30)
- **刷新冷却时间** (Refresh Cooldown): 两次刷新之间的最小间隔 (默认: 1500ms)
- **顶部偏移量** (Top Offset): 判定"顶部"的像素偏移 (默认: 10px)
- **启用滚轮到顶部** (Enable Scroll to Top): 开启Shift+向上滚轮功能 (默认: 开启)
- **滚轮到顶部冷却时间** (Scroll to Top Cooldown): 两次到顶操作的最小间隔 (默认: 2000ms)
- **显示通知** (Show Notifications): 是否显示刷新状态通知
- **调试模式** (Debug Mode): 开启控制台调试信息
- **语言设置** (Language): 选择界面语言

## 🔧 工作原理 / How It Works

### 刷新功能 / Refresh Functionality

脚本使用多种方法来确保刷新功能的可靠性：

1. **主页标签点击**: 在主页时点击Home标签
2. **刷新按钮检测**: 查找页面上的刷新按钮
3. **键盘快捷键**: 模拟按下'.'键（Twitter的内置快捷键）
4. **新帖子按钮**: 查找并点击"显示新帖子"类型的按钮

### 滚轮到顶部功能 / Scroll to Top Functionality

- **精确路径检测**: 只在 `/home` 和 `/home/` 路径下启用功能
- **Shift键检测**: 监测Shift键按下状态
- **滚轮方向检测**: 只响应向上滚轮操作
- **冷却机制**: 防止频繁触发滚动到顶部
- **平滑滚动**: 使用浏览器的平滑滚动API

### 路径限制 / Path Restriction

脚本只在以下路径生效：
- `https://x.com/home`
- `https://x.com/home/`

在其他页面（如帖子详情、通知、消息等）不会触发任何功能，避免误操作。

## 🐛 问题反馈 / Bug Reports

如果遇到问题，请在 [GitHub Issues](https://github.com/Xeron2000/twitter-scroll-refresh/issues) 中反馈。

## 📝 更新历史 / Changelog

### v1.4.0  
- ✨ 新增 **Shift + 向上滚轮** 快速到顶部功能
- 🎯 改进路径检测，只在主页时间线页面生效
- 🛠️ 简化设置界面，移除复杂的操作方式选择
- 🐛 修复在帖子详情页面误触发的问题
- 📝 更新文档和使用说明

### v1.3.1  
- 🐛 修复累积滚动阈值难以控制的问题
- 🔄 重构滚轮事件处理逻辑

### v1.3.0  
- ✨ 新增滚轮到顶部功能
- 🎯 支持多种操作方式：双击滚轮、Shift+滚轮、长按滚轮
- ⚙️ 新增相关设置选项

### v1.2.1  
- 🌐 完善国际化支持
- 🐛 修复刷新逻辑的兼容性问题

### v1.2.0 
- 🔄 初始版本发布
- ⚙️ 基础刷新功能
- 🌐 双语界面支持

## 📄 许可证 / License

MIT License - 详见 [LICENSE](https://github.com/Xeron2000/twitter-scroll-refresh/blob/main/LICENSE) 文件。
