---
tags: [agent]
categories: [Cases]
description: 尝试从医学相关benchmark自行制作agent。
---

斯坦福大学做的一个benchmark, 链接：[PhysicianBench](https://healthrex.github.io/PhysicianBench/)

最初的计划是自己做一个agent，官方对自己设置的miniagent给出了很少的限制，基本只是不断的调用工具循环，并把所有信息塞在上下文里面。计划是想比miniagent表现更好。但事实上增加结构和设计并不一定意味着更好的表现，最开始大量的路径被控制验证截断，导致压根没跑完。后续不同版本在试图修复上一个版本的问题的同时，自己本身又引入了新的问题。再后续尝试从头设计一个简化的结构，并总结一番这里暴露的问题和经验，尝试用到[WalkingMinion]({% link _posts/2026-10-22-minion.md %})里面。

