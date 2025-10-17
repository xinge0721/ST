# 🎮 酒馆助手 - 游戏状态面板

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![SillyTavern](https://img.shields.io/badge/SillyTavern-Helper-blue)](https://github.com/SillyTavern/SillyTavern)

> 为 SillyTavern（酒馆）提供美观的游戏状态卡片，支持主角、女主、NPC、作品、艺人等多种类型的动态显示。

## ✨ 特性

- 🎨 **美观UI** - 深色游戏风格，金属质感
- 📊 **动态插入** - 支持 0~∞ 个角色/作品/艺人
- 🎯 **自动分组** - 主角、女主、NPC、作品、艺人分类显示
- 🔄 **可折叠** - 点击标题栏折叠/展开，节省空间
- 💾 **状态记忆** - 折叠状态自动保存
- 📱 **响应式** - 自动适配内容高度

## 🚀 快速使用

### 方法1：通过 jsDelivr CDN（推荐）

在酒馆助手的**正则替换**中添加：

**正则表达式（Find）：**
```regex
(?:<主角>[\s\S]*?</主角>\s*)?(?:<女主>[\s\S]*?</女主>\s*)?(?:<NPC>[\s\S]*?</NPC>\s*)?(?:<作品区>[\s\S]*?</作品区>\s*)?(?:<旗下艺人区>[\s\S]*?</旗下艺人区>\s*)?
```

**替换为（Replace）：**
```html
<iframe src="https://cdn.jsdelivr.net/gh/你的用户名/仓库名@main/游戏状态卡片/index.html" style="width:100%;max-width:600px;min-height:150px;height:auto;border:none;margin:5px auto;display:block;" frameborder="0"></iframe>
```

> ⚠️ 记得将 `你的用户名/仓库名` 替换为实际的 GitHub 地址！

### 方法2：通过 GitHub Pages

1. 启用本仓库的 GitHub Pages
2. 使用地址：`https://你的用户名.github.io/仓库名/游戏状态卡片/index.html`

### 方法3：通过 jQuery load

在酒馆助手的**前端界面**中：

```html
<body>
<script>
$("body").load("https://cdn.jsdelivr.net/gh/你的用户名/仓库名@main/游戏状态卡片/index.html")
</script>
</body>
```

## 📝 使用示例

### 主角信息

```
<主角>
<名字>辛格</名字>
<体力>85/150</体力>
<金钱>50000</金钱>
<学识>10级</学识>
<背包>钥匙、药水、宝石</背包>
</主角>
```

### 女主/NPC

```
<女主>
<小红>
<体力>80/100</体力>
<好感度>450/520</好感度>
<当前状态>正在讨论新项目</当前状态>
</小红>
<小美>
<体力>90/100</体力>
<好感度>300/520</好感度>
</小美>
</女主>
```

### 作品

```
<作品区>
<电影《夏日回忆》>
<人气>12000</人气>
<收益>350000</收益>
</电影《夏日回忆》>
</作品区>
```

### 艺人

```
<旗下艺人区>
<女优小樱>
<状态>可用</状态>
<当前活动>拍摄中</当前活动>
</女优小樱>
</旗下艺人区>
```

## 📦 包含的面板

- **游戏状态卡片** - 主推面板，支持所有功能
- **手机状态栏** - 手机风格状态显示
- **聊天消息美化** - 聊天气泡美化
- **界面示例** - 各种界面示例

## 🛠️ 本地开发

```bash
# 克隆仓库
git clone https://github.com/你的用户名/仓库名.git

# 注意：这是编译后的 dist 文件夹
# 源代码需要从原项目编译
```

## 📖 详细文档

- [动态插入完整指南](https://github.com/你的用户名/仓库名/blob/main/动态插入完整指南.md)
- [云端部署教程](https://github.com/你的用户名/仓库名/blob/main/云端部署教程.md)

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

[MIT License](LICENSE)

## 🙏 致谢

- [SillyTavern](https://github.com/SillyTavern/SillyTavern) - 强大的AI聊天前端
- [酒馆助手](https://n0vi028.github.io/JS-Slash-Runner-Doc/) - 扩展框架

---

**作者：** 辛格  
**创建日期：** 2025-10-17  
**最后更新：** 2025-10-17

如有问题，欢迎提 Issue！ 🎉

