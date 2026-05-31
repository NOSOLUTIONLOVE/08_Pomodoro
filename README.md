<div align="center">

# Pomodoro — 专注番茄钟

> 单文件番茄钟，打开即用。环形进度、动态背景、本地统计，助你保持专注。

[![License](https://img.shields.io/github/license/NOSOLUTIONLOVE/08_Pomodoro?style=for-the-badge)](LICENSE)
[![GitHub Repo](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/NOSOLUTIONLOVE/08_Pomodoro)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)]()
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com)

<br />

[Features](#-features) · [Quick Start](#-quick-start) · [Usage](#-usage) · [License](#-license)

</div>

---

## ✨ Features

### 计时模式

| 模式   | 默认时长 | 说明                     |
|--------|----------|--------------------------|
| 专注   | 25 分钟  | 工作时段，暖色渐变背景   |
| 短休息 | 5 分钟   | 完成一个番茄后的短暂休息 |
| 长休息 | 15 分钟  | 完成 4 个番茄后的长休息  |

专注结束自动进入短休息；达到设定番茄数后切换长休息；休息结束自动回到专注。

### 界面与交互

- 环形进度条，随模式切换颜色（专注 / 短休息 / 长休息）
- 番茄进度点，显示当前周期完成情况
- 动态背景与浮动粒子，专注时背景随进度加深
- 可自定义专注、短休、长休时长及长休息触发间隔（支持直接输入或 ± 按钮调整）

### 数据统计

- 今日 / 本周 / 累计番茄与连续天数
- 今日专注曲线、12 周热力图、24 小时分布
- 数据保存在浏览器 `localStorage`，换设备或清缓存会丢失

## 🚀 Quick Start

```bash
git clone git@github.com:NOSOLUTIONLOVE/08_Pomodoro.git
cd 08_Pomodoro
open index.html
```

## 📦 Installation

**无需安装依赖。** 克隆仓库后用浏览器打开 `index.html` 即可。

> 需要联网加载 [Inter](https://fonts.google.com/specimen/Inter) 字体；计时与统计功能离线可用。

## 📖 Usage

### 本地使用

将 `index.html` 拖入 Chrome、Safari、Firefox、Edge 等现代浏览器，或通过本地 HTTP 服务访问。

### 部署到 Vercel

1. 在 [Vercel](https://vercel.com) 导入 GitHub 仓库 `NOSOLUTIONLOVE/08_Pomodoro`
2. Framework Preset 选择 **Other**，Build / Install Command 留空
3. 部署完成后访问分配的域名

入口文件为 `index.html`，无需构建步骤。

### 快捷键

| 按键              | 作用               |
|-------------------|--------------------|
| `Space` / `Enter` | 开始 / 暂停        |
| `R`               | 重置当前计时       |
| `Escape`          | 关闭设置或统计面板 |

在输入框内时快捷键不生效。

### 设置

打开右侧齿轮面板，可修改专注 / 短休 / 长休时长及长休息间隔。数值可直接输入，也可用 `−` / `+` 调整；超出范围会自动校正并提示。

- **计时运行中**无法打开设置，需先暂停
- 修改专注 / 短休 / 长休时长后，会自动切换到对应 Tab 并显示完整新时长
- 若当前计时已有进度，修改时长前会弹出确认；取消则恢复原值
- 长休息间隔（番茄数）修改不影响当前计时模式

## 🛠 Tech Stack

| Layer    | Choice                          |
|----------|---------------------------------|
| Frontend | HTML5 + CSS + Vanilla JavaScript |
| Storage  | Browser `localStorage`          |
| Deploy   | Vercel（静态托管）              |

## 📄 License

See [LICENSE](LICENSE).
