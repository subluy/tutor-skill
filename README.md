# Tutor — 通俗讲题 Skill

用最通俗易懂的语言讲解物理、高数、C语言等理工科题目，配合精美 HTML 动画演示。

## 支持的领域

- **物理**：力学、电磁学、热学、光学、波动
- **高数**：微积分、线性代数、概率统计
- **C语言**：语法、指针、内存管理、数据结构、算法

## 效果预览

讲题时会自动生成带交互式动画的 HTML 页面：

![demo](https://img.shields.io/badge/示例-冒泡排序-blue)

### 冒泡排序讲解
- 🎬 交互式柱状图动画（单步/自动播放/调速）
- 📊 9 趟完整执行过程追踪表
- 💻 代码逐行对照讲解
- 🌓 自动适配深色/浅色模式

### 嵌套三目运算符讲解
- 🌳 SVG 决策树图，绿色标记实际执行路径
- 🔍 逐步拆解求值过程
- 📝 三目 vs if-else 对照

## 安装

```bash
npx skills add <your-github-username>/tutor-skill@tutor -g -y
```

或者手动复制到 `~/.claude/skills/tutor/`：

```bash
mkdir -p ~/.claude/skills/tutor
cp SKILL.md ~/.claude/skills/tutor/
```

## 使用方式

```
帮我讲讲冒泡排序
解释一下这个三目运算符
导数的几何意义是什么
```

每次讲题会基于 `template.html` 生成带交互动画的讲解页面，自动用浏览器打开。

## 文件结构

```
tutor-skill/
├── SKILL.md         # Skill 定义（触发条件、工作流程）
├── template.html    # HTML 模板（MathJax + Prism.js + SVG 动画）
└── README.md        # 本文件
```

## 模板特性

- 📐 **MathJax** 数学公式渲染
- 💻 **Prism.js** C 语言代码高亮
- 🎨 **CSS 动画** + **SVG 图解**
- 🌓 自动跟随系统深色/浅色模式
- 📱 响应式布局

## 讲题输出位置

生成的 HTML 文件存放在：`~/Desktop/讲题/`
