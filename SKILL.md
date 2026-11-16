---
name: mythic-city-collage
description: "Create and visually validate graphic-surreal image systems whose primary criteria are color-area structure, adjacency and temperature relationships, low-highlight value hierarchy, orthographic or panoramic composition, and multi-scale printed/digital microtexture. Use for art direction, image prompts, generated-image acceptance, poster critique, and series continuity; not for ordinary travel photography, conventional cyberpunk, clean 3D product rendering, or requests that merely combine a list of mythic symbols."
metadata:
  locale: zh-CN
  version: "1.4.0"
  cangjie.bundle-id: "bundle.kiuzyx-visual"
  cangjie.capability-count: 9
---

# 神话城市拼贴

这是一套以**色彩搭配结构**和**图片质感风格**为核心的视觉语法。人物、房间、城市、道路、神兽和宇宙都只是可变承载物；不能靠场景相似来证明风格成立。

本版本结合 `@kiuzyx` 近期 27 张作品与现有 43 张历史语料。近期作品更暗、局部颜色更强、边缘密度更低，但两者共享深色大场、暖中性停顿、朱红事件、清晰硬边和整图微颗粒。

## 四个主轴

1. **色调结构。** 深蓝、近黑、暗绿承担大面积重量；米白、暖棕和肤色提供过渡与停顿；朱红/橙色只占小面积做事件。重点不是有哪些颜色，而是面积、明度与邻接。
2. **构图结构。** 先选安静正交场域或极繁全景。安静模式依赖门窗、墙线、桌沿、道路和巨大负形；极繁模式依赖黑空、云海、城市和视觉流。
3. **图片质量与细节。** 清晰硬边必须与全图微颗粒并存；颗粒至少包含微噪、半调/抖动和较大纸纹/压缩块三个尺度。细节集中在二至四个岛，而不是全图均匀铺满。
4. **整体视觉风格。** 日常空间被轻微异化，但图像保持冷静、平面、精确和哑光。忽略可识别对象后，色块结构与复制表面仍应成立。

## 先选构图模式

构图模式组织的是色块、负形、明度和细节，不规定必须出现什么场景。

| 模式 | 画面组织 | 默认细节节奏 |
| --- | --- | --- |
| 安静正交场域 | 墙面、门窗、桌沿、车厢、电梯或道路建立横竖舞台 | 大面积低频负形 + 一至三个局部细节岛 |
| 极繁全景 | 黑空、云海、城市、神山或神话体形成多密度带 | 至少一块大面积安静黑色/蓝色场 |
| 孤立主体 | 一个大形或一个人物处于宽阔单色场 | 主体局部高密，背景极简 |
| 轴线登临 | 色温与明度沿一条入口、窗口或道路推进 | 轴线和门槛成岛，两侧低频 |
| 正面祭坛 | 中央主体、放射线和边框形成近对称秩序 | 中央高密，边缘重复收束 |
| 超近景切片 | 面部、局部表面或一个事件色占满画面 | 只保留一个材质断点和少量背景 |
| 框中世界 | 门、窗、屏幕或画框套住第二层表面 | 内外共享色板与颗粒，密度可不同 |

一张图只选一个主模式。需要复杂感时，增加同一模式内的层级，不并列多个骨架。

## 色彩决策

1. **先写色彩—质感命题。** 例如“冷黑大场被一条朱红裂缝打断”或“暖米白纸张中有一块极小金属反光”，而不是先罗列场景。
2. **分配面积。** 深色承重通常最大，暖中性提供停顿，朱红/橙红只做少量事件。近期样本约为近黑 22%、暗绿 12%、深钴蓝 10%、暖棕/米白 35%、朱红 7%。
3. **规定邻接。** 至少写出三组：哪两种颜色直接相接、在哪个几何边界、承担什么结构。米白咬入蓝、朱红切黑、暖中性或窄绿色桥接冷暖，是常用关系。
4. **压低高光。** 近期样本高光约 1.2%，深阴影约 56%。黑色与深蓝必须保留细颗粒、冷色差或局部轮廓，不能压成没有层次的死黑。

## 图像质量

- **边缘：** 建筑、人物和色块保持清楚、硬直、可远读。
- **填充：** 大面积平涂或有限色阶，不使用光滑连续渐变。
- **微颗粒：** 细噪、抖动、网点或纸纤维覆盖整图。
- **纹理尺度：** 至少三种尺度，例如细纸噪、中尺度半调/抖动、较大压缩块或刷痕。
- **材料断点：** 只保留一个小面积主导事件，例如金属、照片、像素或字体，并被同一色板和颗粒缝合。
- **整体光照：** 哑光、低反光、低泛光；光只用来区分结构，不把画面变成三维场景。

