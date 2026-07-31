# Codex 模型与推理强度选择：Luna、Terra、Sol 成本与实测分析

> 更新时间：2026 年 7 月 31 日
> 适用背景：GPT-5.6 Luna 于 2026 年 7 月 30 日降价后
> 楼主主要用 Codex 写 Python 代码、做调研和一些自动化任务，不太涉及网络安全、生物医学等专业领域，也没有足够的超长文本使用经验。如果你的使用场景和楼主相似，这套经验也可以参考；如果不一样，可能还是需要自己评估下哈~

## 一、为什么做这次分析

2026 年 7 月 30 日，GPT-5.6 Luna 降价 80%。楼主之前主要使用 Sol Medium 作为日常模型，这次分析主要验证：降价后的 Luna 能不能替代 Sol Medium，成为日常主力。

本文数据来自[GPT-5.6 官方模型介绍页面](https://openai.com/zh-Hans-CN/index/gpt-5-6/)。该页面展示的是降价前的成本，本文已按 Luna 降价 80% 后重新计算。

## 二、先给结论

### Luna Max 可以替代 Sol Medium 作为日常主力

本文使用的评测数据均来自 OpenAI 官方页面，主要筛选与楼主日常的 Python 编码、调研和自动化任务比较接近的 9 项指标。按这 9 项汇总，Luna Max 与 Sol Medium 的整体表现接近，而降价后成本低 83%。

楼主之所以选择 Luna Max 作为日常主力，是因为正常使用 Luna Max 额度基本用不完，也没什么必要降低推理强度了。

楼主目前的选择是：

```text
Luna Max（日常主力） → Terra Max（第一升档） → Sol xHigh（第二升档） → Sol Max（最终攻坚）
```

## 三、实际体验

7 月 31 日实际使用 Luna Max 一天后，明显感觉它更省额度；但也更容易触发上下文压缩，可能是因为它思考得更多、过程更长。目前还没有明显感觉到“频繁压缩导致质量下降”，后续继续观察。不过从个人直觉来看，频繁压缩不是一个好的信号。

## 四、为什么 Luna Max 能平替 Sol Medium

在[GPT-5.6 官方基准页面](https://openai.com/zh-Hans-CN/index/gpt-5-6/)的 20 项交互式评测中，主要选取与楼主日常 Python 编码、调研和自动化任务比较接近的 9 项；其余指标放在文末说明，不纳入主比较。

按 Luna 降价 80% 后的成本估算如下：

| 对比 | 胜负情况 | 9 项估算成本合计 |
|---|---:|---:|
| Luna Max vs Sol Medium | Luna Max 胜 5，Sol Medium 胜 3，持平 1 | Luna **$393.63**；Sol Medium **$2,343.77** |

9 项评测中，Luna Max 5 胜、Sol Medium 3 胜、1 平：

- Luna Max 胜在终端和电脑操作、代码与技术任务、知识型工作和自动化：Terminal-Bench（+0.70）、DeepSWE（+6）、GDPval-AA（+30）、OSWorld（+3.36）、AutomationBench（+2.30）。
- Sol Medium 胜在综合智能和浏览检索：Agents’ Last Exam（Sol Medium +1.60）、Artificial Analysis Intelligence Index（Sol Medium +2.35）、BrowseComp（Sol Medium +0.16）。
- Coding Index 持平，都是 74.6。

> **结论：**Luna Max 与 Sol Medium 性能基本持平，两者在 9 项评测中的整体表现接近；Luna 成本低 83%，更具性价比。

## 五、六个档位放在一起看

以下只比较与楼主日常任务相关的 9 项评测。成本按 Luna ×0.2、Terra ×0.8、Sol ×1.0 计算；各个“相对”列都是逐项比较胜负，不是把不同评测分数直接相加。

| 模型 | 9 项降价后成本 | 相对 Luna Max | 相对 Terra xHigh | 相对 Terra Max | 相对 Sol High | 相对 Sol xHigh | 定位 |
|---|---:|---:|---:|---:|---:|---:|---|
| **Luna Max** | **$393.63** | 基准 | 7 胜 2 负 | - | - | - | 日常主力 |
| **Terra xHigh** | **$1,598.01** | 2 胜 7 负 | 基准 | - | - | - | 中间档，不作为主路线 |
| **Terra Max** | **$2,874.30** | 9 胜 0 负 | 9 胜 0 负 | 基准 | - | - | 第一升档 |
| **Sol High** | **$3,311.73** | 8 胜 1 负 | 8 胜 0 负 1 平 | 4 胜 4 负 1 平 | 基准 | - | 中间档，不作为主路线 |
| **Sol xHigh** | **$4,634.45** | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 基准 | 第二升档 |
| **Sol Max** | **$7,194.82** | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 8 胜 1 负 | 最终攻坚 |

> **升级路线：**从这张表基本可以确定，Luna Max → Terra Max → Sol xHigh → Sol Max。这几个档位在指标上能明显拉开差距；其他几个模型 x 推理强度组合作为升级档的意义不大。

> **实际使用：**不必机械升档：你感觉 Luna 搞不定的（用多了你会有感觉），或者实际使用确实搞不定的，直接上 Terra Max、Sol xHigh 或 Sol Max。

## 六、Luna Max、Terra Max、Sol xHigh、Sol Max 的具体表现

成本按 Luna ×0.2、Terra ×0.8、Sol ×1.0 计算。9 项评测的总成本为：Luna Max **$393.63**、Terra Max **$2,874.30**、Sol xHigh **$4,634.45**、Sol Max **$7,194.82**。

每个单元格为“得分 / 降价后估算成本”，成本单位为美元。

| 类别 | 基准 | Luna Max | Terra Max | Sol xHigh | Sol Max |
|---|---|---:|---:|---:|---:|
| 专业智能体 | Agents’ Last Exam | 50.3 / $85.80 | 50.4 / $435.20 | 53.6 / $763.00 | 52.7 / $1,087.00 |
| 综合智能 | Artificial Analysis Intelligence Index v4.1 | 51.24 / $175.19 | 54.95 / $1,412.91 | 57.65 / $1,557.81 | 58.89 / $2,839.42 |
| 编码智能体 | Artificial Analysis Coding Index | 74.6 / $107.48 | 77.4 / $753.38 | 78.7 / $1,816.62 | 80 / $2,454.95 |
| 终端与命令行 | Terminal-Bench 2.1 | 82.5 / $0.13 | 84.3 / $0.78 | 84.9 / $1.33 | 88.8 / $1.72 |
| 代码库工程 | DeepSWE v1.1 | 67 / $0.60 | 70 / $4.00 | 71 / $5.00 | 73 / $9.00 |
| 网页浏览与调研 | BrowseComp | 83.25 / $0.28 | 87.52 / $2.50 | 88.78 / $4.59 | 90.36 / $6.36 |
| 知识型工作 | GDPval-AA v2 | 1592 / $22.49 | 1593 / $253.34 | 1702 / $465.11 | 1748 / $768.57 |
| 电脑操作 | OSWorld 2.0 | 45.57 / $1.56 | 50.2 / $11.74 | 55.82 / $20.19 | 62.57 / $26.62 |
| 工具与自动化 | AutomationBench | 14.9 / $0.10 | 15.2 / $0.46 | 17 / $0.80 | 18.1 / $1.18 |

## 七、20 个评测指标分别是什么

下面的 20 项，指本次从[GPT-5.6 官方页面](https://openai.com/zh-Hans-CN/index/gpt-5-6/)整理出的 20 个交互式评测图表。主分析只选择前 9 项，因为它们与楼主日常的 Python 编码、调研和自动化任务更接近。官网另外列出的长上下文、多模态和学术等静态评测，不在这 20 项的统计范围内。

<table>
<thead>
<tr><th>类别 / 主要测什么</th><th>评测指标</th><th>本次处理</th></tr>
</thead>
<tbody>
<tr>
<td rowspan="2">专业智能与综合能力</td>
<td>Agents’ Last Exam<br><small>跨专业领域的长周期智能体工作流</small></td>
<td>纳入：对应复杂调研和多步骤任务</td>
</tr>
<tr>
<td>Artificial Analysis Intelligence Index v4.1<br><small>智能体、编程、科学推理和通用能力的综合指数</small></td>
<td>纳入：作为整体能力参考</td>
</tr>
<tr>
<td rowspan="3">编码与软件工程</td>
<td>Artificial Analysis Coding Index<br><small>编程智能体的功能实现、终端操作和真实代码库能力</small></td>
<td>纳入：对应 Python 编码</td>
</tr>
<tr>
<td>Terminal-Bench 2.1<br><small>复杂命令行和终端工作流</small></td>
<td>纳入：对应 Codex 终端操作</td>
</tr>
<tr>
<td>DeepSWE v1.1<br><small>真实代码库中的长周期软件工程任务</small></td>
<td>纳入：对应复杂代码修改和调试</td>
</tr>
<tr>
<td rowspan="2">网页调研与知识工作</td>
<td>BrowseComp<br><small>智能体网页浏览和信息检索</small></td>
<td>纳入：对应网页调研</td>
</tr>
<tr>
<td>GDPval-AA v2<br><small>专业知识型工作的综合表现</small></td>
<td>纳入：对应资料整理和知识工作</td>
</tr>
<tr>
<td rowspan="2">电脑操作与自动化</td>
<td>OSWorld 2.0<br><small>电脑操作和跨应用的多步骤任务</small></td>
<td>纳入：对应电脑自动化</td>
</tr>
<tr>
<td>AutomationBench<br><small>工具调用和自动化任务</small></td>
<td>纳入：对应自动化工作流</td>
</tr>
<tr>
<td rowspan="4">网络安全</td>
<td>ExploitBench<br><small>从漏洞代码到可执行利用的网络安全任务</small></td>
<td>不纳入：楼主不做网络安全</td>
</tr>
<tr>
<td>ExploitGym<br><small>在时间限制下完成真实漏洞利用</small></td>
<td>不纳入：楼主不做网络安全</td>
</tr>
<tr>
<td>SEC-Bench Pro<br><small>软件漏洞概念验证代码生成</small></td>
<td>不纳入：楼主不做网络安全</td>
</tr>
<tr>
<td>夺旗（CTF）<br><small>夺旗类网络安全挑战</small></td>
<td>不纳入：楼主不做网络安全</td>
</tr>
<tr>
<td rowspan="3">生命科学</td>
<td>GeneBench Pro<br><small>基因组学和定量生物学分析</small></td>
<td>不纳入：楼主不做生物医学</td>
</tr>
<tr>
<td>LifeSciBench<br><small>生命科学研究任务</small></td>
<td>不纳入：楼主不做生物医学</td>
</tr>
<tr>
<td>MedChemBench<br><small>药物化学和化学研究任务</small></td>
<td>不纳入：楼主不做生物医学</td>
</tr>
<tr>
<td rowspan="4">AI 研究与系统优化</td>
<td>RSI Index<br><small>递归自我优化和 AI 研究能力</small></td>
<td>不纳入：属于 AI 研究场景</td>
</tr>
<tr>
<td>内部研究调试评估<br><small>研究系统调试、训练方案和模型实验优化</small></td>
<td>不纳入：属于 AI 研究场景</td>
</tr>
<tr>
<td>KernelGen 1P<br><small>底层计算内核生成和优化</small></td>
<td>不纳入：不是普通 Python 开发</td>
</tr>
<tr>
<td>NanoGPT<br><small>小型语言模型训练和优化</small></td>
<td>不纳入：不是楼主的日常任务</td>
</tr>
</tbody>
</table>

因此，9 项不是“所有用户都应该看的固定答案”，而是根据楼主的使用场景筛出来的：编码看 Coding、Terminal、DeepSWE；调研看 BrowseComp、Agents’ Last Exam、GDPval；自动化看 OSWorld、AutomationBench，再用综合智能指数做整体校验。

## 参考资料

- [GPT-5.6 官方基准与模型介绍](https://openai.com/zh-Hans-CN/index/gpt-5-6/)
- [OpenAI：GPT-5.6 降价与用量计算说明](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/)
