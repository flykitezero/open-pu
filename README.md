# 🎵 open-pu

一个现代化的、可视化的歌曲乐谱编排工具，专为乐队和音乐创作者设计。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

![Preview](https://via.placeholder.com/800x400/13131a/8b5cf6?text=open-pu+Preview)

## ✨ 特性

- 🎼 **可视化编排** - 拖拽式段落组合，直观构建歌曲结构
- 🎹 **完整调性支持** - 12音名 + 大小调 + 中古调式 + Blues音阶
- 🎸 **丰富乐器配置** - 25+种乐器，支持搜索和自定义添加
- 🎵 **节拍器功能** - 内置节拍器，帮助你按照设定的速度练习或创作
- 🔢 **级数/音名切换** - 可在罗马级数（Ⅰ-Ⅴ-Ⅵ-Ⅳ）和实际音名（G-D-Em-C）之间切换
- 📊 **智能导出** - PDF/PNG/JSON 三种格式，段落长度按小节数比例显示
- 🔄 **数据导入导出** - 保存和恢复编排数据
- 📱 **响应式设计** - 现代化的 UI 设计，流畅的交互体验
- 🎨 **深色主题** - 专业的深色界面，适合长时间使用

## 🚀 在线演示

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Visit%20Demo-blue?style=for-the-badge&logo=github)](https://gdfgr2wag32n6.ok.kimi.link)

**[👉 点击体验在线演示](https://gdfgr2wag32n6.ok.kimi.link)**

### 网页演示截图

![open-pu Demo](demo-screenshot.png)

## 📦 快速开始

### 方式一：直接打开

1. 下载或克隆本项目
2. 直接用浏览器打开 `index.html`
3. 开始编排你的乐谱！

### 方式二：本地服务器

```bash
# 克隆项目
git clone https://github.com/yourusername/open-pu.git

# 进入目录
cd open-pu

# 启动本地服务器（任选一种）
# Python 3
python -m http.server 8080

# Node.js
npx serve .

# 然后访问 http://localhost:8080
```

## 📖 使用指南

### 1. 编辑歌曲信息

点击顶部的歌曲标题、艺人、调性、BPM 进行修改。

**调性选择**：
- 支持 12 个音名（C, C#/Db, D, D#/Eb, E, F, F#/Gb, G, G#/Ab, A, A#/Bb, B）
- 大小调切换
- 中古调式：Dorian, Phrygian, Lydian, Mixolydian, Locrian
- Blues 音阶

### 2. 节拍器

点击 BPM 旁边的节拍器图标可以启动/停止节拍器，帮助你按照设定的速度练习或创作。

### 3. 段落库

左侧是段落库，包含预设的段落模板：
- 前奏 (Intro)
- 主歌 (Verse)
- 副歌 (Chorus)
- 间奏 (Interlude)
- 尾奏 (Outro)
- Solo
- 其他 (Other)

**操作**：
- 拖拽到右侧时间轴
- 鼠标悬停在段落卡片上显示编辑按钮
- 点击 + 添加自定义段落

### 4. 时间轴编排

右侧是时间轴，按顺序排列你的歌曲结构。

**功能**：
- 拖拽段落到这里
- 查看总小节数、预估时长、段落数

### 5. 编辑段落

点击段落上的编辑按钮编辑：

- **段落名称** - 自定义段落名称
- **小节数** - 1-64 小节
- **段落类型** - 前奏/主歌/副歌/间奏/尾奏/Solo/其他
- **和弦进行** - 支持罗马级数（如 Ⅰ-Ⅴ-Ⅵ-Ⅳ）
- **乐器配置** - 25+种乐器，支持搜索和自定义

### 6. 级数/音名切换

点击顶部的小开关，可以在罗马级数（Ⅰ-Ⅴ-Ⅵ-Ⅳ）和实际音名（G-D-Em-C）之间切换显示。

### 7. 导出乐谱

点击「导出/导入」按钮，支持三种格式：

- **PDF** - 适合打印和分享
- **PNG** - 高清乐谱图片
- **JSON** - 保存编排数据（可导入恢复）

### 8. 导入数据

点击「导出/导入」按钮，可以：
- 上传 JSON 文件
- 粘贴 JSON 数据
- 选择替换或追加到当前编排

## 🎨 乐器列表

### 人声
- 男主唱、女主唱、和声

### 吉他
- 主音吉他、节奏吉他、木吉他

### 贝斯
- 贝斯、低音提琴

### 鼓组
- 鼓、打击乐

### 键盘
- 键盘、钢琴、合成器、管风琴

### 弦乐
- 弦乐组、小提琴、大提琴

### 管乐
- 萨克斯、小号、长号、长笛、单簧管、口琴

### 电子
- DJ/搓盘、采样器

### 自定义
- 支持添加任意自定义乐器

## 🛠️ 技术栈

- **HTML5** - 语义化结构
- **CSS3** - CSS Variables, Flexbox, Grid, Animations
- **JavaScript** - ES6+, Drag & Drop API, Web Audio API
- **Tailwind CSS** - 实用优先的 CSS 框架
- **html2canvas** - 截图导出
- **jsPDF** - PDF 生成

## 📁 项目结构

```
open-pu/
├── index.html          # 主页面
├── README.md           # 项目说明
├── LICENSE             # MIT 许可证
├── .gitignore          # Git 忽略文件
├── CHANGELOG.md        # 变更日志
├── CONTRIBUTING.md     # 贡献指南
└── .github/
    └── workflows/
        └── deploy.yml  # 部署配置
```

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本项目
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的修改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 📜 许可证

本项目基于 [MIT](LICENSE) 许可证开源。

## 🙏 致谢

- [Tailwind CSS](https://tailwindcss.com/) - 优秀的 CSS 框架
- [html2canvas](https://html2canvas.hertzen.com/) - 截图导出库
- [jsPDF](https://github.com/parallax/jsPDF) - PDF 生成库

---

Made with ❤️ for musicians