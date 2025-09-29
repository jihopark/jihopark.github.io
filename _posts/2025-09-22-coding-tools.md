---
layout: post
title: My approach of AI coding tools
tags: [llm-products]

---

Google IO 2023 was one of the most memorable event, because our CEO Sundar presented a piece of code that I reviewed.

<p align="center">
  <img src="/images/llms-are-engines/google_io_2023.jpg" alt="Google IO 2023 code demo" style="max-width: 100%; height: auto;">
  <figcaption style="text-align:center; font-style:italic;">
    My code being presented at Google IO 2023.
  </figcaption>
</p>

PaLM, the state-of-the-art language model at that time, was featured to not only fix your bug, but also put code comments in Korean!

A side story for this 15 sec presentation is that I was pulled into a group chat of several Korean Googlers to come up with the best example of LLM fixing a bug. I added this DFS example, because this was something I frequently get wrong. 

I was delighted that PaLM can fix this, but was even more happy when Sundar presented this code live to the world! 

(I joked that this would probably the most influential code snippet that I would ever write or review in my Google career..)

Anyways, this is just over 2 years ago. If I think about how I use coding agents in 2025, the advancement is mind-blowingly fast. People say that software engineering as a career is in track for deprecation. If vibe coding can build softwares, then why do we need expensive engineers?

Before we get to that question, I want to share how I use AI coding tools. I know that there might be a lot of folks who use AI tools better than me, but I want to record my current experience for my own future entertainment.

## Google's Developer Ecosystem / Culture

Google definitely has a unique developer ecosystem and culture, so unique that a software engineer working for Google has a risk of being stuck in it.

(If you are interested, you can read [Software Engineering at Google](https://abseil.io/resources/swe-book))

But in terms of AI coding assistant, I would say outside world has moved much faster. Github Copilot, Cursor, Windsurf, Claude Code, and so many applications have came up over the last 1-2 years.

Since Google has a lot of software engineers, there is huge incentive to make our tools better. Also, we have Gemini, especially 2.5 showing huge improvements in coding capabilities.

By now, our internal AI coding tools have catched up a lot, and engineers adopted fast. We also have released them to the public, so I can introduce some workflows that I use frequently:

1. [gemini-cli](https://github.com/google-gemini/gemini-cli) - a terminal based coding assistant. Similar to Claude Code.
2. [Gemini Code Assist](https://codeassist.google/) - we don't use exactly this, but similar features are integrated to our internal IDE, Cider and code review tool, Critique.

## Most Productive Workflows (I find)

### 1. Code Understanding

When I joined the new team in July, I had to onboard to a new codebase as soon as possible. But the challenge was that I have never written a Java backend nor Angular.js frontend code! Since I mostly worked on data, I was more familiar with C++ or Python.

Obviously, my team mates are the most helpful for onboarding, but I did not want to bother them for every details of the code. So I decided to leverage Gemini CLI.

> "(Hey Gemini) Explain the workflow of this function. Draw a diagram."

> "Which file does this link to? How is it wired up this way?"

It is like having a mentor with unlimited patience and bandwidth right next to you!

I drew how some parts of the code worked on a whiteboard with the help of Gemini to get the whole picture and the details. This really boosted my onboarding. I even could give a presentation to my colleagues on what the status quo of some component is and suggest improvements.

### 2. Refactoring

Refactoring is often neglected, because it is tedious structural changes of the code - Moving function parameters around, breaking down functions, renaming things - while not breaking the compiler or the original feature.

Good news is that LLMs never get bored and is amazing at syntax. Also, it can go through the whole code or even codebase and make changes that are needed if I change one little thing. Tedious edits like imports, header files, etc. 

A new feature development is some times blocked by refactoring. Now, small refactorings would not block me, because the time I spend on it reduced to 1/10.

### 3. Unit Test Generation

Important point to make your codebase easier to refactor is having good unit tests. Any basic unit test is significantly better than nothing. 

However, some times unit tests are omitted due to the tedious syntax of mocking and test case writing. Again, hard-working LLMs are here to help!

Obviously, I do not ask it to write unit test without knowing what I want to cover, but it helps a lot when I don't have different mocking library patterns on top of my head.

### 4. Writing new code

With LLMs, my way of thinking elevated to focus on the logic, rather than specific langauge's syntax. 

I have my basics on OOP and async operations in my head, but just not in Java, which I haven't used in more than 15 years. It would have taken me 2-5x amount of time if I had to look through Java documentations to find the equivalent of something in C++.

Now I will prompt the LLM to implement the logic I want. Sometimes, I even express myself in Python with a simpler syntax and ask it to implement the same logic in Java.

Another good thing is that the coding assistant will take the whole file as a context, so it follows the team's previous patterns and style, whenever reasonable.

I also find this super useful for frontend development. I recently picked up Angular.js, which sometimes involve modifying muliple files (javascript, css, html) at once. LLM is excellent for doing this.

### 5. Self-code review

Due to my personality, I tend to spend quite a lot of time to review my own code before sending it out to a colleague. Now, there is a feature to auto review a changelist. This has been great to reduce both my and the reviewer's time, especially I am prone to make basic mistake on a language that I'm not familiar with.

### 6. Error Message Parsing

Error messages can be brutally long and cryptic, but I now ask LLM to explain them to me and even suggest a fix! This really is a game changer to reduce time debugging.

### 7. Readability Suggestion

Google has a particular culture of readability reviews. Pros of this culture is that the overall code quality is higher, with the cost of slowing down. Especially for new product development, velocity is super important, so I felt relunctant to put any readability related comment on the code.

However, now LLM can read my nitty comment and attach a fix with it. The author can select to apply the fix with one button press. This is really effective to keep the code quality high, while maintaining velocity!

### 8. AI Powered Colab

Colab (Jupyter notebook) is a powerful tool for quick data analysis or data pipeline prototyping. Most colabs do not need to be elegent or well-tested as production code. 

This means that there is more room for "vibe" coding. Colab recently started adding [AI coding assistant](https://developers.googleblog.com/en/fully-reimagined-ai-first-google-colab/) inside the UI!

### 9. Vibe Coding Prototypes

Most of the time, demoing is better than explaining in words. Vibe coding prototypes when brainstorming new ideas on a feature is really powerful for this reason. 

I can imagine or already experienced how vibe coding can be so effective for non-technical roles like product managers, business devs, and UI/UX designers to build ideas without consuming engineering team's resource. 

Vibe coding is at the level to replace engineering teams, but I would not say too early given the pace of speed this space are developing.

I often use [Gemini Canvas from Gemini App](https://gemini.google/overview/canvas/) for this purpose, but there are about thousands of tools to vibe code something.

## Closing

There has been studies that using AI tools actually make [developers slower.](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/#:~:text=We%20conduct%20a%20randomized%20controlled,without%E2%80%94AI%20makes%20them%20slower.), but people are always talking about how crazy productive these AI coding tools are. Who is correct?

While I am not the most expert in this field, I can totally see that when not used properly these tools can slow you down. I also experienced some trial and errors.

There are some principles and tips I have on how to effectively use these tools, but that will be for my next post.
