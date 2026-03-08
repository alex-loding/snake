# 🐍 SNAKE — 贪吃蛇

> 一个功能丰富、主题多彩的单文件贪吃蛇游戏，无需任何依赖，开箱即玩。

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Zero Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen?style=flat-square)

---

## ✨ 特性

### 🎮 游戏玩法
- **经典贪吃蛇**：吃食物得分（每颗 +10），蛇身随之增长
- **饥饿机制**：超过时限未吃到食物则游戏结束，保持节奏紧张感
- **穿墙模式**：开启后蛇可穿越边界从对侧出现
- **多档速度**：慢速 / 正常 / 快速 / 超频 / 极限，满足不同水平玩家

### 🤖 AI 自动驾驶
- 内置智能 AI，可接管操控自动寻路吃食物
- 采用 BFS 最短路径 + 安全性校验 + 哈密顿回路保命策略
- AI 分数与人工分数分开记录，互不干扰

### 🎨 10 套视觉主题
| # | 主题名 | 风格 |
|---|--------|------|
| ① | 赛博朋克 | 霓虹蓝紫，扫描线特效 |
| ② | 深渊暗黑 | 极暗紫红，神秘氛围 |
| ③ | 明亮白昼 | 清爽白底，日间友好 |
| ④ | 幽暗森林 | 深绿色调，衬线字体 |
| ⑤ | 复古像素 | 经典红黑，像素风 |
| ⑥ | 樱花和风 | 粉色系，日系美感 |
| ⑦ | 熔岩火焰 | 橙红高温，炙热感 |
| ⑧ | 极地冰雪 | 浅蓝冷色，冰晶感 |
| ⑨ | 奢华描金 | 黑金配色（默认） |
| ⑩ | 故障艺术 | 纯黑+荧光绿，Glitch 抖动 |

### 🏆 排行榜
- 自动记录 **机器人 Top 10** 和 **人类 Top 10**
- 数据持久化到 `localStorage`，刷新不丢失
- 支持一键清空记录

### 🌐 双语支持
- 中文 / English 实时切换，全界面翻译无死角

### 📐 自适应布局
- 网格尺寸可选：10×10 至 40×40，或开启**自适应**随窗口自动调整
- 移动端兼容，支持触屏方向滑动控制

---

## 🚀 快速开始

无需安装，无需服务器，直接双击打开即可游戏：

```bash
# 克隆仓库
git clone https://github.com/alex-loding/snake.git

# 直接在浏览器中打开
open snake.html
```

或者直接[下载 snake.html](./snake.html) 到本地，用任意浏览器打开。

---

## 🕹️ 操作方式

### 键盘
| 按键 | 功能 |
|------|------|
| `↑ ↓ ← →` | 控制方向 |
| `W A S D` | 控制方向（备选） |
| `Space` | 暂停 / 继续 |
| `R` | 重新开始 |
| `⌨` 按钮 | 查看所有快捷键 |

### 触屏
在画布上滑动手指即可控制方向。

---

## ⚙️ 游戏设置

所有设置会自动保存，下次打开时恢复：

| 设置项 | 说明 |
|--------|------|
| 游戏速度 | 慢速 → 极限，共 5 档 |
| 蛇盘大小 | 10×10 ~ 40×40 或自适应 |
| 主题 | 10 套主题即时切换 |
| 语言 | 中文 / English |
| 🤖 自动驾驶 | AI 接管控制 |
| 🌀 穿墙模式 | 开启边界穿越 |

---

## 📁 项目结构

```
snake.html   ← 完整游戏，单文件，零依赖
README.md    ← 本文档
```

---

## 🛠️ 技术实现

- **纯原生 HTML5 + CSS3 + JavaScript**，无任何框架或第三方库
- Canvas 2D 渲染游戏画面
- CSS 变量（`var()`）驱动主题切换，过渡丝滑
- `localStorage` 持久化分数与设置
- AI 核心：BFS 寻路 + 蛇尾安全性模拟 + 哈密顿回路兜底

---

## 📄 License

[MIT](./LICENSE) © 2025
