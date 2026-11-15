# 制作配方

## 先把需求变成六个变量

```text
ground       一个具体的当代地点/物件
witness      谁在观看：通勤者、恋人、店员、无脸人、动物
anomaly      出现什么：巨日、龙、面具、眼睛、门、解剖体
operation    异常改变什么：揭示、吞噬、交换、复制、倒转、封门
intensity    1 克制的日常显灵 / 2 神话叙事 / 3 极繁拼贴
format       图片画幅、视频时长、系列数量、平台
```

信息不足时，优先选择便利店、住宅巷口、夜间道路、潮湿积水和通勤者。它们与这套视觉最稳，也最容易避免空泛的“梦境”。

## 图像提示词公式

```text
[画幅与用途]. [日常锚点与地点]. [观察者及其姿态]. [从前景到异常的主导轴线].
[主导异象 = 尺度 + 象征动作]. [城市/山水/建筑层如何被改变].
[冷底暖冲突色板]. [复古日式版画 + 硬边拼贴 + 套色偏移 + 纸噪材质].
[镜头高度、景别、光线、天气]. [叙事语气].
```

把“异象 = 尺度 + 动作”写清楚。例如不要只写“很多龙”，而写“一条巨大的青龙从云中俯冲，身体围住城市，头部正对前景台阶”。

### 提示词 1：神话全景

```text
Vertical 2:3 surreal editorial poster. A lone commuter in a black coat stands at the bottom of
a wide red carpet leading through a blue-and-vermilion checkerboard plaza. Behind the plaza,
a dense layered city of convenience stores, utility poles, temple roofs and glass towers climbs
into green mountains. A colossal hollow crescent eye opens above Mount Fuji, and white woodblock
clouds pour down through the eye without covering the central axis. Deep cobalt sky, vermilion
sun, ivory clouds, moss green forest, black ink. Retro Japanese print mixed with hard-edge photo
collage, fine contour lines, slight screen-registration offset, visible paper grain, flat printed
color blocks. Wide-angle frontal perspective, impossible vertical scale, no random decorative
symbols.
```

中文要点：底部通勤者与红毯建立朝圣轴；城市层保持日常可识别；巨眼只执行“打开天空”这个动作。

### 提示词 2：日常显灵

```text
Vertical 9:16 cinematic frame, quiet Japanese suburban street at dusk. Utility poles, low houses,
a roadside vending machine and glossy puddles occupy the lower half; a solitary figure in a long
black coat stands at the left edge and looks into a fog-filled road. Above the fog, an enormous
white celestial sphere begins to rise behind the city skyline while red clouds spread across a
deep ultramarine sky. The puddles reflect the impossible sphere before the sky itself fully reveals
it. Restrained surrealism, flat illustrated texture over photographic detail, slight VHS softness,
hand-printed grain, crisp utility wires. The ordinary street remains believable; only scale,
lighting and reflection are impossible.
```

中文要点：让水洼先泄露异象，天空后完成揭示；普通街道必须可居住。

### 提示词 3：肖像寓言

```text
Vertical 4:5 editorial fashion portrait on a flat cobalt blue background. A young man in a
tailored ivory suit stands in strict profile, holding a dense bouquet of red roses, blue aster
and white chrysanthemums. A red oni mask is fitted directly into the front of his face, overlapping
his skin without floating. Fine ink contours, peach and vermilion skin tones, dense floral detail,
coarse offset-print grain, slight color misregistration. Calm pose, no aggression, one impossible
identity substitution, generous negative space.
```

中文要点：服装、花束和站姿都克制，只保留“脸被鬼面替换”这一处异常。

### 提示词 4：极繁拼贴

```text
Vertical 3:4 psychedelic collage. A serene white-robed oracle stands at the center of a dark
forest, one palm opening a river of blue pixel fragments that floods a night city. Around the
figure, hard-cut fragments of medical anatomy, circuit boards, antique ornaments and small blue
screens showing an eye are pasted together at conflicting perspectives. Vermilion-red beasts and
green mountain silhouettes frame the edge. The figure remains calm and legible; one continuous
luminous axis runs from the raised hand into the distant skyline. Xerox grain, halftone dots,
screen-print misregistration, glossy magazine scraps, black cosmic void.
```

中文要点：中心人物必须平静、可读；所有碎片围绕一条发光轴线工作。

