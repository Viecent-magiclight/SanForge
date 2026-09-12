<div align="center">

# SanForge

**macOS 上的 Xsan / 存储网络管理工具**

[![Platform](https://img.shields.io/badge/macOS-14%2B-000000?logo=apple&logoColor=white)](https://www.apple.com/macos/)
[![Architecture](https://img.shields.io/badge/Universal-Apple%20Silicon%20%7C%20Intel-blue)](https://developer.apple.com/documentation/apple-silicon)
[![Language](https://img.shields.io/badge/Language-中文%20%7C%20English-green)](#)
[![License](https://img.shields.io/badge/License-Proprietary-red)](#license)

[![Slack](https://img.shields.io/badge/Slack-XSAN%20Channel-4A154B?logo=slack&logoColor=white)](https://macadmins.slack.com/archives/C06JWSJ6P)

---

</div>

Apple 已停更 Server.app / Xsan Admin，不少制作、后期和媒资环境仍在用 Xsan 做共享存储。**SanForge** 是一款原生 macOS 应用，把 SAN 部署、卷与 LUN、目录、配额、访问控制和 DNS 收回到同一个界面里。

> 界面为 **简体中文 / English**，可随时切换。

---

## 📌 目录

- [能做什么](#-能做什么)
- [环境要求](#-环境要求)
- [使用说明](#-使用说明)
- [试用授权](#-试用授权)
- [反馈与支持](#-反馈与支持)
- [授权与版权](#-授权与版权)
- [English](#english)

---

## ✨ 能做什么

| 模块 | 功能说明 |
|------|----------|
| **SAN 部署** | 向导引导：在本机新建 SAN，或作为备用元数据控制器加入已有 SAN |
| **概览** | SAN / 元数据控制器 / Open Directory 状态、容量，以及常用下一步 |
| **卷** | 卷 → 存储池 → LUN 层级；启动 / 停止卷、查看容量、创建卷并分配存储池角色 |
| **LUN** | 扫描存储、写入标签，按已标记 / 未标记筛选；避免误改已归属卷的磁盘 |
| **配额** | 按用户、用户组或目录限制已挂载卷上的用量（软限额、硬限额、宽限期） |
| **计算机** | 元数据控制器与客户端：角色、网络、认证与存储链路 |
| **用户与组** | 管理 Open Directory 网络用户与用户组（与本机登录账户分开鉴权） |
| **文件管理** | 浏览已挂载卷，查看并写入 POSIX / ACL（含继承与向下传播） |
| **DNS** | 为 SAN 与目录主机名提供本机解析；退出主程序后仍可继续服务 |
| **日志与检查器** | 集中查看近期事件；选中对象时在右侧查看详情 |
| **运维补充** | 备份 SAN / 目录配置、导出客户端配置、设置主机名等 |

---

## 🖥 环境要求

- **macOS 14** 或更高版本
- 本机已安装 **Xsan**
- 使用**管理员账户**登录本应用
- **Apple Silicon** 与 **Intel Mac** 均可（Universal 包）

> ⚠️ 部分能力（扫描存储、改卷、改目录）需要本机已正确接入光纤 / iSCSI，并具备相应管理权限。

---

## 🚀 使用说明

1. 使用已打包的 `SanForge.app`（或从本仓库用 Xcode 打开并运行主程序）。
2. 首次从网上下载时，若被系统拦截：在 Finder 中 **右键 → 打开**。
3. 以本机管理员身份登录。
4. 按向导完成 SAN 配置，再管理卷、目录与日常运维。

> 📖 应用内 **帮助**（菜单或 `⌘?`）提供各板块的操作说明。

---

## 🔑 试用授权

软件提供 **7 天试用授权**，激活码如下：

```
SF2-T-CF-YZY2HH55Q4547LFFNWJNGPWFSVOHWJRPESYTWGTCSXXSHAJVNJCW2AWVWR75GL32XEPHIBBDYVBBVY7SQPFZ44O5KO4IT43JECVMSBY
```

> ⚠️ 正式使用需要有效授权。授权与商务合作请联系版权方，**请勿**在 Issue 或讨论区张贴激活相关内容。

---

## 💬 反馈与支持

- **Slack**：前往 [macadmins Slack XSAN 频道](https://macadmins.slack.com/archives/C06JWSJ6P) 交流
- **Issues**：在本仓库提交问题反馈

> 🎁 开发者将为积极反馈的用户提供**软件全量授权**。

---

## © 授权与版权

**Copyright © 魔力光年（Magic Light）**

SanForge 为专有商业软件。未经版权方书面许可，任何人不得复制、修改、再分发本软件或其源码，也不得将其用于未经授权的商业用途。

本仓库若公开，仅供展示与沟通；**不授予**开源许可证（No license）。购买或获发的是软件使用权，与仓库可见性无关。

---
---

<div align="center">

# SanForge

**Storage network administration for macOS Xsan**

</div>

Apple retired Server.app / Xsan Admin years ago, but many shops still run Xsan for shared storage. **SanForge** is a native macOS app that brings SAN deployment, volumes and LUNs, directory, quotas, access control, and DNS back into one place.

> The UI is available in **Simplified Chinese** and **English**.

---

## 📌 Table of Contents

- [Features](#-features)
- [Requirements](#-requirements)
- [Getting Started](#-getting-started)
- [Trial License](#-trial-license)
- [Feedback & Support](#-feedback--support)
- [License](#-license)

---

## ✨ Features

| Module | Description |
|--------|-------------|
| **SAN setup** | Guided wizard to create a SAN on this Mac, or join an existing SAN as a standby metadata controller |
| **Overview** | Live status for the SAN, metadata controller, and Open Directory, plus common next steps |
| **Volumes** | Volume → storage pool → LUN tree; start/stop volumes, review capacity, create volumes with pool roles |
| **LUNs** | Scan storage, apply labels, filter labeled / unlabeled; avoid relabeling LUNs already owned by a volume |
| **Quotas** | Limit space on a mounted volume by user, group, or folder (soft, hard, and grace) |
| **Computers** | Metadata controllers and clients: role, network, authentication, and storage link |
| **Users & groups** | Open Directory network accounts (directory admin auth is separate from the Mac login) |
| **File management** | Browse mounted volumes; view and write POSIX / ACL entries, including inheritance |
| **DNS** | Local name resolution for SAN and directory hosts; can keep serving after the app quits |
| **Logs & Inspector** | Recent events in one place; details for the selected object |
| **Ops extras** | Back up SAN / directory config, export a client profile, set the host name, and more |

---

## 🖥 Requirements

- **macOS 14** or later
- **Xsan** installed on this Mac
- Sign in to the app as a **local administrator**
- **Apple Silicon** and **Intel** (Universal build)

> ⚠️ Scanning storage and changing volumes or directory data also require a working fabric / iSCSI path and the matching admin rights.

---

## 🚀 Getting Started

1. Open the packaged `SanForge.app`, or open this repository in Xcode and run the main app.
2. If Gatekeeper blocks a downloaded build: in Finder, **Control-click → Open**.
3. Sign in as a local administrator.
4. Use the wizard to configure the SAN, then manage volumes and day-to-day operations.

> 📖 In-app **Help** (Help menu or `⌘?`) covers each pane.

---

## 🔑 Trial License

7-day trial activation key for the software:

```
SF2-T-CF-YZY2HH55Q4547LFFNWJNGPWFSVOHWJRPESYTWGTCSXXSHAJVNJCW2AWVWR75GL32XEPHIBBDYVBBVY7SQPFZ44O5KO4IT43JECVMSBY
```

> ⚠️ A valid license is required for production use. Contact the copyright holder for licensing. **Do not** post activation material in Issues or Discussions.

---

## 💬 Feedback & Support

- **Slack**: Join the [macadmins Slack XSAN channel](https://macadmins.slack.com/archives/C06JWSJ6P)
- **Issues**: Submit feedback in this repository

> 🎁 Developers will offer full software licenses to users who provide valuable feedback.

---

## © License

**Copyright © Magic Light (魔力光年)**

SanForge is proprietary commercial software. Without written permission you may not copy, modify, or redistribute the software or its source, and you may not use it for unauthorized commercial purposes.

If this repository is public, it is for visibility and conversation only. **No open-source license is granted.** A purchased or issued license is a right to use the product; it is not a source license.

---

<div align="center">

*Made with ❤️ for macOS storage administrators*

</div>
