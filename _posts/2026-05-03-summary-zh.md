---
layout: default
title: "Horizon Summary: 2026-05-03 (ZH)"
date: 2026-05-03
lang: zh
---

> From 21 items, 5 important content pieces were selected

---

1. [NASA 阿尔忒弥斯二号任务激光通信成功从月球传回 484 GB 数据](#item-1) ⭐️ 9.0/10
2. [Mercury 的几百万行 Haskell 代码](#item-2) ⭐️ 8.0/10
3. [Dav2d 作为最快的 AV2 解码器的介绍](#item-3) ⭐️ 8.0/10
4. [VS Code 自动将 'Co-Authored-by Copilot' 添加到提交中](#item-4) ⭐️ 8.0/10
5. [DeepSeek-V4 预览版正式上线并开源，增强了 Agent 能力](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [NASA 阿尔忒弥斯二号任务激光通信成功从月球传回 484 GB 数据](https://dailygalaxy.com/2026/05/nasa-just-beamed-484-gigabytes-from-moon/) ⭐️ 9.0/10

NASA 在阿尔忒弥斯二号任务中，利用激光通信系统 O2O 从月球成功传回 484 GB 数据，下行速率达 260 Mbps，远超传统射频。 这一成就标志着激光通信技术在太空探索中的重大进展，可能会彻底改变未来的月球和火星任务。近实时分析和公众观看高质量视频的能力将增强科学合作和公众参与。 O2O 系统由 MIT 林肯实验室开发，允许高带宽通信，使科学家几乎实时分析高清图像。参与该项目的地面站包括喷气推进实验室和澳大利亚国立大学的斯特罗姆洛山天文台。

telegram · zaihuapd · May 3, 00:50

**背景**: 太空中的激光通信利用红外光进行数据传输，相比传统的无线电波提供更高的带宽。这项技术对未来的太空任务至关重要，因为它允许在更短的时间内传输更多的数据，这对于实时通信是必不可少的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nasa.gov/goddard/esc/o2o/">Exploration and Space Communications: LEMNOS - NASA</a></li>
<li><a href="https://www.scientificamerican.com/article/nasas-artemis-ii-laser-communications-system-is-beaming-4k-video-from-the/">NASA’s Artemis II laser communications system is beaming 4K ...</a></li>
<li><a href="https://abcnews.com/Technology/lasers-world-watch-artemis-ii-astronauts-travel-moon/story?id=129781981">Lasers could allow the world to watch Artemis II astronauts ...</a></li>

</ul>
</details>

**标签**: `#NASA`, `#Artemis II`, `#laser communication`, `#space exploration`, `#data transmission`

---

<a id="item-2"></a>
## [Mercury 的几百万行 Haskell 代码](https://blog.haskell.org/a-couple-million-lines-of-haskell/) ⭐️ 8.0/10

这篇文章讨论了 Mercury 在生产工程中使用 Haskell 的情况，详细介绍了他们如何管理大约两百万行的代码库。它突出了团队在实施 Haskell 以满足金融科技解决方案时面临的优势和挑战。 这很重要，因为它展示了 Haskell 在真实生产环境中的能力，特别是在金融科技行业，这可能会影响其他考虑在项目中使用 Haskell 的公司。社区分享的见解也反映了编程语言采用和生产力的更广泛趋势。 文章指出，Haskell 强大的类型系统有助于防止错误，但也提到该语言可能难以掌握，导致开发者之间的生产力水平差异。此外，社区评论表明，尽管 Haskell 有独特的优势，但像 Rust 这样的其他语言可能为某些开发者提供更好的生产力。

hackernews · unignorant · May 3, 00:01

**背景**: Haskell 是一种静态类型、纯函数式编程语言，以其强大的类型系统和惰性求值而闻名。它通常用于对可靠性和可维护性要求严格的行业，如金融和电信。Mercury 是一家金融科技公司，已将 Haskell 用于其后端系统，为大量企业提供服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.haskell.org/a-couple-million-lines-of-haskell/">A Couple Million Lines of Haskell : Production Engineering at Mercury</a></li>
<li><a href="https://serokell.io/blog/haskell-in-production-caribou">Haskell in Production : Caribou</a></li>
<li><a href="https://en.wikipedia.org/wiki/Haskell">Haskell - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了对 Haskell 在生产中使用的热情与谨慎。一些用户欣赏该语言的优势，而另一些用户则对其复杂性和与 Rust 等其他语言相比的生产力表示担忧。

**标签**: `#Haskell`, `#Software Engineering`, `#Production Engineering`, `#Programming Languages`, `#Community Discussion`

---

<a id="item-3"></a>
## [Dav2d 作为最快的 AV2 解码器的介绍](https://code.videolan.org/videolan/dav2d) ⭐️ 8.0/10

Dav2d 被介绍为最快的 AV2 解码器，显著提高了视频压缩效率和流媒体应用的性能。这个新解码器旨在在所有平台上都小巧、便携且非常快速。 这一发展具有重要意义，因为它承诺提高流媒体效率，可能使内容提供商和消费者都受益。Dav2d 的推出可能会促进 AV2 的采用，而 AV2 预计将优于其前身 AV1。 Dav2d 作为一个跨平台解码器正在开发，重点关注正确性和针对各种架构（包括 x86、ARM 和 RISC-V）的性能优化。该项目仍在进行中，计划进行进一步的性能提升。

hackernews · dabinat · May 2, 17:32

**背景**: AV2 是由开放媒体联盟开发的下一代视频编码规范，旨在提供比 AV1 更好的压缩性能。AV2 的开发始于 2020 年，旨在支持以更低比特率传输高质量视频，使其适合现代流媒体需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://videocardz.com/newz/videolan-publishes-dav2d-an-early-cpu-decoder-for-av2-video-codec">VideoLAN publishes dav2d, an early CPU decoder for AV2 video codec - VideoCardz.com</a></li>
<li><a href="https://www.phoronix.com/news/Dav2d-Open-Source-AV2-Decode">VideoLAN Publishes Dav2d For Open-Source AV2 Decoder - Phoronix</a></li>
<li><a href="https://en.wikipedia.org/wiki/AV2_(video_coding_format)">AV2 (video coding format)</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了对 Dav2d 性能的兴奋以及它在 AV2 采用中的潜在作用，类似于 Dav1d 对 AV1 的影响。一些用户对未来将补充此解码器的编码器表示期待。

**标签**: `#AV2`, `#video coding`, `#streaming`, `#decoding`, `#performance`

---

<a id="item-4"></a>
## [VS Code 自动将 'Co-Authored-by Copilot' 添加到提交中](https://github.com/microsoft/vscode/pull/310226) ⭐️ 8.0/10

VS Code 中的新功能自动将 'Co-Authored-by Copilot' 插入提交信息，无论是否实际使用了 Copilot。此变化引发了关于作者身份和人工智能伦理的重大争议。 此功能引发了关于代码作者身份完整性和人工智能在软件开发中角色的重要伦理问题。这可能会影响开发者对工具的信任以及提交历史的真实性。 该功能在没有充分验证的情况下实施，导致人们对其默认激活表示担忧。此外，代码库中关于该功能行为存在不一致性。

hackernews · indrora · May 2, 19:57

**背景**: 在 Git 中，'Co-Authored-by' 尾部允许多个作者被记入提交，这对协作至关重要。人工智能在软件开发中的伦理影响正受到越来越多的审视，尤其是在透明度和问责制方面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors">Creating a commit with multiple authors - GitHub Docs</a></li>
<li><a href="https://codewave.com/insights/ethical-issues-ai-software-development/">What Are the Ethical Issues for AI in Software Development? -</a></li>

</ul>
</details>

**社区讨论**: 社区成员对该功能的伦理影响表示强烈担忧，有人将其与误导性的营销行为进行比较。其他人强调在实施此类更改之前需要更好的验证。

**标签**: `#VS Code`, `#AI Ethics`, `#Software Development`, `#Community Discussion`, `#Git`

---

<a id="item-5"></a>
## [DeepSeek-V4 预览版正式上线并开源，增强了 Agent 能力](https://t.me/zaihuapd/41185) ⭐️ 8.0/10

DeepSeek-V4 的预览版本正式上线并同步开源，相比前代模型，Agent 能力显著增强。DeepSeek-V4-Pro 在多项评测中超越了所有现有的开源模型。 这一发布具有重要意义，因为它为 AI/ML 社区提供了一种经济高效的替代方案，可能会对现有模型造成冲击。它可能会影响开源 AI 技术的发展和采用。 DeepSeek-V4-Pro 拥有 1.6 万亿参数（激活 490 亿），而 DeepSeek-V4-Flash 拥有 2840 亿参数（激活 130 亿），均支持一百万个令牌的上下文长度。这些模型旨在提供更快和更经济的 API 服务。

telegram · zaihuapd · May 3, 02:21

**背景**: DeepSeek 是一家开发大型语言模型的中国 AI 公司，以其经济高效的训练方法而受到关注。该公司成功创建了与行业知名企业竞争的模型，特别是在其开源方法方面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash · Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI`, `#Machine Learning`, `#Open Source`, `#Deep Learning`, `#Model Performance`

---