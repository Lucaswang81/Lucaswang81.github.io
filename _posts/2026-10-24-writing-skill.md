---
layout: blog_post
selected: true
title: 学习英文写作原则
date: 2026-10-24
tags:
  - writting
---
TL;DR：该博客总结笔者学习到的英文写作原则和技巧，目的是为了写出有逻辑，结构化的文章或短文来抵抗ai对本人写作的影响。包括：八大写作原则和如何善用AI写作。（AI-Generated Percentage：0%）

Goal：结构清晰，逻辑严密，循序渐进

# 原则一：重要的事情先说
![](https://raw.githubusercontent.com/Lucaswang81/blog-images/main/images/20261025082810340.png)


> 黄色区域为重要信息

**博主曾存在弯弯绕绕，含蓄腼腆的写作习惯**。典型表现为通过冗长铺垫，“山路十八弯”，费尽周折在文章末尾或段落末尾阐述重要结论；一段中存在多个重要观点。

**BLOT：bottom line on top**。为了结构清晰，每一段重要主旨句仅位于段落首句，且一段只能存在一个重要观点，断落剩余内容为对观点的具体阐述或补充说明，当一段想表达两个意思时候请拆成两段。

**让读者阅读体验舒服**。文章内容应考虑读者时间是否充裕，以及认知水平高低。BLOT可以让读者仅通过浏览首段及其他段落首句，花费10%的时间获取70%的观点，使读者清晰得到重要内容，节省时间。

**Self-check 原则**

1. 写完一段话之后问问自己这一段话的主旨是什么，读第一句话是否完整表达了段落主旨

2. 把要展示的文字砍去最后20%，看看要表达的意思是否表达了，然后再砍去 50% 90%，看看要表达的意思是否表达了

**原则可以迁移到阅读领域**。如果社会共识是BLOT，那我们读其他人的文章或论文时也可以通过浏览首段和首句来节省时间，庆幸的是英文文章大多是遵循BLOT的。

# 原则二：分解/分类

![](https://raw.githubusercontent.com/Lucaswang81/blog-images/main/images/20261025082847760.png)

**树状结构与分形**。一篇文章有引导句，每一段落有一个主题句，引导句总结全文，是主题句的主题句。每个主题句由各段落具体内容支撑，可有数个支撑论据。

**多叉树分解写作原则**：开始写文章时，先想好自己的文章要表达什么思想（引导句），之后思考引导句根节点如何分类，也就是找到叶子节点（主题句）支撑，每个主题句扩写一段话（How we get there？包括有意义的数据，案例等）支撑主题句。分类原则尽量做到不重不漏。

**文章最后总结句与引导句呼应**。有头有尾。

# 原则三：连接词

> 一篇文章就像一段旅途，将读者从A点带到B点，道路往往不是笔直前行，常伴有转弯，有刹车，有停顿，这就是连接词。

**连接词分类**

- 对比：however, but, yet, on the other hand, whereas
- 示例：for example, for instance
- 延续：furthermore, moreover,
- 总结：finally, in conclusion, thus, as a result

**八句成文法**

![](https://raw.githubusercontent.com/Lucaswang81/blog-images/main/images/20261025082911619.png)

# 原则四：原子结构

> 案例来自Prof. Fang的分享，理念类似与 VQ-VAE，万事万物都可以被压缩为离散向量，通过拼接后形成完整实体。通过逆向分析文章的原子结构，下次写作可以直接复用结构以提升效率。本小节会结合前三节内容。

**写作分两步**

1. 理清思路：想表达什么观点（引导句），几个子观点（主旨句），每个子观点打算用什么方法论述（how to get there）

2. 原子结构排列组合形成文章，类似乐高

**原子结构分类**

> 可以在阅读论文中构建自己的原子结构，下面是AI总结的深度学习中可以被划分的原子结构

- 分类

- 好处坏处

- 时间顺序

- 对比

- 顺序

- 因果

---

<details>

<summary>写作原子结构在深度学习论文中的体现</summary>

- Categorization（分类）

- Related Work 中对现有方法进行归类梳理，或者 Method 中对模型组成部分/任务场景进行切分。

- Existing approaches to `[Task/Problem]` can be broadly categorized into two streams: `[Category A]`, which `[core mechanism of A]`, and `[Category B]`, which focuses on `[core mechanism of B]`.

- Pros and Cons（好处坏处）

- Introduction 或 Related Work 中指出前人方法的亮点以及随之而来的致命短板，从而引出本文工作。

- While `[Existing Method]` provides the advantage of `[Advantage/Strength]`, it often comes at the cost of `[Limitation/Computational Burden]`, thereby limiting its applicability to `[Challenging Scenario]`.

- 时间顺序（Timeline）

- Introduction 开头陈述技术演进史，展现从传统方法到深度学习再到大模型的发展历程。

- Early attempts predominantly relied on `[Early/Handcrafted Method]`. With the advent of `[Paradigm Shift, e.g., deep learning/Transformers]`, significant progress has been made by `[Modern Solution]`; more recently, however, attention has shifted towards `[Current Trend/New Frontier]`.

- Comparison（对比）

- Experiments / Discussion 中对比自己模型与基线（Baseline），或 Method 中突出核心差异。

- In contrast to existing `[Baseline Paradigm]` that typically `[Baseline limitation/action]`, our proposed `[Method Name]` dynamically `[Our advantage]`, enabling `[Beneficial effect/metric gain]`.

- Pipeline（顺序）

- Method 章节介绍整体架构前向传播流水线（Pipeline / Overview）。

- The overall framework proceeds in `[N]` consecutive stages: first, `[Stage 1]` extracts `[...]`; subsequently, `[Stage 2]` refines `[...]` via `[...]`; finally, `[Stage 3]` projects `[...]` to obtain the final `[Output]`.

- Causality（因果）

- 消融实验（Ablation Study）分析、误差分析（Error Analysis）或 Motivation 解释现象背后原因。

- The superior performance can be primarily attributed to `[Core Innovation/Module]`, which effectively mitigates `[Specific Issue/Bottleneck]`, thereby leading to `[Measurable Improvement]`.

</details>

**原子结构使用原则**

1. 灵活使用，一切是为内容服务

2. 原子结构会逐渐演化

3. 不熟悉的顶级原子结构不如熟练使用的一般原子结构

**使用案例**

> 切记边想边写，通过可视化逻辑线梳理来展现自己的思想更高效

> 可视化案例以Prof. Fang分享为例

![](https://raw.githubusercontent.com/Lucaswang81/blog-images/main/images/20261025082946413.png)

# 原则五：相似性原则

**同一类事情放在一起写**。完成一类事情的讨论之后再进行下一类的讨论，这样读者才可以享受这个阅读旅程，不然会显得很混乱。

<details>

<summary>具体调整示例</summary>

- 调整前

> In 1981, Roger Sperry received the Nobel Price for his proof of the split-brain theory. According to Dr. Sperry, the brain has two hemispheres with different, but over-lapping functions.

>

> The left side of the brain is responsible for analytical, linear, verbal and rational thought. Left-brain thinking is "spotlight" thinking. The right hemisphere is holistic, imaginative, nonverbal and artistic. It is the left brain that a person relies on when balancing a checkbook, remembering names and dates, or setting goals and objectives. Whenever a person recalls another person's face, becomes engrossed in a symphony, or simply daydreams, that person is engaging in right-brain functions. Right-brain thinking is "floodlight" thinking and right-brain processes are, to the chagrin of many, less often rewarded in school. Since most of the Western concepts of thinking come from Greek logic, which is a linear logic system, left-brained processes are most rewarded in the Western education system.

- 调整后

> In 1981, Roger Sperry received the Nobel Price for his proof of the split-brain theory. According to Dr. Sperry, the brain has two hemispheres with different, but over-lapping functions. The right and left hemispheres of the brain each specialize in distinct types of thinking processes. In the most basic sense, the left brain is the analytical side while the right brain is the creative side.

>

> The left side of the brain is responsible for analytical, linear, verbal and rational thought. Left-brain thinking is "spotlight" thinking. It is the left brain that a person relies on when balancing a checkbook, remembering names and dates, or setting goals and objectives. Since most of the Western concepts of thinking come from Greek logic, which is a linear logic system, left-brained processes are most rewarded in the Western education system.

>

> The right hemisphere is holistic, imaginative, nonverbal and artistic. Whenever a person recalls another person's face, becomes engrossed in a symphony, or simply daydreams, that person is engaging in right-brain functions. Right-brain thinking is "floodlight" thinking and right-brain processes are, to the chagrin of many, less often rewarded in school.

</details>

**相似性原则应用尺度**。篇幅较短可以按照上述把左右脑分开阐述，但如果篇幅较长的关于左右脑在各个方面的对比说明文，那么需要权衡考虑，比如下面表格写作时，先总体总结左右脑特征，然后按照下面几个类别分析左右脑 ，第一类为处理信息的类别，左脑一段右脑一段对比功能效果会更好，总之灵活处理，以读者阅读感受为出发点才能写出好文章。

| 对比项 | 左脑 | 右脑 |

| :------- | :- | :- |

| 处理信息类别 | | |

| 处理信息速度 | | |

| 和学校教育的关系 | | |

| 适合什么工作 | | |

| 如何练习 | | |

# 原则六：支持你的观点

Powerful evidence rules

- **Specific**: clearly defined or identified

- **Concrete**: existing in a material or physical form; not abstract

- **Example**: a thing characteristic of its kind or illustrating a general rule

<details>

<summary>具体修改示例</summary>

**Bad example with fine architecture**

> I am applying for the position at your university.

>

> I got my Ph.D. from Stanford University.

>

> After graduation, I joined the University C.

>

> I have developed a few projects, and each project produced several papers.

>

> Moreover, I have gained decent funding for my projects.

>

> I believe that I have built significant momentum to contribute to your institution.

**Support your opinions with powerful evidence**

> I am applying for the position of XX in the **Department of A** at the **B University** with a focus on **fluid mechanics**.

>

> I got my **Ph.D. from Stanford University** in **Civil and Environmental Engineering** with a **Ph.D. Minor in Computational and Mathematical Engineering** in **Spring 2020**.

>

> After graduation, I joined the **University C** as **a tenure-track assistant professor in 2020 Fall**.

>

> Within the **past 2 years as a PI**, I have developed **two independent projects**, and each project produced **x peer-reviewed paper** with my **student**.

>

> Moreover, I have gained more than **$xxx of external support** for one of my projects.

>

> I believe that I have built **significant momentum** for **publication, project development**, and **funding application** as **an early-career faculty**.

</details>

# 原则七：简化你的写作

**保持简单（KISS-Keep it simple and stupid）**。简单常用词汇通常有更宽泛的含义。复杂罕见词汇通常含义更加具体精确。使用简单词降低词不达意的机会，但语言是为了表达和交流思想，并不是为了用复杂词汇炫耀。比如老外学习“棒”是好的意思，使用大棒人就会出现笑柄。

**句子不可过长**。句子长短相间，错落有致，长难句的设计是为了精确表达观点和帮助读者理解概念，出发点从来不是为了考验读者阅读水平。好的长难句设计会符合读者思维习惯，尽管句子结构长难，但理解方面会简单紧凑清晰。所以读到长难句应该开心，作者为了方便你的理解精心设计。

**高效原则**。选择词汇不通过单词中文释义，而是体会原英文单词的意境。句子写完看是否有冗余或重复表达可以删除，是否可以用地道但简单词汇表达同样意思，做到恰到好处少一单词不精准，多一单词冗余的境界。警惕“换句话说”这种表达，尝试在这个短语之前就把思想表达清楚。能用一句话表达清楚就不要用两句话。

**逆向工程**。让ai把已经发表的论文根据初学者表达出来，然后我们对其进行精简

> Here we show that the global self-attention of million-scale image patches—as represented by the Vision Transformer (ViT)—generates dynamic receptive fields that capture long-range semantic dependencies, resulting in an effective inductive bias fundamentally different from the local convolution kernels.

>

> 这是长难句但读起来舒服，如果拆分成多个短句会造成语义逻辑不连贯。

<details>

<summary>具体修改示例</summary>

- The committee decided to **postpone** the meeting ~~to a later date~~ due to **unforeseen circumstances** ~~that arose unexpectedly.~~

- The committee decided to **delay** the meeting because of unexpected events.

---

- ~~The utilization of~~ advanced technology in ~~the implementation of~~ the project will **facilitate** the achievement of the desired **outcomes**.

- **Using** advanced technology in the project will help achieve the desired **results**.

---

- The **proliferation** of digital devices has **significantly augmented** ~~the means by which~~ individuals can communicate ~~with one another~~.

- The **increase** in digital devices has **greatly expanded** how people can communicate.

---

- ~~In the event that~~ you **encounter** any issues, please ~~do not hesitate~~ contact the support team for **assistance**.

- **If** you **have** any issues, please contact the support team for **help**.

---

- It is **imperative** to **utilize** appropriate safety measures to **mitigate** the risk of ~~potential~~ hazards in the ~~workplace~~.

- It is **important** to **use** safety measures to **reduce** the risk of hazards at work.

---

</details>

# 原则八：让你的写作富有变化

1. 名词、动词和形容词三者互换。

2. 变化句子的长短和开头。

- **形容词和名词的互换**

- Chinese is becoming more and more **popular** in the world.

- Chinese is gaining **popularity** in the world.

- **名词和动词的互换**

- Most dietitians **advocate** cutting out fat and reducing carbohydrates as the best means of **losing weight**.

- **According to** most dietitians, dieters should avoid fat and reduce carbohydrates as the best way to achieve **weight loss**.

**变化句子的长短和开头**。主谓宾构成的句子是最常见的。但是如果所有的句子都是单调的主谓宾，则文章非常单调。

如果句子的开头都是用类似的词，比如“I”“We”。文章读起来会味同嚼蜡。

我们可以用7种方法改变每句的开头，让文章丰富起来。

1. 用一个具体的主语

**Researchers** can test a hypothesis via experiments.

2. 用一个短语

**For this reason**, no one knows why we sleep.

3. 用一个从句

**Because** writing is both science and art, students must practice it and get timely feedback.

4. 用一个副词

**Unobservantly**, teachers may assume that students all can learn by teaching them once.

5. 用一个形容词

**Intelligent and passionate**, we start the path to improve our writing skills.

6. 用一个动名词

**Allowing plenty of time and based on correct principles**, we can all become writing masters.

7. 用一个不定式

**To be a professor**, one must have a Ph.D. degree.

# AI 辅助写作

## Prompt Engineering

**目标**：合理设计并编写提示词实现高效率，准确，可控，适应不同任务和场景，实现和机器的有效交流。

**哲学**：GIGO，输出水平会匹配输入认知水平，人们之间的差距不会因llm出现而消除。更加稳固的信息茧房可能是llm适应普通人的认知水平而让他失去了提升认知水平的能力。

**提示词基本格式**：

```text

- Play a role.

- Instruction - a specific task or instruction you want the model to perform

- Context - can involve external information or additional context that can steer the model to better responses

- Input Data - is the input or question that we are interested to find a response for

- Output Indicator - indicates the type or format of the output.

```

Enter之前如果没有觉察到自己在干什么将会是无效prompt，虽然我们可以在此纠正，不过模型思考的时间还有我们阅读的时候会是低效的。所以prompt也需要冥想，不然自动驾驶模型很糟糕。

interesting ideas

- tell me a trivial fact about something few people know about

- Provide me with a trivial fact on astronomy that is simple to explain but fascinating

- so you can find some few fact in an area but difficult to find

## 提示词语气

**提示语气与认知影响输出语气和认知**。输出匹配输入，原因在于注意力机制计算了输入的语气词和认知水平匹配，所以当我们想获得某种答案，不仅要让gpt模仿对应的人物，我们也应该模仿对应的提示语气和认知。

统计数据表明，人的智商呈现正态分布，但AI的输出取决于用户的智商啊，一个人的智商并不会被ai提高，且对于大多数人来说ai是一种迫害，ai只是在缩短达到目的的时间，是否真正有提高人的能力有待讨论。如果仅用ai帮助节省时间，那么我们并不会成长还会退步，用于提升自身认知水平才是提升，不然就是退步。

延迟满足被摧毁，思考深度

脑海中一定要预演ai可能会输出什么，不然就是浪费时间去读垃圾，这种能力也来自于对自身状态的觉察

顽皮

学术

技术

llm匹配身份输出

输入之前直接预演 gpt 会回答什么

socrates辩证法深度思考

头脑风暴正方反方

你是一个在流体力学最领先权威的教授，有着写30年proposal的经验，而且成功率非常高，比如说你申请上了，NFS，

先梳理逻辑

给gpt明确的消息，字数，内容分点，水平PHD

先要有逻辑思路，然后再问，不然就会被ai带着走

做一个大项目之前，先用思维导图列出要进行的内容，有逻辑有条理，refine方案之后行动