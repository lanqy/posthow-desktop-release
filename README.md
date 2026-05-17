# Post.How Desktop Release

Post.How 桌面客户端的公开发布仓库，用于分发 Windows、macOS 和 Linux 安装包。

> 当前版本：`v0.0.1`  
> 发布页面：[Post How v0.0.1](https://github.com/lanqy/posthow-desktop-release/releases/tag/v0.0.1)

## 下载

请前往 [Releases](https://github.com/lanqy/posthow-desktop-release/releases) 下载适合你系统的安装包。

| 系统 | 架构 | 安装包 | 适用场景 |
| --- | --- | --- | --- |
| Windows | x64 | [`Post.How_0.0.1_x64-setup.exe`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How_0.0.1_x64-setup.exe) | 推荐给大多数 Windows 用户 |
| Windows | x64 | [`Post.How_0.0.1_x64_en-US.msi`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How_0.0.1_x64_en-US.msi) | 适合企业部署或需要 MSI 的环境 |
| macOS | Apple Silicon | [`Post.How_0.0.1_aarch64.dmg`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How_0.0.1_aarch64.dmg) | 适用于 M 系列芯片 Mac |
| Linux | x86_64 | [`Post.How_0.0.1_amd64.AppImage`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How_0.0.1_amd64.AppImage) | 免安装运行 |
| Linux | amd64 | [`Post.How_0.0.1_amd64.deb`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How_0.0.1_amd64.deb) | Debian / Ubuntu 系发行版 |
| Linux | x86_64 | [`Post.How-0.0.1-1.x86_64.rpm`](https://github.com/lanqy/posthow-desktop-release/releases/download/v0.0.1/Post.How-0.0.1-1.x86_64.rpm) | Fedora / RHEL / openSUSE 系发行版 |

## 安装

### Windows

下载 `setup.exe` 后双击安装即可。若你需要通过企业软件分发系统部署，请使用 `.msi` 文件。

### macOS

下载 `.dmg` 文件并打开，将 `Post.How` 拖入 `Applications`。如果首次启动时出现安全提示，请在「系统设置 > 隐私与安全性」中允许打开。

### Linux

AppImage：

```bash
chmod +x Post.How_0.0.1_amd64.AppImage
./Post.How_0.0.1_amd64.AppImage
```

Debian / Ubuntu：

```bash
sudo apt install ./Post.How_0.0.1_amd64.deb
```

Fedora / RHEL / openSUSE：

```bash
sudo rpm -i Post.How-0.0.1-1.x86_64.rpm
```

## 校验文件

下载后可以使用 SHA-256 校验安装包完整性。

| 文件 | SHA-256 |
| --- | --- |
| `Post.How_0.0.1_x64-setup.exe` | `ed096b61661092cb58e385c3e3a10aca3f1fad435c5f737a7db60237100eec5e` |
| `Post.How_0.0.1_x64_en-US.msi` | `fb3b65466994abf6a6c5a6be1f3336b947821fade407cf6cdec7464af3291493` |
| `Post.How_0.0.1_aarch64.dmg` | `246167fe1841fb0be79fdf3f9902c012185d048e40e86d741217854f2cb56dc8` |
| `Post.How_0.0.1_amd64.AppImage` | `1654213d4a438fa27a4a790fb4cebc972e3bc6ae7aefd8f595ba097704a97c2e` |
| `Post.How_0.0.1_amd64.deb` | `75101e0fc93cab6448722502cb118b6d4c34cbbc5fb1199fb20775cc0c73bcc6` |
| `Post.How-0.0.1-1.x86_64.rpm` | `30e4db24c257b92ef06c061c18cf6e1ebbe1598ff4aaefccd2ecc736293e108e` |

macOS / Linux：

```bash
shasum -a 256 <filename>
```

Windows PowerShell：

```powershell
Get-FileHash .\<filename> -Algorithm SHA256
```

## 版本发布

本仓库仅保存 Post.How 桌面端 release 产物，不包含应用源码。新版本会以 GitHub Release 的形式发布，发布说明和安装包请以 [Releases](https://github.com/lanqy/posthow-desktop-release/releases) 页面为准。

## 问题反馈

如果下载、安装或启动过程中遇到问题，请在 [Issues](https://github.com/lanqy/posthow-desktop-release/issues) 中反馈，并尽量附上以下信息：

- 操作系统和版本
- 使用的安装包名称
- 错误截图或终端输出
- 可复现步骤
