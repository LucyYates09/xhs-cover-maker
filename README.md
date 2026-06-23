# 小红书封面工具箱 · xhs-cover-maker

一套用于制作小红书封面的开源工具：

- **网页排版工具**：纯前端、零安装，所见即所得，一键导出高清 PNG。
- **Codex Skill**：把真人照片、参考封面、标题和 Logo 组合成 3:4 高点击封面，并精准控制人物身份、原始背景与正面柔光面灯。

👉 在线使用：https://lucyyates09.github.io/xhs-cover-maker/

## 网页工具功能

- **⚡ 智能排版**：把整段文案粘进去，自动识别大标题 / 粉色小标题 / 正文，`#话题标签` 自动删除。
- **📄 自动分页**：文字多了自动按页填满、放不下翻到下一页，回车换行也会自动分页。
- **🖼 悬浮图片**：插入或直接 `Ctrl/⌘+V` 粘贴图片，浮于文字之上自由拖动、缩放、裁剪、旋转、调圆角。
- **🅰 文字样式**：加粗 / 斜体 / 下划线、文字颜色、任意颜色文字底色（高亮）、网红中文字体（思源黑体、站酷快乐体、庆科黄油体等）。
- **🎨 背景**：纯色 + 格子 / 网格 / 横线 / 斜纹 / 圆点 / 棋盘等图案，颜色可调。
- **📐 比例**：3:4 竖封 / 1:1 方图 / 4:5，字号行距可调。
- **⬇ 导出**：每页单独导出 2x 高清 PNG。

## 使用

直接打开 `index.html`（双击即可），或访问上面的在线网址。无需联网即可使用，网络字体需联网加载（已用国内可访问镜像）。

## Codex Skill

技能目录：[skills/xhs-portrait-cover](skills/xhs-portrait-cover)

它适合这些需求：

- “参考这张封面的层级，用我的自拍做一张小红书封面。”
- “背景保留我照片原来的颜色，蓝色只做标题点缀。”
- “把脸提亮，像镜头正前方放了一盏强柔光面灯。”
- “不要轮廓光、白色描边或 AI 塑料磨皮。”
- “只改标题错字，其他设计全部保持不动。”

### 安装

```bash
git clone https://github.com/LucyYates09/xhs-cover-maker.git
mkdir -p ~/.codex/skills
cp -R xhs-cover-maker/skills/xhs-portrait-cover ~/.codex/skills/
```

安装后可这样调用：

```text
Use $xhs-portrait-cover to turn my portrait and headline into a polished
3:4 Xiaohongshu cover. Keep my original background and add a strong
frontal soft beauty light without rim light.
```

也可以直接用中文：

```text
使用 $xhs-portrait-cover，参考这张封面的文字层级，用我的自拍制作
3:4 小红书封面。保留原背景，只给人物增加正前方强柔光面灯。
```

### 技能特点

- 拆解参考图的版式、标题层级、颜色和视觉重心，而非机械照搬。
- 默认使用两行大标题、真人主体、分类标签和悬浮 Logo 卡片。
- 锁定五官、眼镜、痣、发型、表情、服装与人物比例。
- 明确区分正面面光和轮廓光，内置强面光与错误光效修正提示词。
- 每轮只调整一个变量，避免修改背景时连带改变人物或排版。
- 附带提示词配方与发布前 QA 检查清单。

技能本身不包含任何真人照片、品牌私有素材或生成结果。

## 技术

单文件 HTML + 原生 JS，导出用 [html2canvas](https://html2canvas.hertzen.com/)，中文字体走 Google Fonts 国内镜像（loli.net）。
