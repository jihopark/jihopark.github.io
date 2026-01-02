---
layout: post
title: Can LLM coding agents replace software engineers
tags: [llm-products]

---

Maybe this post is for those executives/managers who think their dev teams can all be laid off and replaced by LLM coding agents.

I heard a story from my software engineer working in finance that his stakeholder came back with some vibe coded results from ChatGPT and asked him why his team cannot fulfil his request faster. In my friend's mind, several reasons came up - integrating to existing prod code, some weird tech debt, headcount issue, etc. - but he did not say much, because it would all just sound like an excuse to the stakeholder and make him sound incompetent. Those reasons are hard to explain to a non-technical person without enough context.

Like this anecdote, vibe coding makes our jobs look so easily replaceable. Compelling quotes from people like Jensen Huang (who has a serious stake in hyping up the idea of replacing dev team jobs with his GPUs) appear on famous business news and magazines. 

What should we do? Students or juniors—should you stop pursuing this path? Seniors—should you treat this as a mid-life crisis and start looking for other occupations? I mean, how can we possibly be better than Devin, our software engineer AI?

https://www.youtube.com/watch?v=fjHtjT7GO1c&ab_channel=Cognition

Let me say this—not all software engineers will be replaced! (But, as always, I may be wrong, so don't depend on my word for your career decisions).

## Coding vs. Programming

There is a lot of confusion between these two words, especially among non-technical people. In order to contemplate our existential crisis, we need to clearly define these terms.

**Programming** is fundamentally about getting computers to work on tasks for us. These tasks are something that we do not want to do, because they are tedious, time-consuming, or too complex to do. We can also think of this as “automation”.

**Coding** is about giving computers instructions for these tasks. It is a way of communication. We started from punching holes in cards. Often, we need programming languages like C++ and Python, which closely resemble our common language English and mathematical expressions. Nowadays, there are also "no-code" platforms, which make it easier to instruct the computer via UI. While these are not written format, they still can be considered as "coding" as they should have some syntax to make things work (think of Scratch, the UI-based programming language, or Zapier, or recently n8n workflows).

**Programming** is larger than coding. A child can learn how to write the alphabet, but it is not sufficient to write a sentence. Writing a sentence is a good start, but not sufficient to write a book, let alone an essay.

**Programming** involves all processes that go into developing software—problem definition, planning, ideation, design, testing, and many more. Coding is just one small part.

## Programming vs. Software engineering

Let’s look at even a bigger picture. **Software engineering** is not just about **programming**. Software engineers don’t build real, physical things, such as bridges or tunnels like civil engineers, but we are still called “engineers”. Why?

Because we do not just "code" to automate tasks, but we build "programs" that perform tasks not thousands, probably millions, maybe trillions of times. Such repetition needs to be reliable, lasting for a pretty long time, serving many customers. We also need to build new features. This often requires structural changes to the program, which incur constant refactoring and migrations. Doing this while maintaining stability is like changing train components while the train is running at 300 km/h!

Even before that, we need to figure out what to build. People may think that this is the role of product managers, designers, or business developers, but without the input of software engineers, such proposals can be disastrous from the beginning. Some companies do not even have other functions, so engineers need to wear those hats ourselves.

Last but not least, software engineering is mostly a team sport. Unless you are an individual, independent developer, you most likely work with a team of other software engineers and non-tech functions. This involves "social" and "management" aspects, which many of us dread, but it is necessary to get big things done. Code reviews, bug tracking, project management tools, etc. exist for this reason.

## Can we be replaced by LLMs?

Now that we have defined these three terms, we can go back to the question: "Can software engineers be replaced by LLMs?"

Well, it depends.

While it is debatable whether LLMs have or will bring enough value in all industries, one thing for sure is that they have fueled the productivity of software engineers. 

They can do coding pretty well with amazing speed. Apparently, a lot of our work involves "boilerplate" tasks, which were tedious and time-consuming. LLMs excel at these. 

As I mentioned in my previous post, they have almost replaced Stack Overflow and a lot of API documentation reading. For example, I use the Python libraries Pandas and Matplotlib a lot, which I find the APIs not too intuitive sometimes, but using Gemini really boosted my productivity. 

With some good principles as I discussed, LLM coding tools will make software engineers productive.

Being productive is one thing, but do LLMs always make the right decisions?

## Context, context, context for decisions.

When Claude and Gemini came up with millions of tokens of context window, a lot of people thought: "Now, I can attend to the whole codebase, so I have all the context!"

Yes, but not enough yet. Apparently, not all contexts are documented. Some might be from a meeting that happened 2 years ago, or an office corridor chat that happened 3 minutes ago. In reality, codebases are really messy and documentation is almost never complete. Some contexts are not always accessible to LLMs.

Humans live in context—we didn't fall from the sky. The more senior you are, the more context you need to absorb. That's why they attend so many meetings, conferences, etc. A competent, long-tenured engineer leaving your team is going to hurt the team, because they exit with all that context.

So yes, the so-called "long" context of LLMs is not long enough to replace your engineer, who makes decisions on what and how to build things.

## Conclusion

So, can LLM coding agents replace software engineers? The answer is not straightforward. LLMs have become powerful productivity tools that handle boilerplate, answer API questions, and speed up development. But software engineering encompasses far more than coding: it requires understanding undocumented context, making architectural decisions, navigating technical debt, collaborating across teams, and balancing competing priorities in real-world systems.

The stakeholder in my friend's story saw working code from ChatGPT and wondered why the team couldn't deliver faster. What they didn't see was the invisible work—the context, the trade-offs, the maintenance burden, the human judgment. 

Again, who knows how far LLMs will advance in 2026! Let's just hope we can keep growing ourselves so we won't be replaced by AI any time soon.
