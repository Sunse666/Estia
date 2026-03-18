# Estia
<p align="center"> <img src="assets/logo/logo.png" alt="Estia Logo" width="128"> </p><p align="center"> <strong>轻量动态视频壁纸</strong> </p><p align="center"> <img src="https://img.shields.io/badge/Platform-Windows-blue?style=flat-square" alt="Platform"> <img src="https://img.shields.io/badge/Engine-MPV-9b4dca?style=flat-square" alt="Engine"> </p>


## ✨ 简介
- 基于 MPV 的 Windows 动态视频壁纸工具，追求极致的轻量与简洁无需复杂配置，只需一个视频文件，即可让你的桌面栩栩如生，告别单调的静态壁纸，拥抱动感的视觉体验


## 🖼️ 截图

这个因人而异


## 🚀 功能特性

### 🎬 视频壁纸
- 支持主流视频格式(MP4、MKV、AVI、MOV、WebM 等)
- 无缝循环播放，流畅无卡顿
- 全屏自适应，完美贴合桌面

### ⚡ 轻量高效
- 基于 MPV 播放器内核，资源占用极低
- 无后台服务，随开随用
- 不影响桌面图标操作

### 🎛️ 灵活配置

- 支持音量调节(0-100)
- 可调播放速度(0.5x - 2.0x)
- 一键静音开关
- 循环/单次播放切换

### 🔧 简单易用
- INI 配置文件，直观易懂
- 零学习成本，开箱即用


## 📦 安装与使用

### 系统要求
- 操作系统：Windows 10 / 11
- 依赖：无需额外安装

### 快速开始

1. 从 Releases 页面下载最新版本
2. 解压到任意目录
3. 将视频文件放入程序目录，命名为 video.mp4(或修改配置指定路径)
4. 运行 Estia.exe

### 目录结构

```
Estia/
├── Estia.exe        # 主程序
├── config.ini      # 配置文件
└── video.mp4     # 视频文件
```


## ⚙️ 配置说明

配置文件为程序目录下的 config.ini，使用 INI 格式

### 完整配置示例

```INI
[Settings]
//视频文件路径
video_path = .\video.mp4

//音量 (0-100)
volume = 100

//是否循环播放 (inf/no)
loop = inf

//是否静音 (yes/no)
mute = no

//播放速度 (0.5-2.0)
speed = 1.0
```

### 配置项说明

|字段|默认值|说明|
|---|---|---|
|video_path|.\video.mp4|视频文件路径|
|volume|100|音量，范围 0-100|
|loop|inf|循环播放：inf(无限循环)/ no(单次播放)|
|mute|no|静音：yes / no|
|speed|1.0|播放速度，范围 0.5-2.0|

### 路径写法

```
# 相对路径(推荐)
video_path = .\video.mp4
video_path = .\videos\nature.mp4

# 绝对路径
video_path = C:\Videos\wallpaper.mp4
video_path = D:\Downloads\动态壁纸.mp4
```

> [!TIP]
> 支持的视频格式：MP4、MKV、AVI、MOV、WebM、FLV、WMV 等主流格式


## 🛠️ 技术特点
- 基于 MPV 播放器内核，硬件解码加速
- 利用 Windows WorkerW 窗口层实现桌面嵌入
- 不修改系统文件，安全无侵入
- 支持多显示器(主显示器)
- 低内存占用，低 CPU 使用率


## ❓ 常见问题

### Q: 桌面图标还能正常点击吗？

可以视频窗口嵌入在桌面图标层的下方，不影响任何桌面操作

### Q: 如何更换壁纸视频？

方法一：将新视频命名为 video.mp4 替换原文件，重启程序

方法二：修改 config.ini 中的 video_path 指向新视频路径

### Q: 视频没有声音？

检查配置文件中：

- mute 是否设置为 no
- volume 是否大于 0

```
mute = no
volume = 100
```

### Q: 视频卡顿/不流畅？

- 尝试使用较低分辨率的视频(推荐 1080p)
- 使用 H.264 编码的 MP4 格式
- 确保显卡驱动已更新

### Q: 支持多显示器吗？

目前仅支持主显示器显示动态壁纸，多显示器支持计划中

### Q: 修改配置后如何生效？

修改 config.ini 保存后，重启程序即可生效

### Q: 为什么开机自启动了？

自动设置，不需要可以在任务管理器内关闭


## 📋 推荐视频资源

- 二次元画风壁纸
- 自然风景延时摄影
- 赛博朋克城市夜景
- 水族馆/海洋生物

> [!TIP]
> 推荐使用无缝循环视频，避免播放时出现明显的跳帧


## 🗺️ 计划

- [ ] 系统托盘控制菜单
- [ ] 多显示器支持
- [ ] 播放列表 / 随机切换
- [ ] 定时切换壁纸
- [ ] GUI 设置界面
- [ ] 支持网络视频流

---
<p align="center"> Made with 💚 by Estia </p>
