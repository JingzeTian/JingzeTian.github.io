# Project Gallery Cover Style Spec

本站 Project Gallery 封面图的统一风格规范。以后新增项目时，按本文生成 `featured.jpg`，保证视觉一致。

## 使用场景

- 为 `content/project/<slug>/` 生成 Gallery 封面
- 替换已有项目的封面并保持同一风格

## 文件约定

| 项 | 约定 |
|---|---|
| 路径 | `content/project/<slug>/featured.jpg` |
| 文件名 | 必须是 `featured.jpg`（小写；Hugo/Wowchemy 默认识别） |
| 比例 | **16:9** |
| 建议尺寸 | 长边约 **1600px**（如 1536×1024） |
| 体积 | JPEG，质量约 85–90，单张最好 **&lt; 200KB** |
| Front matter | 见下方模板 |

```yaml
image:
  focal_point: Center
  preview_only: true   # 封面只出现在 Gallery，不重复出现在详情页顶部
```

同时为项目写一句 **英文 summary**（约 12–25 词），放在 `index.md` 的 `summary` 字段，语气简洁、陈述事实、少用加粗。

## 视觉风格（必须遵守）

一句话：**冷静学术风的扁平编辑插画**——冷灰蓝底、居中单一隐喻、大留白、无文字。

### 调色

| 角色 | 色值 / 描述 |
|---|---|
| 主色 | Slate blue `#3B5B7A` |
| 辅色 | Muted teal（低饱和青绿） |
| 背景 | Misty cool-gray → pale blue 柔和渐变 |
| 忌用 | 紫色 / 霓虹发光 / 奶油底+赤陶 / 高对比赛博风 |

### 构图

- 画幅：**16:9 横版**
- 主体：**居中一个**项目隐喻（最多两个并列，如「双产品」）
- 留白充足，主体约占画面 40–60%
- 光感：左上方柔光，轻微软阴影
- 造型：扁平矢量 / 轻编辑插画，几何干净，可有极轻体积感

### 禁止出现

- 任何文字、字母、数字、logo、水印
- UI 真实截图、浏览器框、手机外框（可用抽象面板暗示）
- 血腥、暴力、写实恐怖元素
- 杂乱拼贴、多场景分镜、贴纸风徽章

## 英文 Prompt 模板

生成时**整段复制**，只替换 `{{METAPHOR}}`：

```text
Minimal editorial illustration cover for an academic HCI portfolio. Soft cool slate-blue (#3B5B7A) and muted teal accents on a misty cool-gray to pale blue gradient background. Flat vector with subtle soft shadows, generous negative space, no text, no logos, no neon glow, no purple. Soft lighting from upper-left. Centered metaphor: {{METAPHOR}}. Calm professional research aesthetic.
```

生成参数建议：

- Aspect ratio: `16:9`
- 输出文件名（临时）：`featured-<slug>.png`，再压缩为项目目录下的 `featured.jpg`

## 各项目隐喻参考（已有）

新增项目时，先想一句「这个项目用什么物体/场景一句话讲清」，再填入 `{{METAPHOR}}`。

| 项目 slug | Metaphor（英文，可作参考） |
|---|---|
| `eye-controlled-virtual-keyboard` | a stylized human eye casting a soft gaze beam onto a simplified QWERTY-like virtual keyboard floating in space |
| `undergraduate-thesis-platform` | a desktop eye-tracker bar beneath a monitor showing circular Fitts-law style target circles in a clean experimental UI layout |
| `hcix23-vr-accessibility` | a VR headset beside an abstract upper-body silhouette performing a gentle hand gesture, suggesting accessible VR interaction |
| `timer-smart-ring` | a sleek smart ring on a stylized hand, with a small floating clock/timer arc motif nearby suggesting time tracking |
| `daquan-ui-design` | a floating dashboard UI panel with abstract cards, map tiles, and charts suggesting an industrial park management system interface |
| `vr-moon` | a crescent moon and lunar surface with a tiny rover and a subtle VR headset silhouette, suggesting a moon-base VR simulation |
| `sea-battle-ue4` | a stylized warship on calm geometric ocean waves, with abstract targeting arcs suggesting a sea battle simulation; not aggressive or bloody |
| `two-product-designs` | side-by-side assistive design icons — a simplified eye-controlled wheelchair and a friendly small companion robot — balanced composition |
| `flapping-wing-aircraft` | a biomimetic flapping-wing micro aircraft inspired by a bird, mid-flight with elegant wing motion lines |

## 新增项目标准流程

1. 创建 `content/project/<slug>/`，写好 `index.md`（含英文 `summary`）。
2. 根据项目内容写一句 `{{METAPHOR}}`（具体、可画、单一焦点）。
3. 用上方 Prompt 模板生成 **16:9** 图。
4. 压缩为 JPEG（长边 ~1600，质量 ~86），保存为 `featured.jpg`。
5. 确认 front matter 含 `focal_point: Center` 与 `preview_only: true`。
6. 本地 `hugo server` 看首页 Projects Gallery 是否风格一致。

### 压缩命令示例（可选）

```bash
python -c "from PIL import Image; im=Image.open('in.png').convert('RGB'); w,h=im.size; m=1600; s=m/max(w,h) if max(w,h)>m else 1; im=im.resize((int(w*s),int(h*s))); im.save('featured.jpg','JPEG',quality=86,optimize=True)"
```

## Summary 写法提示

- 一句说清：**做了什么 + 用什么/对谁有用 +（可选）结果**
- 英文，约 12–25 词
- 避免模板腔（"This project aims to..."）和过多加粗
- 示例：`Participatory design with people with SMA on gaze-assisted upper-body gestures for VR — published at CHI'24.`

## 验收清单

- [ ] 与现有封面同一色系（冷灰蓝，非紫非霓虹）
- [ ] 无文字 / logo
- [ ] 16:9，主体居中，留白够
- [ ] 文件名为 `featured.jpg` 且体积合理
- [ ] `summary` 简短可读
- [ ] Gallery 里与其它卡片并排不违和
