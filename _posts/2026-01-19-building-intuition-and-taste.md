---
layout: post
title: Building intuition and taste
tags: [llm-products]

---

Every time AI coding gets better, my job description gets fuzzier.        

Recently, I have been trying out more new tools like Google [Antigravity](https://antigravity.google/) and Claude Code, for both work and hobby projects and it's been an eye-opening experience.

This weekend, I had a one-hour window, so I decided to try out this idea of a grocery logger, where Claude can read my grocery receipt image, categorize them, and save them into a DB. Then later, I would be able to ask questions like, "How much did I spend on meat this month?", "Which groceries have the cheapest rice?", or "Is this dumpling a good price?"

In my "experience", I "knew" this involved creating a MCP (Model Context Protocol) server with a SQLite Database, so I did some quick research and found out that Claude Desktop can connect to a MCP server locally on my MacOS.

Okay, great! I started to write a prompt, which felt like drafting a design doc, listing out what functionalities I want, what the inputs and outputs are, what are the end use cases I want to support. And clicked enter.

BOOM. Claude Code wrote the MCP server, even ran commands to start the server, looked at the errors, fixed the first draft, and then completed the code. I reviewed the code and gave some suggestions. With about a 5-turn conversation, an MCP server was completed and fully integrated to Claude Desktop. 

At this point, I was 15 minutes into the process. Then another 15 minutes, I was looking to deploy this server online. Claude gave me some suggestions on which free services I can use, with pros and cons. I liked one service, because I "felt" that persistency in the DB together with the server node would save me a lot of trouble. In about another 20 minutes, the server was fully deployed and I could use it on my mobile app.

<p align="center">
  <img src="/images/building-intuition/claude1.png" alt="claude_screenshot" style="max-width: 100%; height: auto;">
</p>

I still had 15 minutes before I had to do my family chores, so I was "thinking", maybe a fuzzy string matching of the item names might help, so I prompted.

`nice, that worked. let's go back to feature development. Should we add fuzzy matching to query item_price or query_spending for robustness?`

I thought it's funny that I had to show positive sentiment here and also ask for an opinion, rather than asking Claude to implement it, but I guess I had a "gut feeling" that this feature was possibly not important, so framed it as a suggestion.

And then surprisingly Claude said:

<p align="center">
  <img src="/images/building-intuition/claude2.png" alt="claude_screenshot2" style="max-width: 100%; height: auto;">
</p>

Wow, this kind of pushback is something a good junior engineer would do. Mind blowing!

--

I'm sure a lot of you experienced much more extensive and complicated usage of tools like this (and much earlier than me), but this got me thinking a lot. It was like hiring a super fast and smart intern, who is most likely going to get better day by day.

In order to make good use of this intern, I must be thinking at one abstraction layer higher. I need to be more like a product manager, a tech lead, and a UX designer.

PMs decide what to build. Tech leads decide how to architect it. UX designers decide how it flows. The common part? Decisions. 

## Intuition

Then how do you make "good" decisions? So far, the best decision makers I have seen do these two things well: (a) gather many ideas (diverge), (b) rapidly decide which ones to apply (converge).

And this requires intuition, because in most real situations, you don't have time or complete information to analyze everything rationally with all the data in the world.

Thinking on my own, I think my intuition for software engineering is built over decades of hands-on work. I have been coding for 20+ years, since I was a teenager. For education, for fun and for work. 

I can still feel the codes that I wrote for the 1st time when I was a teenager - from the command line based Blackjack and Omok game, ASP.NET website I built and maintained for our high school student community, Android client code for my first paid internship, the first Tensorflow Keras code that ran on 1 GPU in my postgraduate NLP lab, numerous data pipelines I wrote in my first team in Google, and the latest launched AI product Pomelli.

I remember one course in my 2nd year of undergrad called Computer Organization, where Assembly was taught. I had to manipulate bits with this ancient language. At that point, I didn't really get the point of this course. It was mandatory so I took it. Looking back, the course probably didn't have a huge impact on my skills itself, but it has somewhat contributed to developing my intuition about how the computer works under the hood. Similarly, C/C++ taught me Object Oriented Programming, and Ruby on Rails taught me the basics of web programming.

Taste is another big part of intuition that gets built by doing and trying to get the details right. It's weird to say that software engineers have "taste", but it is important when there is no right or wrong. I believe that some part of software engineering is a form of art, so, yes, there is definitely taste involved.

I feel like automatically generated code doesn't build taste, at least not as effectively as writing them yourself, similar to how Spotify's algorithm does not necessarily build new music taste. 

Intuition and taste are built when you can actually sense your work and are willing to explore the unknown. 

## A new Generation of Software Engineer

I'm concerned about how new programmers can build intuition and taste. Why learn the details when AI can handle them for you?  

But that's exactly the trap. A good engineer will need to think for herself—deciding when to dig deeper versus when to stay high-level, and actively seeking opportunities to build intuition.

Becoming a good software engineer is less about knowledge now, and more about discipline. A healthy stubbornness to understand things even when you don't have to. That's harder than learning to code.

--

This isn't just about coding, though.  

Writers, designers, musicians - anyone whose craft is built through repetition (many parts of life) faces the same question: how do you develop taste when AI can do the repetition for you?

I don't have an answer. But as a parent, I think about this constantly. I want my children to develop the intuition to write their own thoughts, design with their gut, explore music with their ears—not just consume what algorithms serve them. 

Maybe I'm a traditionalist. But I'm not a pessimist. Assembly becoming Python didn't make us worse engineers. Encyclopedias moving to Wikipedia didn't make us stupid. We've adapted before.                                                                                                                          
                                                                                                                                                             
Still—how do we build intuition in a world where AI can shortcut the hard parts? That's a question I'll keep thinking about.    