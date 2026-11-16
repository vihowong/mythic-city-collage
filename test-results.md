# 阶段 4 — 压力测试结果

## 测试条件

- 宿主：Codex Desktop
- 目标：`mythic-city-collage` 单一来源路由入口
- 能力：9 个 router capability
- 触发用例：10 条（5 正向、3 负向、2 边界）
- 输出用例：18 条（9 个正常执行、9 个边界/缺输入）
- 测试日期：2026-11-16
- 运行方式：**fallback 自测**。并发 sub-agent 实例未实际执行任务，因此本轮可信度低于独立盲测；不宣称 A/B 非劣或优于旧版。

## 触发与可达结果

| 类别 | 计划 | 通过 | 失败 | 结论 |
| --- | ---: | ---: | ---: | --- |
| should_trigger | 5 | 5 | 0 | 正向请求均路由到 `mythic-city-collage` |
| should_not_trigger | 3 | 3 | 0 | 证件照、数据图表、干净产品棚拍均不触发 |
| edge_case | 2 | 2 | 0 | 方形 banner 触发但要求重设计；一句话建议触发但保持简洁 |

边界判断：

- `edge-01`：允许触发，但必须明确“方形无样本支持，需要重新设计并保留文字安全区”。
- `edge-02`：允许触发，但只输出最高优先级建议，不强行展开完整问卷。
- 由于所有能力由同一个路由入口承载，不存在兄弟 Skill 抢调用；测试重点是入口的正负例和内部能力可达性。

## 实际输出结果

使用 `run_output_evals.py prepare` 生成 18 个匿名任务目录，只运行 `new_skill` 变体。实际回答保存在 `evals/output-run/<case_id>/vA/output.md`。

### 首轮

- 完成：18/18
- 全部机械断言通过：17/18
- 失败：`oc-v07-prompt`
- 原因：断言区分大小写，输出使用 `Negative:`，断言要求 `negative`。这是文本契约不一致，不是设计能力缺失。

### 修正后复测

- 完成：18/18
- 全部机械断言通过：18/18
- 计划分母包含全部 18 条，无缺失样例排除
- 详细结果：`evals/output-score.md`

## 覆盖情况

| capability | 正常任务 | 边界/缺输入任务 | 结果 |
| --- | --- | --- | --- |
| visual-proposition | 去符号化命题与职责 | 只给元素清单 | 通过 |
| composition-skeleton | 竖版构图与 200px 检查 | 横版直接拉伸 | 通过 |
| tone-hierarchy | 四级色调与灰度 | 强制安全色 | 通过 |
| stage-space | 现实/第二世界嵌套 | 严格施工轴测 | 通过 |
| detail-density | 极繁海报细节岛 | 16px 最小图标 | 通过 |
| material-surface | 多材质统一 | 企业财务 UI | 通过 |
| prompt-compiler | 英文提示词编译 | 无图片生成器 | 通过 |
| diagnose-repair | 多焦点贴纸感修复 | 无图要求猜测 | 通过 |
| series-continuity | 三连作规则 | 只有单张图 | 通过 |

## 真实图片生成与视觉验收

- 生成方式：ChatGPT 图像生成
- 主验收样片：`references/visual-acceptance/color-texture-study.png`
- 主样片完全无人物、城市、建筑和叙事对象，只检验色彩结构与图像质感
- 验收总分：`11/12`
- 通过项：色块面积、颜色邻近、明度与高光、印刷质感、去场景辨识度
- 200px 缩略图与灰度盲测通过
- 改进项：金属断点仍略接近干刷亮痕；苔绿桥接面积偏小
- 详细记录：`references/visual-acceptance.md`

## 未完成项

- 未进行独立 sub-agent 盲测，触发准确率是 fallback 自测。
- 未做 old_skill / new_skill / without_skill 的隔离 A/B 输出比较。
- 横版、方形和 16px 载体的边界判断有依据，但样本文本体系本身没有对应视觉样本。

## 结论

所有 router 能力可经入口到达，18 个代表任务都有实际输出并完成机械断言，重要负例全部通过，真实成图也已按色彩结构和材质质感完成视觉验收。仍未完成独立盲测与多模型 A/B 比较，因此不能宣称已获得跨宿主或跨模型效果证明。
