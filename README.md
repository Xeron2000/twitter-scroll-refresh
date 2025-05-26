# Twitter Scroll Refresh

一个简单易用的用户脚本，通过在Twitter/X顶部向上滚动来快速刷新时间线。

A simple userscript that allows you to refresh Twitter/X timeline by scrolling up at the top of the page.

## ✨ 功能特性 / Features

- 🔄 **智能刷新**: 在页面顶部向上滚动即可刷新时间线
- 🌐 **双语支持**: 支持中文和英文界面
- ⚙️ **可自定义设置**: 调整滚动阈值、刷新冷却时间等参数
- 🔔 **通知提示**: 可选的刷新状态通知
- 🐛 **调试模式**: 开发者友好的调试选项
- 🎯 **多方法兼容**: 支持多种刷新方式，确保在不同情况下都能正常工作

## 📦 安装 / Installation

1. 首先安装用户脚本管理器:
   - [Tampermonkey](https://www.tampermonkey.net/) (推荐)
   - [Greasemonkey](https://www.greasespot.net/)
   - [Violentmonkey](https://violentmonkey.github.io/)

2. 点击下面的链接安装脚本:
   [安装脚本 / Install Script](https://github.com/Xeron2000/twitter-scroll-refresh/raw/refs/heads/main/Twitter%20Scroll%20Refresh-1.2.1.user.js)

## 🚀 使用方法 / Usage

1. 打开 Twitter/X 网站
2. 滚动到页面顶部
3. 继续向上滚动即可触发刷新

就这么简单！脚本会自动检测你的操作并刷新时间线。

## ⚙️ 设置 / Settings

点击用户脚本管理器中的"设置"按钮，或使用快捷菜单来访问设置面板：

### 可配置选项 / Configuration Options

- **滚动阈值** (Scroll Threshold): 触发刷新的滚动敏感度 (默认: 30)
- **刷新冷却时间** (Refresh Cooldown): 两次刷新之间的最小间隔 (默认: 1500ms)
- **顶部偏移量** (Top Offset): 判定"顶部"的像素偏移 (默认: 10px)
- **显示通知** (Show Notifications): 是否显示刷新状态通知
- **调试模式** (Debug Mode): 开启控制台调试信息
- **语言设置** (Language): 选择界面语言

## 🔧 工作原理 / How It Works

脚本使用多种方法来确保刷新功能的可靠性：

1. **主页标签点击**: 在主页时点击Home标签
2. **刷新按钮检测**: 查找页面上的刷新按钮
3. **键盘快捷键**: 模拟按下'.'键（Twitter的内置快捷键）
4. **新帖子按钮**: 查找并点击"显示新帖子"类型的按钮

## 🐛 问题反馈 / Bug Reports

如果遇到问题，请在 [GitHub Issues](https://github.com/Xeron2000/twitter-scroll-refresh/issues) 中反馈。

## 📄 许可证 / License

MIT License - 详见 [LICENSE](https://github.com/Xeron2000/twitter-scroll-refresh/blob/main/LICENSE) 文件。
