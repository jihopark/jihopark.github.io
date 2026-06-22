---
layout: post
title: Learning to learn
tags: [llm-products]

---

Last month, I wrote about [building intuition and taste](/2026/01/19/building-intuition-and-taste/) and wondered how new programmers can develop these skills when AI can handle the details for them.

I didn't have an answer. But now there's some data.

Anthropic just published a [randomized controlled trial](https://www.anthropic.com/research/AI-assistance-coding-skills) studying how AI assistance affects skill formation. They gave junior developers a task to learn a new Python library (Trio) - half with AI assistance, half without. Then everyone took a quiz.

The results were striking: developers who used AI scored 50% on average. Those without AI? 67%. That's nearly two letter grades of difference.

But here's what's interesting. The AI group wasn't actually faster. On average, completion time was about the same. So they didn't gain speed, and they learned less. Worst of both worlds.

--

Reading through the paper, I found myself nodding along - this matched my intuition about how skills are built through friction, not shortcuts. But then I got to the qualitative analysis, and things got more nuanced.

The researchers watched screen recordings of every participant and identified six distinct patterns of how people used AI. Three patterns led to poor learning outcomes (24-39% quiz scores). Three led to surprisingly good ones (65-86%).

The low scorers? They delegated everything to AI, progressively relied more on it, or used it as an iterative debugging crutch. This is the kind of behavior I experienced when I have low energy & motivation level, as mentioned in my previous post, [Useful principles for using AI coding tools](https://me.jiho-ml.com/2025/11/10/coding-tools-principles/).
  
The high scorers did something different.

One pattern was "Generation-Then-Comprehension" - they had AI generate code, but then asked follow-up questions to understand what it did. Another was "Conceptual Inquiry" - they only asked conceptual questions and solved errors themselves. The third was "Hybrid Code-Explanation" - they asked for code and explanations together.

The highest scoring group (86% average) looked almost identical to the lowest scoring group (39%) at first glance - both used AI to generate code. The difference? The high scorers took an extra step to check their own understanding afterward.

--

This feels like empirical evidence for something I've been thinking about. It's not whether you use AI, but how you use it to not only complete the task, but also to learn on the way.

The paper found that participants who encountered more errors and resolved them independently learned more. The struggle was the point. But crucially, you can still use AI and preserve that struggle - if you stay cognitively engaged.

Asking "write this function for me" is different from asking "explain how this nursery pattern works." Both use AI. One has an opportunity to learn, but one doesn't.

There's a line in the paper that stuck with me. Participants in the AI group self-reported feeling "lazy" and noted "there are still a lot of gaps in my understanding." Meanwhile, the no-AI group found the task "fun" and said the instructions helped them develop understanding.

The AI users knew they were learning less. They just couldn't resist the shortcut.

I think this is the real challenge. It's not about restricting AI access. It's about developing the discipline to use it in ways that build, rather than bypass, understanding.

In my previous post, I wrote that becoming a good software engineer is less about knowledge now, and more about discipline. This research suggests the same thing from a different angle: the tools are neutral. The discipline to stay curious and wanting to learn - that's what separates growth from stagnation.

--

Perhaps, this is not just about coding, but how AI will impact education overall. Our children will have more tech-integrated life than us. Recently, the book [Anxious Generation](https://www.anxiousgeneration.com/book) raised awareness of the negative impacts of smartphones to our kids. AI will be a bigger wave.

This leads me to a seemingly unrelated, but deeply connected question: how do we raise a child who is curious and self-driven toward learning, even when there are just shortcuts right there? I feel like this is asking a child (or anyone really) full of marshmallows and chocolates to not eat it and just eat a bowl of salad everyday. 

Being a parent myself, I have started to gain tremendous interest in the matter.

--

Recently, I read an article from the Economist, [Why child prodigies rarely become elite performers](https://www.economist.com/science-and-technology/2026/01/14/why-child-prodigies-rarely-become-elite-performers). The gist was that children who specialized in a discipline too early didn't necessarily have a higher chance of success as adults. Children who were exposed to various kinds of sports were more likely to become elite professional athletes. For example, Rafael Nadal played football until he fully committed to tennis at age 12. This was true in science and other fields as well.

There was an interesting hypothesis in this article - children who tried various sports learned how to learn.

> "Learning is itself a learnable skill, and the best way to hone it is to pursue a variety of things."

Going forward, learning how to use AI well and developing that discipline also feels like learning for the sake of learning. Perhaps the conclusion is that we need an educational shift that enables children and juniors to learn how to learn, even when shortcuts like AI exist. In a society where educational philosophies focused on outcomes are prevalent, this feels like a significant paradigm shift, but I believe this is truly the necessary direction for growing ourselves and properly educating our children.