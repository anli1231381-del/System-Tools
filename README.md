# PointArt System Tools

PointArt 内部 Windows 实用工具归档库。当前收录序列与视频处理、PDF 合并、文件夹映射、文件拷贝和序列检查等 5 个独立工具。

> 本仓库用于保存工具说明和发布记录，不是源代码仓库。可执行文件统一从 [Releases](https://github.com/anli1231381-del/PointArt-System-Tools/releases) 下载。

## 工具列表

| 原文件 | Release 附件 | 用途 | 文件版本 | 大小 |
| --- | --- | --- | --- | ---: |
| `序列视频多任务编辑大师_v3.exe` | `sequence-video-multitask-editor-v3.exe` | 序列与视频多任务编辑 | 文件名标识 v3 | 89.79 MB |
| `PDF合并大师.exe` | `pdf-merge-master.exe` | PDF 与图片合并 | 1.0.0 | 65.59 MB |
| `文件夹映射大师.exe` | `folder-mapping-master.exe` | 文件夹映射管理 | 未提供 | 43.31 MB |
| `文件拷贝大师1.0.exe` | `file-copy-master-1.0.exe` | 文件拷贝任务 | 文件名标识 1.0 | 10.45 MB |
| `序列检查大师.exe` | `sequence-check-master.exe` | 序列文件检查 | 未提供 | 7.66 MB |

## 下载

前往 [Releases](https://github.com/anli1231381-del/PointArt-System-Tools/releases) 打开最新发布记录，可按需单独下载每个 EXE。GitHub 会简化中文附件名，因此 Release 使用上表中的英文文件名；文件内容与对应原文件一致。

当前归档版本：`2026.08.25`。

## SHA-256

下载后建议先校验文件哈希：

| 文件 | SHA-256 |
| --- | --- |
| `序列视频多任务编辑大师_v3.exe` | `B2809BC1C9F20C86DB5C397AF867A6C3A3C1BB351D50735C3ECA45DCCF25E1F7` |
| `PDF合并大师.exe` | `F2CB08093D82DD25243326E6EC5404CA5E718CE523835A8D952B0D263E569D9D` |
| `文件夹映射大师.exe` | `0BDA4784C4DD0E1DD1127839631B0423173C1A0DE319CD335255E7D6417922B8` |
| `文件拷贝大师1.0.exe` | `E7EEED7983708A3D36D9AED21A9DEA119376F5F9860430A0D450340F6FCBE4C0` |
| `序列检查大师.exe` | `30F845A3F282233822994FA7CE6A890D6CAA272D33E2421D89C674D2BC316983` |

PowerShell 校验示例：

```powershell
Get-FileHash -Algorithm SHA256 '.\PDF合并大师.exe'
```

## 安全提示

- 当前 5 个 EXE 均未附带 Authenticode 数字签名，Windows 可能显示 SmartScreen 或“未知发布者”提示。
- 未签名不等同于文件一定不安全；请确认下载来源，并使用上方 SHA-256 核对文件完整性。
- 文件映射、拷贝、批量编辑类工具可能修改大量文件。首次使用前请准备备份，并在测试目录中验证流程。
- 请勿把来源不明、哈希不一致或被意外替换的文件加入本仓库的 Release。

## 文件信息

| 文件 | 原始修改时间 | 数字签名 |
| --- | --- | --- |
| `序列视频多任务编辑大师_v3.exe` | 2026-07-14 18:42 | 未签名 |
| `PDF合并大师.exe` | 2026-07-18 14:37 | 未签名 |
| `文件夹映射大师.exe` | 2025-07-30 18:06 | 未签名 |
| `文件拷贝大师1.0.exe` | 2025-07-28 23:15 | 未签名 |
| `序列检查大师.exe` | 2025-07-17 11:06 | 未签名 |

## 发布约定

- Git 仓库只保存 README 和发布说明，不直接提交二进制文件。
- EXE 作为 Release 附件保存，避免二进制文件进入 Git 历史。
- 更新任一工具时应重新计算 SHA-256，并在新 Release 中记录变更。

