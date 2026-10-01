# Codex 模型与推理强度选择：三个推荐档位

> 更新时间：2026 年 10 月 1 日

## 一、三个推荐档位

楼主主要用 Codex 写代码、做调研和自动化任务，目前按任务直接选择以下三个档位，不用逐级尝试。

| 模型档位 | 雷达 IQ | 推荐用途 |
|---|---|---|
| GPT-5.6 Luna Max | 100 | 简单需求，优先节省额度 |
| GPT-6.1 Sol High | 暂无分数 | 需求明确、有测试和验收机制的工程开发 |
| GPT-6 Astra Medium | 117 | 最强档位，用于方案、机制、架构和 Skill 设计 |

IQ 参考 [Codex Radar](https://codexradar.com/) 的综合智能评分，记录于 2026 年 10 月 1 日，随众测更新。

**不推荐 GPT-6 Luna：** Max 档的雷达 IQ 只有 82，楼主使用下来也觉得效果较差，省额度仍推荐 GPT-5.6 Luna Max。

## 二、Sol High 的判断依据

从楼主的[鹈鹕测试](model-quality-check.md#三如何检测降智)看，GPT-6.1 Sol High 的生成效果比较接近 GPT-6 Astra Medium。雷达暂未给出 GPT-6.1 Sol High 的分数，楼主估计其 IQ 高于 GPT-6 Sol High（103），目前把它作为工程开发的主力档位。

需求明确、能通过测试验收的任务，优先用 Sol High；更依赖判断力、需要权衡方案的工作，直接用 Astra Medium。

## 三、快速切换档位（macOS）

楼主的开源工具 **[Codex Model Slider（中文说明）](https://github.com/cabbagecabbage/codex-model-slider/blob/main/README.zh-CN.md)**，把常用模型与推理强度放进三档滑块，拖一下就能同时切换。

[一行安装到桌面，以后双击启动 →](https://github.com/cabbagecabbage/codex-model-slider/blob/main/README.zh-CN.md#快速使用)
