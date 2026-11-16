# 神话城市拼贴

一个从 43 张竖幅视觉作品与 2 段动态研究中蒸馏出的 Codex 技能。它不从象征物清单出发，而是把参考图真正稳定的**压缩色调、舞台式空间、受控细节密度和印刷/数字材质断裂**转成可执行的创作流程、图像提示词、修复方法、短视频分镜与验收标准。

`v1.2.0` 用 cangjie-skill 的 RIA-TV++ 流程重新蒸馏 43 张静态图与 2 段动态样本：完成五路候选提取、三重验证、单入口路由、九张 R/I/A1/A2/E/B 能力卡、共享术语和边界测试。此前 `v1.1.0` 已把重心从素材词典转向色调、构图、细节密度与整体风格。

## 能做什么

- 根据情绪张力选择六种构图骨架，而不是先收集神话符号
- 用承重色、过渡色、事件色控制和统一参考图的色调气质
- 将高密细节组织成“岛”，避免均匀噪点与素材仓库
- 生成孤立图腾、轴线登临、全景游行、正面祭坛、超近景切片和框中世界提示词
- 设计 6–20 秒单镜头显形或 24–32 秒多场景漫游
- 按可量化标准修复“元素拼贴、彩虹化、三维游戏感、贴纸化、整体失焦”等问题
- 按需加载视觉命题、构图、色调、空间、细节、材质、提示词、诊断或系列能力卡
- 用缩略图、灰度、去名词、颗粒连续性和缺输入场景进行边界测试

## 安装

把整个 `mythic-city-collage` 文件夹放入 Codex 技能目录：

```text
$CODEX_HOME/skills/mythic-city-collage
```

未设置 `CODEX_HOME` 时，通常使用：

```text
~/.codex/skills/mythic-city-collage
```

## 调用示例

```text
用 $mythic-city-collage 把“凌晨两点便利店门口的等待”做成一套三连主视觉。
```

```text
用 $mythic-city-collage 写一个 12 秒竖屏视频方案：雨后的高架桥、一个抽烟的人、逐渐升起的巨大白日前，以及水洼里的第二层城市。
```

## 文件

- `SKILL.md`：视觉识别点、构图选择、工作流与反拼贴约束
- `references/style-grammar.md`：色调、构图、细节、线面、材质与整体风格分析
- `references/production-recipes.md`：视觉命题、五类图像配方、改图、系列和视频模板
- `references/quality-rubric.md`：静态/动态评分、五种盲测与按层级修复方法
- `references/capability-index.md`：9 个能力的完整意图/关键词路由
- `references/capabilities/`：按需加载的 R/I/A1/A2/E/B 深层能力卡
- `references/cheatsheet.md`：九条决策规则速查
- `references/glossary.md`：共享视觉术语
- `references/overview.md`：蒸馏来源、骨架、批判与边界
- `references/digest.md`：面向读者的视觉语法精华
- `test-prompts.json`：darwin 兼容的触发与边界用例
- `test-results.md`：fallback 自测、输出断言与未完成项

## 边界

这个仓库发布的是提炼后的方法，不包含原始参考图片或视频。它不用于复制某位创作者的既有作品，也不用于普通旅行摄影、常规霓虹赛博朋克或只做素材摘要的请求。
