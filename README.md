# KMusic 🎵

一款基于 SwiftUI 开发的多源音乐聚合播放器，支持 iOS/macOS 平台。

![Swift](https://img.shields.io/badge/Swift-5.9-orange.svg)
![Platform](https://img.shields.io/badge/Platform-iOS%2015.0%2B%20%7C%20macOS%2012.0%2B-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ 功能特性

- 🎧 **多音源支持** - 内置酷我、酷狗、QQ音乐、网易云、咪咕等主流音乐平台
- 📜 **歌词同步** - 支持 LRC 歌词解析与实时滚动显示
- 🔌 **自定义源** - 支持通过 URL/本地文件导入第三方 JS 脚本扩展音源
- 🔍 **全局搜索** - 跨平台搜索歌曲
- 📱 **后台播放** - 支持后台持续播放音乐
- 🎨 **深色主题** - 精心设计的深色 UI，支持毛玻璃效果

## 📸 截图

| 发现页 | 播放器 | 搜索 |
|:---:|:---:|:---:|
| 歌单广场 | 歌词同步 | 多源搜索 |

## 🏗 项目结构

```
KMusic/
├── Core/
│   ├── API/              # 各平台 API 服务
│   ├── Engine/           # JS 引擎 & 音源管理
│   ├── Models/           # 数据模型
│   └── Player/           # 音频播放器
└── UI/
    ├── Home/             # 首页歌单
    ├── Search/           # 搜索页
    ├── Player/           # 播放器界面
    └── Settings/         # 设置页
```

## 🚀 快速开始

### 环境要求

- Xcode 15.0+
- iOS 15.0+ / macOS 12.0+
- Swift 5.9+

### 安装运行

1. 克隆项目
```bash
git clone https://github.com/Mac-XK/KMusic.git
cd KMusic
```

2. 打开 Xcode 项目
```bash
open KMusic.xcodeproj
```

3. 选择目标设备，点击运行

## 🔧 自定义音源

KMusic 支持导入兼容 [lx-music](https://github.com/lyswhut/lx-music-desktop) 格式的自定义音源脚本。

### 导入方式

1. **URL 导入** - 在设置 → 自定义源管理中输入脚本 URL（支持 GitHub/Gitee/GitLab 链接自动转换）
2. **本地导入** - 选择本地 `.js` 脚本文件导入

### 脚本格式

脚本需包含以下元信息：
```javascript
// @name        音源名称
// @version     1.0.0
```

## 📝 技术实现

- **SwiftUI** - 声明式 UI 框架
- **AVFoundation** - 音频播放
- **JavaScriptCore** - JS 脚本引擎
- **Combine** - 响应式编程
- **URLSession** - 网络请求

## 📄 开源协议

本项目基于 [MIT License](LICENSE) 开源。

## ⚠️ 免责声明

本项目仅供学习交流使用，请勿用于商业用途。音乐版权归原作者所有。

---

如果觉得这个项目对你有帮助，欢迎 ⭐️ Star 支持！
