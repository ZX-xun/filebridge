# Filebridge

[English](#english) | [中文](#中文)

---

## 中文

### 这是什么？

**让 AI 帮你操作另一台电脑上的文件。**

你的 AI 在这台电脑，要处理的文件在另一台电脑？  
那台电脑太老装不了 AI，或者不让随便装软件？

Filebridge 解决这个问题：在那台电脑上运行这个小工具，你就能在这台电脑上用 AI 读写它的文件了。

**举个例子：**
- 你在笔记本上用 Claude，想让它帮你整理服务器上的日志文件
- 你的台式机有 AI，想让它批量修改另一台老电脑上的文档
- 公司电脑不让装 AI，但你想用自己电脑的 AI 帮它处理文件

**一句话：** 让装了 AI 的电脑，能操作没装 AI 的电脑上的文件。

**能做什么：**
- 📖 让 AI 读取远程电脑的文件（代码、日志、文档等）
- ✏️让 AI 修改远程电脑的文件（可选，需要明确开启）
- 🔒 只开放你指定的文件夹，其他地方 AI 访问不到
- 🔐 用临时密码保护，用完就关

### 当前版本

**v0.0.1** — 早期测试版本

⚠️ 建议仅共享专门用于开发或测试的目录，不要直接共享系统盘或包含敏感信息的目录。

### 下载安装

进入右侧 **[Releases](../../releases)** 页面，根据目标电脑的系统和架构下载对应的安装包：

| 平台 | 架构 | 适用设备 |
|------|------|----------|
| Windows | x64 | Intel/AMD 处理器的 Windows 电脑 |
| Windows | ARM64 | ARM 架构的 Windows 设备 |
| Linux | x64 | Intel/AMD 处理器的 Linux 系统 |
| Linux | ARM64 | ARM 架构的 Linux 设备（如树莓派） |

**注意：** 请下载 Assets 中以 `filebridge-0.0.1` 开头的安装包，不要下载 GitHub 自动生成的 `Source code.zip`。

### 使用指南

#### Windows

1. 下载对应架构的 `.zip` 安装包
2. 解压到任意目录
3. 双击运行 `启动.bat`
4. 在控制台中选择要共享的目录
5. 选择访问权限（只读/读写）
6. 将显示的**端点地址**和 **Token** 提供给 AI 助手
7. 保持控制台窗口运行（关闭窗口即停止服务）

#### Linux

1. 下载对应架构的 `.tar.gz` 安装包
2. 解压：`tar -xzf filebridge-*.tar.gz`
3. 运行：`./启动.sh` 或 `bash 启动.sh`
4. 按照提示选择共享目录和权限
5. 将显示的**端点地址**和 **Token** 提供给 AI 助手
6. 保持终端运行（`Ctrl+C` 停止服务）

### 安全建议

🔒 **请务必遵守以下安全规则：**

- ❌ **不要**将 Token 发布在 Issue、公开聊天或截图中
- ❌ **不要**共享系统目录（如 `C:\Windows`、`/etc`、`/usr` 等）
- ❌ **不要**共享包含密码、密钥、证书的目录
- ❌ **不要**向不可信的 AI 开启读写或命令执行权限
- ✅ **优先使用只读模式**
- ✅ **仅共享专门的工作目录或测试目录**
- ✅ **使用完毕后及时关闭服务**

### 问题反馈

遇到问题？请在 [Issues](../../issues) 页面提交，并提供以下信息：

- Filebridge 版本号
- 操作系统及版本
- CPU 架构（x64/ARM64）
- 使用的协议（REST/MCP）
- 完整的错误信息
- 问题复现步骤

⚠️ **提交前请删除所有敏感信息：** Token、个人目录路径、IP 地址、用户名等。

### 许可证

MIT License

---

## English

### What is this?

**Let AI access and edit files on another computer.**

Your AI is on this computer, but the files are on another one?  
That computer is too old to run AI, or you're not allowed to install software there?

Filebridge solves this: run this small tool on that computer, and you can use AI on this computer to read/write its files.

**Examples:**
- You use Claude on your laptop, want it to help organize log files on your server
- Your desktop has AI, want it to batch-edit documents on another old computer
- Your work computer doesn't allow AI installation, but you want to use your personal computer's AI to process its files

**In short:** Let the computer with AI operate files on the computer without AI.

**What it can do:**
- 📖 Let AI read files on a remote computer (code, logs, documents, etc.)
- ✏️ Let AI modify files on a remote computer (optional, must be explicitly enabled)
- 🔒 Only expose folders you specify, AI can't access anywhere else
- 🔐 Protected by temporary password, close it when done

### Current Version

**v0.0.1** — Early Testing Release

⚠️ It's recommended to only share directories specifically prepared for development or testing, not system drives or sensitive data folders.

### Download & Installation

Visit the **[Releases](../../releases)** page on the right, and download the appropriate package for your system:

| Platform | Architecture | Target Device |
|----------|--------------|---------------|
| Windows | x64 | Intel/AMD Windows PCs |
| Windows | ARM64 | ARM-based Windows devices |
| Linux | x64 | Intel/AMD Linux systems |
| Linux | ARM64 | ARM-based Linux devices (e.g., Raspberry Pi) |

**Note:** Download packages starting with `filebridge-0.0.1` from Assets, not the auto-generated `Source code.zip` from GitHub.

### Usage Guide

#### Windows

1. Download the appropriate `.zip` package for your architecture
2. Extract to any directory
3. Double-click `启动.bat` to run
4. Select the directory you want to share in the console
5. Choose access permissions (read-only/read-write)
6. Provide the displayed **endpoint URL** and **Token** to your AI assistant
7. Keep the console window open (closing it stops the service)

#### Linux

1. Download the appropriate `.tar.gz` package for your architecture
2. Extract: `tar -xzf filebridge-*.tar.gz`
3. Run: `./启动.sh` or `bash 启动.sh`
4. Follow prompts to select shared directory and permissions
5. Provide the displayed **endpoint URL** and **Token** to your AI assistant
6. Keep the terminal running (press `Ctrl+C` to stop)

### Security Guidelines

🔒 **Please strictly follow these security rules:**

- ❌ **DO NOT** publish Tokens in Issues, public chats, or screenshots
- ❌ **DO NOT** share system directories (e.g., `C:\Windows`, `/etc`, `/usr`)
- ❌ **DO NOT** share directories containing passwords, keys, or certificates
- ❌ **DO NOT** grant write or command execution permissions to untrusted AI
- ✅ **Prefer read-only mode whenever possible**
- ✅ **Only share dedicated work or test directories**
- ✅ **Close the service immediately after use**

### Issue Reporting

Encountered a problem? Please submit on the [Issues](../../issues) page with the following information:

- Filebridge version number
- Operating system and version
- CPU architecture (x64/ARM64)
- Protocol used (REST/MCP)
- Complete error message
- Steps to reproduce

⚠️ **Remove all sensitive information before submitting:** Tokens, personal directory paths, IP addresses, usernames, etc.

### License

MIT License
