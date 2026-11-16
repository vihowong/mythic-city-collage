---
name: mythic-city-collage
description: "Create and visually validate graphic-surreal image systems from compressed high-chroma color, staged impossible space, controlled detail density, and print/digital material tension. Use for art direction, image prompts, generated-image acceptance, series keyframes, poster critique, and short motion treatments; not for ordinary travel photography, conventional cyberpunk, or requests that merely combine a list of mythic symbols."
metadata:
  locale: zh-CN
  version: "1.3.0"
  cangjie.bundle-id: "bundle.mythic-city-visual-corpus"
  cangjie.capability-count: 9
---

# 神话城市拼贴

这不是一套元素清单，而是一套**以色彩结构和图像质感为核心的视觉语法**。具体场景、人物、城市或巨物只负责承载形式关系；验收时首先要看色块面积与邻近关系、冷暖与明暗层级、半调/纸噪/套色错位和材料表面是否成立。

龙、眼睛、门、棋盘、红日或城市都只是可替换的载体。先建立视觉关系，再决定用什么形象承担责任；不要从“把这些东西放在一起”开始。

本版本由 43 张竖幅静态图和 2 段动态研究蒸馏而来。实际图片生成请求以生成器输出和成图验收为准；素材作者与授权追溯不属于本技能的操作门槛。

## 三个识别点

1. **色彩面积结构。** 大面积深钴蓝、墨黑或暗绿承重，朱红、橙红与桃色制造事件，米白负责呼吸。重点不是出现过哪些颜色，而是每种颜色占多大面积、挨着什么、在明度中排第几层。
2. **图像质感。** 黑色轮廓、平涂色块、粗糙油墨边界、半调颗粒、套色错位、纸纤维和局部金属高光共同构成表面。所有对象都应像印在同一种材料上，而不是来自不同渲染器。
3. **可替换的空间承载。** 构图只负责组织色块、密度、方向与层级；人物、城市或叙事场景是可变承载物。即使把识别对象全部拿掉，色彩结构与图像质感仍应成立。

缺少其中两项时，通常只会得到复古插画、赛博海报或元素拼贴，而不是这套视觉。

## 先选构图骨架

构图骨架约束的是色块与质感的分布，不定义必须出现什么场景。

| 骨架 | 画面组织 | 细节分布 | 适用交付 |
| --- | --- | --- | --- |
| 孤立图腾 | 一个巨大主体悬在宽阔单色场中，余白达到 40–70% | 主体细节集中，背景极简 | 封面、肖像、单张冲击图 |
| 轴线登临 | 人物或入口在底部，道路、台阶、画面框或视线推向中心巨物 | 上下分区，中轴连续 | 海报、系列主视觉、纵深叙事 |
| 全景游行 | 地面、神话层、宇宙层横向堆叠，人物只是众多事件之一 | 三至五条密度带，局部故事多 | 世界观、长海报、视频全景 |
| 正面祭坛 | 严格或近对称的径向线、边框、主面孔、人物或符号居中 | 中央高密，外围秩序化 | 封面、音乐视觉、仪式感画面 |
| 框中世界 | 门、窗、镜框、屏幕或舞台口套住第二层空间 | 内外两级密度，边缘可做装饰带 | 门户、时间切换、嵌套叙事 |

不要同时使用三种骨架。需要复杂感时，增加同一骨架内的层级，而不是增加新的构图中心。

## 四个决策

1. **先写色彩—质感命题。** 用一句话说明颜色和表面如何产生张力，例如“冷黑秩序被一条暖色裂缝打断”。视觉命题应能脱离场景和具体符号成立。
2. **确定色调结构。** 先决定谁承担 35–55% 的基础面积，谁只占 8–20% 的事件面积，哪里保留米白色停顿，以及主要颜色之间的邻近关系。参考图不是等比例彩虹。
3. **画出细节岛。** 全图保留二至四个高细节区域，例如云团、人脸、建筑群或文字边带；其余区域用平涂、轮廓或低密纹理承重。高细节应围绕视觉事件，而不是均匀撒满。
4. **安排一次材质断裂。** 选择一个位置让镜面金属、摄影、低清像素或字体侵入基础印刷表面。断裂必须服务色彩结构，并通过同一色板、黑轮廓和全局颗粒重新统一。

## 工作流

