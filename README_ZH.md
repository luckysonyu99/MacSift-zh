# MacSift - 简体中文版

> 基于 [MacSift v0.3.1](https://github.com/Lcharvol/MacSift) 的简体中文本地化版本

## 🎯 改动说明

本版本在原版 MacSift 基础上添加了**简体中文语言支持**，使中文用户能够更方便地使用这款优秀的 macOS 磁盘清理工具。

**注意**：原项目已经支持 macOS 15 (Sequoia)，本 fork 仅添加了中文翻译，未修改任何核心功能。

### ✨ 本 Fork 的改动

- ✅ **完整的简体中文界面**
  - 翻译了所有 165 个界面字符串
  - 包括主界面、设置、菜单、提示信息等
  - 自动跟随系统语言设置

### 📦 原版功能特性

- ✅ **支持 macOS 15 (Sequoia) 及以上**
  - 在 macOS 15 上使用标准材质效果
  - 在 macOS 26 (Tahoe) 上自动启用 Liquid Glass 效果
  - 通过运行时检查实现优雅降级

- ✅ **强大的清理功能**
  - 11 种文件分类扫描
  - 重复文件检测
  - 安全删除（移至废纸篓）
  - 完全透明的操作流程

### 📝 修改的文件

1. **新增文件**
   - `MacSift/Resources/zh-Hans.lproj/Localizable.strings` - 简体中文翻译文件

2. **修改文件**
   - `Package.swift` - 添加中文资源声明
   - `build-app.sh` - 添加中文本地化支持

### 🚀 使用方法

#### 下载预编译版本
从 [Releases](../../releases) 下载最新的 `MacSift.app.zip`，解压后拖入 `/Applications` 文件夹。

#### 从源码编译
```bash
# 克隆仓库
git clone https://github.com/你的用户名/MacSift-zh.git
cd MacSift-zh

# 编译
./build-app.sh

# 运行
open MacSift.app
```

#### 授予权限
首次运行需要授予"完全磁盘访问权限"：
1. 打开 **系统设置** → **隐私与安全性** → **完全磁盘访问权限**
2. 点击 **+** 添加 `MacSift.app`
3. 重启应用

### 🌍 支持的语言

- 🇺🇸 English (英语)
- 🇫🇷 Français (法语)
- 🇨🇳 简体中文 (新增)

应用会自动跟随系统语言。如需强制使用中文：
```bash
defaults write com.macsift.app AppleLanguages '(zh-Hans)'
```

### 📋 系统要求

- macOS 15.0 (Sequoia) 或更高版本
- Apple Silicon 或 Intel 处理器
- Swift 6.0+

### 🎨 功能特性

#### 文件分类
- 📦 **缓存** - 应用缓存文件
- 📝 **日志** - 系统和应用日志
- 🗑️ **临时文件** - /tmp 和临时目录
- 📱 **iOS 备份** - iPhone/iPad 备份
- 💾 **时间机器快照** - 本地 TM 快照
- 🔧 **Xcode 垃圾** - DerivedData、Archives 等
- 📦 **开发缓存** - npm、pip、cargo 等
- 📥 **旧下载** - 90 天以上的下载文件
- 📧 **邮件附件** - Mail.app 下载的附件
- 📊 **大文件** - 超过阈值的大文件
- 🔄 **重复文件** - 内容完全相同的文件

#### 安全特性
- ✅ 默认开启"演练模式"（不实际删除）
- ✅ 所有删除操作移至废纸篓（可恢复）
- ✅ 删除前需要明确确认
- ✅ 超过 10GB 会额外警告
- ✅ 完整的审计日志

### 📸 截图

（可以添加中文界面截图）

### 🙏 致谢

- 原作者：[Lcharvol](https://github.com/Lcharvol)
- 原项目：[MacSift](https://github.com/Lcharvol/MacSift)

### 📄 许可证

MIT License - 与原项目保持一致

### 🔗 相关链接

- [原项目地址](https://github.com/Lcharvol/MacSift)
- [问题反馈](../../issues)
- [发布页面](../../releases)

---

**注意**：本项目仅添加了中文翻译，所有核心功能和代码均来自原项目。如果你觉得这个工具有用，请给原项目一个 ⭐️！