## 工作流

1. 提炼**色彩—质感命题、主要邻接、构图模式、画幅和输出媒介**。
2. 选择安静正交场域或极繁全景，并固定一个 200px 可读的主形、轴线或负形结构。
3. 指定色彩面积、明度职责与至少三组邻接关系。
4. 预留 30–60% 低频负形；把细节集中到二至四个岛。
5. 建立统一硬边、平涂、微颗粒和半调/抖动表面，再安排一个小面积材质断点。
6. 最后选择人物、房间、道路、城市或神话体作为可替换承载。
7. 需要深入构图、色调或材质时，读取 [style-grammar.md](references/style-grammar.md)。
8. 需要提示词或系列方案时，读取 [production-recipes.md](references/production-recipes.md)。
9. 交付前按 [quality-rubric.md](references/quality-rubric.md) 检查色彩结构、构图、图像质量和场景独立性。
10. 用户要求图片时，调用可用图像生成器，保存最终提示词和真实成图，再执行 200px、灰度、去场景和图像质量评分；不能只验提示词。

## 深层能力路由

先读 [capability-index.md](references/capability-index.md)；按当前问题加载一张能力卡，跨两个领域时最多两张。

| 当前问题 | 能力卡 |
| --- | --- |
| 主题、场景或元素无法形成风格命题 | [visual-proposition.md](references/capabilities/visual-proposition.md) |
| 不知道该做安静场域还是极繁全景 | [composition-skeleton.md](references/capabilities/composition-skeleton.md) |
| 色块面积、邻接、冷暖或暗部不稳 | [tone-hierarchy.md](references/capabilities/tone-hierarchy.md) |
| 需要门窗、框线、室内外层次和负形 | [stage-space.md](references/capabilities/stage-space.md) |
| 细节太满、负形不足或缩略图失焦 | [detail-density.md](references/capabilities/detail-density.md) |
| 图片太光滑、颗粒单一或像廉价复古滤镜 | [material-surface.md](references/capabilities/material-surface.md) |
| 需要可执行提示词 | [prompt-compiler.md](references/capabilities/prompt-compiler.md) |
| 成图颜色像但整体质感不对 | [diagnose-repair.md](references/capabilities/diagnose-repair.md) |
| 系列统一与新旧模式切换 | [series-continuity.md](references/capabilities/series-continuity.md) |

规则速查见 [cheatsheet.md](references/cheatsheet.md)，术语见 [glossary.md](references/glossary.md)，来源与判断依据见 [overview.md](references/overview.md)，完整方法说明见 [digest.md](references/digest.md)。实际成图与验收记录见 [visual-acceptance.md](references/visual-acceptance.md)。

## 反拼贴与反场景化

- **缩略图测试：** 200px 下仍能看见主形、结构轴或明确负形。
- **去场景测试：** 忽略人物、房间、道路、城市和故事名称后，色彩面积、邻接与表面仍成立。
- **灰度测试：** 仍有深色承重、暖中性停顿和少量事件亮部。
- **纹理测试：** 全图有连续微颗粒，同时至少存在三种纹理尺度。
- **细节预算测试：** 关闭最密区域后，色块和构图仍完整。

## 输出契约

按用户要求的媒介交付，默认包含：

- **色彩结构：** 色角色、面积、明度、三组主要邻接。
- **构图模式：** 安静/极繁选择、主形、负形、观看路径。
- **图像质量：** 硬边、平涂、多尺度微颗粒、材质断点和暗部层次。
- **细节岛：** 二至四个高密区域及其职责。
- **可执行提示词：** 色彩与表面在前，场景在后，并附针对性负面约束。
- **视觉验收：** 实际成图、最终提示词、四项主轴评分和必要修订记录。

## 质量闸门

- 色彩存在承重、过渡、事件与停顿职责，不是平均彩色。
- 至少有三组明确的颜色邻接。
- 构图属于清楚的安静场域或极繁全景，不混成两个中心。
- 大面积负形与局部细节岛形成节奏。
- 清晰硬边与全图多尺度微颗粒同时存在。
- 暗部有层次，高光面积小且无泛光。
- 忽略场景和人物后，色彩结构与图片质感仍成立。
- 生成请求已经检查真实成图，而不是只检查提示词。

## 已知边界

- 本轮近期样本来自 X 公开图，平台 `large` 尺寸可能经过压缩；不能把平台纹理全部归因于作者原始输出。
- 作者与授权检查不属于本技能的验收门槛。
- 横版、方形和真实无损原图的适配仍需额外测试。

若作品主要靠特定房间、城市、龙、眼睛、霓虹或文字证明风格，回到“四个主轴”重新建立色彩、构图与图像质量。
