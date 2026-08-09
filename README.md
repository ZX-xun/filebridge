# filebridge
让你的电脑上的AI 通过 REST/MCP 远程读取和操作另一台电脑的文件
Filebridge 可以临时把一台 Windows 或 Linux 电脑变成受控的 REST/MCP 文件服务，让获得授权的 AI 读取或操作指定目录。

## 当前公开版本

当前公开版本：v0.0.1

这是早期测试版本，建议仅共享专门用于调试的目录，不要直接共享整个系统盘。

## 下载

请进入右侧的 Releases 页面，根据目标电脑的系统和处理器下载对应安装包。

- Windows x64：普通 Intel/AMD Windows 电脑
- Windows ARM64：ARM Windows 电脑
- Linux x64：Intel/AMD Linux 电脑
- Linux ARM64：ARM Linux 设备

不要下载 GitHub 自动生成的 `Source code.zip`，应下载 Release 的 Assets 中以 `filebridge-0.0.1` 开头的安装包。

## 使用流程

1. 下载对应系统的安装包。
2. 解压安装包。
3. Windows 双击“启动.bat”。
4. Linux 运行“启动.sh”。
5. 选择允许访问的目录和权限。
6. 把程序显示的端点和 Token 发给需要连接的 AI。
7. 保持程序窗口打开，关闭窗口后连接停止。

## 安全提醒

- Token 相当于临时密码，不要发布在 Issue、截图或公开聊天中。
- 优先使用只读模式。
- 不要向不可信的 AI 开启命令执行权限。
- 不建议共享系统盘、用户主目录或包含密码、密钥的目录。

## 问题反馈

如果使用中遇到问题，请在 Issues 页面提交，并提供：

- Filebridge 版本
- 操作系统
- CPU 架构
- 使用的连接模式
- 完整错误信息
- 问题复现步骤

请删除错误信息中的 Token、个人目录、IP 地址和隐私数据。

## License

MIT
