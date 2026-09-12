# Codex 模型与推理强度选择：Luna、Sol、Astra 使用体验与历史成本分析

> 更新时间：2026 年 9 月 13 日
> 阅读说明：第二、三节是最新的个人选择与使用体验；第四至七节保留此前 Luna、Terra、Sol 的评测与成本分析，不包含 Astra，也不代表当前价格或订阅额度换算。
> 楼主主要用 Codex 写 Python 代码、做调研和一些自动化任务，不太涉及网络安全、生物医学等专业领域，也没有足够的超长文本使用经验。如果你的使用场景和楼主相似，这套经验也可以参考；如果不一样，可能还是需要自己评估下哈~

## 一、为什么做这次分析

2026 年 7 月 30 日，GPT-5.6 Luna 降价 80%。楼主之前主要使用 Sol Medium 作为日常模型，这次分析主要验证：降价后的 Luna 能不能替代 Sol Medium，成为日常主力。

此前整理的评测数据来自[GPT-5.6 官方模型介绍页面](https://openai.com/zh-Hans-CN/index/gpt-5-6/)，成本按当时 Luna 降价 80% 后的口径重新计算。9 月 13 日加入 Astra 的使用体验后，楼主更看重额度、智能与完成速度的综合取舍，因此更新了前面的选择建议。后面的旧评测保留作为历史参考，不用于证明 Astra 的效果。

## 二、先给结论

### 按任务类型，在额度、智能与完成速度之间取舍

楼主目前常用 **Luna Max、Sol High 和 Astra Medium（GPT-6）**，可以根据任务直接选择，不用逐级尝试。

| 使用场景 | 楼主倾向的档位 | 主要考虑 |
|---|---|---|
| 简单需求，比较在意额度，可以多等一会儿 | Luna Max | 成本低，很多日常任务都能搞定 |
| 需求明确、有测试和验收机制的工程开发 | Sol High | 工程能力强，体感比 Luna Max 完成任务更快 |
| 方案、机制、架构和 Skill 设计 | Astra Medium | 更容易抓住重点，适合依赖判断力和设计质量的任务 |

**选模型时，楼主现在尤其看重：任务有没有明确的验收标准，能不能通过测试和实际运行来判断结果好不好。** 对于需求明确的复杂开发，楼主也会优先考虑 Sol High；对于难以仅靠测试判断设计质量的任务，更倾向于直接上 Astra Medium。

> 这是个人使用建议，没有做严格的对照测试。下面的速度指完成整个任务的速度，额度消耗和压缩频率也都是使用观察。

## 三、实际体验

### 2026 年 9 月 13 日：三个常用档位的取舍

**Luna Max 省额度，但等待时间更长。** 楼主体感它在这三个常用档位中完成任务最慢，长任务中更容易遇到上下文压缩。简单需求、不着急的任务，用它仍然很合适。最近的体验也让楼主更在意高推理强度带来的等待时间，而不只是看效果和额度。

**Sol High 更适合明确的工程开发。** 相比 Luna Max，楼主体感它完成任务更快，处理复杂问题更稳；同一次上下文中往往能推进更多工作，压缩没那么频繁，任务状态也保持得更好。不过，额度消耗高出不少。这些现象不能直接归因于推理长短，任务本身、工具输出和上下文使用方式也会影响体验。

只要需求明确，有比较完善的测试和验收机制，即使是复杂系统开发，楼主也会优先考虑 Sol High。它像一个很强悍的工程师，适合把具体的事情做出来，再根据验证结果不断修正。

**Astra Medium 更适合依赖判断力的设计工作。** 方案、机制、架构和 Skill 设计，很难仅靠测试通过来保证质量。楼主体感 Astra 更容易理解意图、抓住重点和做出取舍，表达也更精炼；在这些任务里，完成速度比前两个常用档位更快，结果也更合心意。楼主愿意直接用它，争取尽可能少地返工。

它的额度消耗也明显更快，但少量设计工作通常是人与 AI 一起思考的过程：AI 输出后，人要阅读、判断、讨论，再继续推进，总用量不一定很大。这时候，楼主更愿意把额度花在更强的判断力上。

如果打个比方，**Sol 像一个很强悍的工程师，Astra 像一个非常聪明的设计师。** 具体怎么选，还要结合自己的任务、等待时间和额度预算；以上体感不代表所有任务都会有相同结果。

### 2026 年 8 月 6 日：当时的 Luna Max 体验

截至 8 月 6 日，楼主已经连续使用 Luna Max 一周。和 Sol Medium 相比，实际使用时效果上几乎感受不到差异；体感上额度消耗速度可能降低了 80%，日常可以一直开 Fast 使用，性价比实在太高了。

## 四、为什么 Luna Max 能平替 Sol Medium

> **历史分析范围：** 以下第四至七节保留此前的评测数据和成本口径，仅比较 Luna、Terra、Sol，不包含 Astra。评测成本合计不是订阅额度的实测消耗，旧路线也不是 9 月 13 日更新后的日常选择。

在[GPT-5.6 官方基准页面](https://openai.com/zh-Hans-CN/index/gpt-5-6/)的 20 项交互式评测中，主要选取与楼主日常 Python 编码、调研和自动化任务比较接近的 9 项；其余指标放在文末说明，不纳入主比较。

按 Luna 降价 80% 后的成本估算如下：

| 对比 | 胜负情况 | 9 项估算成本合计 |
|---|---:|---:|
| Luna Max vs Sol Medium | Luna Max 胜 5，Sol Medium 胜 3，持平 1 | Luna **$393.63**；Sol Medium **$2,343.77** |

9 项评测中，Luna Max 5 胜、Sol Medium 3 胜、1 平：

- Luna Max 胜在终端和电脑操作、代码与技术任务、知识型工作和自动化：Terminal-Bench（+0.70）、DeepSWE（+6）、GDPval-AA（+30）、OSWorld（+3.36）、AutomationBench（+2.30）。
- Sol Medium 胜在综合智能和浏览检索：Agents’ Last Exam（Sol Medium +1.60）、Artificial Analysis Intelligence Index（Sol Medium +2.35）、BrowseComp（Sol Medium +0.16）。
- Coding Index 持平，都是 74.6。

> **结论：** Luna Max 与 Sol Medium 性能基本持平，两者在 9 项评测中的整体表现接近；Luna 成本低 83%，更具性价比。

## 五、六个档位放在一起看

以下只比较与楼主日常任务相关的 9 项评测。成本按 Luna ×0.2、Terra ×0.8、Sol ×1.0 计算；各个“相对”列都是逐项比较胜负，不是把不同评测分数直接相加。

| 模型 | 9 项降价后成本 | 相对 Luna Max | 相对 Terra xHigh | 相对 Terra Max | 相对 Sol High | 相对 Sol xHigh | 当时的定位 |
|---|---:|---:|---:|---:|---:|---:|---|
| **Luna Max** | **$393.63** | 基准 | 7 胜 2 负 | - | - | - | 日常主力 |
| **Terra xHigh** | **$1,598.01** | 2 胜 7 负 | 基准 | - | - | - | 中间档，不作为主路线 |
| **Terra Max** | **$2,874.31** | 9 胜 0 负 | 9 胜 0 负 | 基准 | - | - | 第一升档 |
| **Sol High** | **$3,311.73** | 8 胜 1 负 | 8 胜 0 负 1 平 | 4 胜 4 负 1 平 | 基准 | - | 中间档，不作为主路线 |
| **Sol xHigh** | **$4,634.45** | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 基准 | 第二升档 |
| **Sol Max** | **$7,194.82** | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 9 胜 0 负 | 8 胜 1 负 | 最终攻坚 |

> **当时按评测筛选的路线：** Luna Max → Terra Max → Sol xHigh → Sol Max。这几个档位在所选指标上能明显拉开差距，但这组比较没有覆盖实际完成速度、压缩频率和 Astra 的表现。

> **当前选择：** 9 月 13 日更新后的个人建议见[第二节](#二先给结论)，常用档位为 Luna Max、Sol High 和 Astra Medium，按任务类型和额度、速度需求选择。

## 六、Luna Max、Terra Max、Sol xHigh、Sol Max 的具体表现

成本按 Luna ×0.2、Terra ×0.8、Sol ×1.0 计算。9 项评测的总成本为：Luna Max **$393.63**、Terra Max **$2,874.31**、Sol xHigh **$4,634.45**、Sol Max **$7,194.82**。

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
