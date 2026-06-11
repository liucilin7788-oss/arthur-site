# LibTV CLI 集成

## 项目简介

将 LibLib AI 的 LibTV CLI 工具集成到 Claude Code 中，实现通过命令行操作 AI 图像/视频生成画布。支持项目管理、节点操作、模型搜索、素材上传等功能。

## 核心功能

| 功能 | 说明 |
|------|------|
| **项目管理** | 创建、列出、绑定画布项目 |
| **节点操作** | 创建/删除/列出画布节点（图片、视频、音频、脚本等） |
| **模型搜索** | 搜索可用的 AI 模型（按类型筛选） |
| **素材上传** | 上传图片/视频/音频到画布节点 |
| **分组管理** | 创建/绑定分组，批量操作节点 |
| **脚本生成** | 从脚本节点生成分镜图组 |
| **账号管理** | 多账号切换、团队空间支持 |

## 常用命令

```bash
# 登录
libtv login web        # 浏览器扫码登录
libtv login phone      # 手机验证码登录

# 项目管理
libtv project list     # 列出所有项目
libtv project use <uuid>  # 绑定当前项目

# 节点操作
libtv node list        # 列出画布节点
libtv node create -t image -n "我的图片"  # 创建图片节点
libtv node delete <node>  # 删除节点

# 模型搜索
libtv model search <关键词>  # 搜索模型
libtv model <模型名>  # 查看模型详情

# 上传素材
libtv upload <节点> <文件路径>  # 上传文件到节点

# 分组管理
libtv group list       # 列出分组
libtv group create <分组名>  # 创建分组
libtv group use <分组名>  # 绑定当前分组
```

## 节点类型

| 类型 | 说明 |
|------|------|
| `image` | 图片节点 |
| `video` | 视频节点 |
| `audio` | 音频节点 |
| `script` | 脚本节点（可生成分镜图） |
| `text` | 文本节点 |
| `storyboard` | 分镜图节点 |
| `video-clip` | 视频片段节点 |

## 技术栈

- **LibTV CLI** — LibLib AI 官方命令行工具
- **Claude Code Skill** — 集成为 Claude Code 技能
- **Node.js** — CLI 运行时

## 演示视频

> 🎬 演示视频待上传

<!-- 视频位置 -->
<!-- <video src="videos/libtv-demo.mp4" controls width="100%"></video> -->

## 项目截图

> 📸 截图待添加

---

*Built by 亚瑟 | 2026*