## 通用负面约束

```text
generic neon cyberpunk, seamless glossy CGI, plastic skin, stock-photo realism, blurry subject,
random shrine objects, multiple competing focal points, unreadable clutter, floating symbols with
no spatial effect, excessive tiny text, flat brightness with no black anchor, generic fantasy
landscape, empty city without lived-in objects, anime screenshot copy, watermark
```

负面约束只删除会破坏系统的内容。不要把某一类文化符号整体列入负面，否则会削弱这套视觉能在不同文化场景中转译的能力。

## 系列连续性

一次做 3 张以上时，建立以下四栏：

| 固定项 | 可变项 | 逐张动作 | 禁止漂移 |
| --- | --- | --- | --- |
| 同一观察者服装/轮廓 | 其位置与尺度 | 每张只发现一个新异象 | 人物脸型与服装不能随机变化 |
| 蓝、红、象牙、墨黑主色 | 某一颜色的面积占比 | 从街景逐步推到宇宙 | 不要突然变成粉紫赛博色板 |
| 同一材质组合 | 版画、摄影、数字材料的比例 | 材质碰撞逐张升级 | 不要中途改成无纹理 3D |
| 同一世界规律 | 入口的形式 | 水、门、眼、云各自成为门 | 规则不能只为单张好看而改变 |

最简单的三连作：

1. 观察者站在普通街口；
2. 门槛被发现，异象只进入局部；
3. 镜头拉开，城市整体已处于异象内部。

## 视频生成：单镜头显灵

适用于 6–20 秒竖屏。建议锁定一个主运动，例如缓慢推进。

```text
0.0–3.0s  ESTABLISH
固定中景，人物与街道完整可读。声音只有环境底噪和低频脉动。

3.0–6.0s  SIGNAL
天空或水洼出现单一光点；镜头继续极慢推进。不要让建筑变形。

6.0–10.0s  INTRUSION
光点扩张成巨日/眼睛/神性球体，云层受压，倒影先于现实发亮。

10.0–14.0s  RESPONSE
人物影子、路面、招牌和树叶同时响应。保持人物不动或只转头。

14.0–18.0s  HOLD
让观众看清新空间。镜头可以几乎停止，不用快速环绕。

18.0–20.0s  WITHDRAW
用雾、烟、黑场或声音骤停撤回，不解释异象来源。
```

视频提示词结尾必须写：

```text
one continuous shot, stable subject identity, restrained camera push-in, one surreal reveal,
the real street remains recognizable, no constant morphing, no text, no cutaway
```

## 视频生成：五场景神话漫游

适用于 24–32 秒横屏或方形。每镜 4–6 秒，每个镜头只承担一个叙事动作。

| 镜次 | 时长 | 场景职责 | 镜头 |
| --- | --- | --- | --- |
| 1 | 4–6s | 观察者与住宅/街角 | 横移或静止 |
| 2 | 4–6s | 城市全景显出第二层尺度 | 推进或上摇 |
| 3 | 4–6s | 具体物件与招牌维持现实感 | 缓慢横移 |
| 4 | 4–6s | 门槛出现，异象越过边界 | 固定机位或轻推 |
| 5 | 4–6s | 人与异象共享全局 | 后退或静止 |

镜头间允许硬切或短叠化，但保持同一套天空逻辑、人物服装和材质密度。不要每镜重新设计世界。

## 声音方向

- 静态拼贴视频可用低保真鼓组、模拟合成器底噪、磁带抖动和偶尔的金属敲击。
- 环境片不要铺满旋律。保留电线风鸣、远处车流、便利店冷柜和鞋底水声。
- 异象出现时可让高频短暂消失，留下 1–3 秒低频压迫或空洞静音，再让声音回归。
- 不默认加旁白。若用户要求旁白，让台词只描述人物正在看见什么，不解释象征意义。

## 交付模板

### 图片提示词包

```text
概念：
日常锚点：
异象与动作：
观察者：
构图轴：
色板：
材质：
主提示词：
负面提示词：
可替换变量：
```

### 视频镜头包

```text
概念：
时长/画幅：
世界规则：
角色固定项：
镜头表：时间 | 画面 | 运动 | 异象状态 | 声音
关键帧提示词：
运动提示词：
收尾方式：
连续性风险：
```
