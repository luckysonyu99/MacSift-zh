# MacSift 简体中文版

> Fork 自 [Lcharvol/MacSift](https://github.com/Lcharvol/MacSift)

一款优雅的 macOS 磁盘清理工具，支持简体中文界面。

## ✨ 本 Fork 的改动

- ✅ **简体中文支持** - 完整翻译所有界面文本（165 个字符串）
- ✅ **macOS 15+ 适配** - 支持 macOS 15 (Sequoia) 及更高版本

## 🚀 安装使用

### 方式一：下载预编译版本

1. 前往 [Releases](../../releases) 下载最新版本
2. 解压后将 `MacSift.app` 移动到 `/Applications` 目录
3. 右键点击应用选择"打开"（首次运行需要）
4. 在"系统设置 → 隐私与安全性 → 完全磁盘访问权限"中添加 MacSift

### 方式二：从源码构建

```bash
# 克隆仓库
git clone https://github.com/luckysonyu99/MacSift-zh.git
cd MacSift-zh

# 构建应用
./build-app.sh

# 安装到 Applications
mv MacSift.app /Applications/
```

## 📋 系统要求

- macOS 15 (Sequoia) 或更高版本
- 需要授予"完全磁盘访问权限"

## 🙏 致谢

- 原项目：[Lcharvol/MacSift](https://github.com/Lcharvol/MacSift)
- 中文本地化：通过 [Claude Code](https://claude.ai/code) 和 [Happy](https://happy.engineering) 完成

## 📄 许可证

与原项目保持一致 - 详见 [LICENSE](LICENSE)