1. 从需求中提炼：**色彩—质感命题、主要色块的面积与邻近关系、构图骨架、画幅、交付媒介**。不要先收集象征物。
2. 选定一种构图骨架，并确定缩略图状态下唯一可辨认的主体轮廓。
3. 指定色调结构：承重色、过渡色、事件色、停顿色；写清面积、明度与相邻颜色。再用墨黑统一轮廓和阴影。
4. 把细节组织成岛状区域，并决定哪一处材质发生断裂。
5. 选择一个具体形象执行视觉命题。形象可以来自城市、人物、动物、建筑、图案或抽象体，不要求出现“日常街头”。
6. 需要构图、色调、材质的具体判断时，读取 [style-grammar.md](references/style-grammar.md)。
7. 需要提示词、系列或视频方案时，读取 [production-recipes.md](references/production-recipes.md)。
8. 交付前按 [quality-rubric.md](references/quality-rubric.md) 自检，优先修复构图和色调问题。
9. 用户要求生成图片时，调用可用图像生成器，保存最终提示词和选定成图，优先验收色彩面积/邻近结构、明度层级和图像质感。场景识别只用于检查承载关系，不作为风格通过依据。
10. 做一次“去场景测试”：忽略人物、城市、建筑和故事后，画面仍应保留下可辨认的色块结构、冷暖冲突和统一表面。没有生成图时，不得宣称视觉验收通过。

## 深层能力路由

常规请求可使用本文件的常驻规则直接完成。遇到需要展开判断的任务，先读 [capability-index.md](references/capability-index.md)，再按当前问题只加载一张能力卡；明确跨两个领域时最多加载两张。

| 当前问题 | 能力卡 |
| --- | --- |
| 只有抽象主题、氛围词或元素清单 | [visual-proposition.md](references/capabilities/visual-proposition.md) |
| 不知道封面、全景、祭坛还是特写 | [composition-skeleton.md](references/capabilities/composition-skeleton.md) |
| 颜色太甜、太脏、太彩虹或缺少事件色 | [tone-hierarchy.md](references/capabilities/tone-hierarchy.md) |
| 现实与第二世界并存、梦境漂浮、空间不通 | [stage-space.md](references/capabilities/stage-space.md) |
| 要求丰富但缩略图失焦，或细节全图同密度 | [detail-density.md](references/capabilities/detail-density.md) |
| 照片、版画、金属、字体和像素像贴纸 | [material-surface.md](references/capabilities/material-surface.md) |
| 需要可直接使用的图像提示词 | [prompt-compiler.md](references/capabilities/prompt-compiler.md) |
| 现有成图像素材堆叠，需要诊断修复 | [diagnose-repair.md](references/capabilities/diagnose-repair.md) |
| 三连作、系列封面或关键帧统一 | [series-continuity.md](references/capabilities/series-continuity.md) |

需要规则速查时读取 [cheatsheet.md](references/cheatsheet.md)，需要完整术语时读取 [glossary.md](references/glossary.md)，需要理解蒸馏依据与局限时读取 [overview.md](references/overview.md) 和 [digest.md](references/digest.md)。成图验收的方法与样例读取 [visual-acceptance.md](references/visual-acceptance.md)。

## 反拼贴约束

- **缩略图测试：** 缩小到 200px 时，仍能看见一个主轮廓、一条轴线或一个明确入口。
- **去名词测试：** 去掉龙、眼睛、门等名词后，视觉命题仍然成立；否则只是在组合词典。
- **颗粒统一测试：** 全图共享同一套纸噪、半调或印刷错位，不能让每种素材拥有独立渲染质感。
- **重复规则测试：** 同一视觉规则至少出现三次，例如相同黑轮廓、相同橙蓝节奏或相同硬边云团，使异质素材像同一世界的产物。
- **细节预算测试：** 关闭最密区域后，画面仍应有清楚的色块构图；细节不能承担全部可读性。

## 输出契约

按用户需要的媒介交付，默认包含：

- **视觉命题：** 一个不依赖符号清单的情绪或思想冲突。
- **构图说明：** 骨架、主轮廓、观看入口、空间层级。
- **色调说明：** 承重色、事件色、停顿色与明暗结构。
- **细节与材质：** 高细节岛、基础表面、唯一材质断裂。
- **可执行提示词：** 包含构图、色调、线条、细节密度和负面约束。
- **视觉验收：** 生成请求必须包含实际成图、最终提示词、评分与必要修订记录。
- **动态方案：** 只在视频请求中加入镜头、异象显形、声音和节奏。

若用户只要成品图或提示词，直接执行，不先要求填写问卷。保持用户现有语言；英文提示词可以保留，但用用户语言解释视觉判断。

## 质量闸门

交付前确认：

- 色块面积有承重、过渡、事件和停顿四级职责，不是平均彩色。
- 主要颜色之间的邻近关系有意图，冷暖与明暗不是随机分布。
- 图像表面有明确的印刷/半调/套色/纸噪或等价质感，而不是无触感的干净渲染。
- 不同媒介共享同一黑轮廓、色板和表面颗粒。
- 高细节集中在明确区域，背景有足够的平涂或低密区域承重。
- 忽略所有可识别场景后，色彩结构与图像质感仍有独立辨识度。
- 缩略图仍能读出一个主形或方向轴；它是承载结构，不是场景要求。
- 图片生成请求已经检查真实成图，而不是只检查提示词。

若作品主要靠堆叠龙、眼睛、霓虹、棋盘和文字来证明风格，回到“四个决策”第 1 步重做。
