---
layout: post
title: Some useful principles for using AI coding tools
tags: [llm-products]

---



<p align="center">
  <img src="/images/coding-tools-2/quardrants.png" alt="Quadrants" style="max-width: 100%; height: auto;">
</p>

# Mindset

## Quadrants

Think about where you are at this 4-quadrants.


Quardrant 1 - High Impact Zone.
Quardrant 2 - High Danger Zone.
Quardrant 3 - Full Fun Vibe Coding Zone.
Quardrant 4 - "Parents at the party" Vibe Coding Zone.


1. Potentially I can make the most impact with LLM, but also I need to be most cautious. Don't forget the code here is going to be run on production, so I need to be rigorous. I need to think about basic unit and integration testing.

Being productive here can lead to being good at my main job. Be thoughtful.

2. I would not operate here too frequently, unless I have a patient colleague who can help me review the code. But don't throw them a large chunk of garbage code without any understanding. This risks of making that person mad and lose trust on me. 

I should try to get my proficency at least at medium level, to Quadrant 1 as close as possible.

3. This is where I have no idea what's going on (flying blind), but get to have fun to see the outputs. At least, I need to make sure what you want as output (ex. UI, data visualization). I will probably waste a lot of time prompting, because I am not really understanding the code. Just ride the vibe.

4. Here is also quite productive, but not it's not totally vibing. I call it the parents at the party, because I might still be parenting the code that's been generated, which is not exactly vibe coding. It's like being a parent who still want to enjoy the party vibe while discplining their children.

## Intern

Treat AI coding tool as your intern, not an expert.

- Sometimes, I need to micromanage. Be specific about which files and past changelists to read to do the task.
- Give them tasks that are tedious, straightforward, and stupid, but and need to be done.
- Break up the tasks into smaller chunks.
- Don't trust their codes. Read their code with suscipicious eyes. Read the rationale of their changes, too. 
- Accept that they will sometimes be stuck in a rabbit hole.
- Accept that they will sometimes be brilliant than me and produce creative solutions.

## Use Git effectively + small change lists.

Make sure to separate into small chunks of changelists and commit what you already reviewed and that's good. This will help organize what's going on and roll back if things go badly.

Also, Some IDEs will first show the proposed changes that I need to accept in bite pieces. Please use this feature.

## Check your energy level

Sometimes, when things don't work, I tend to get into a loop where I just keep generating and prompting the AI coding tool to fix the stupid error message I don't understand. If it fails, I just regenerate or just reword the prompt slightly, and re-try.

LLMs get stuck in a rabbit hole, especially when I am stuck in the rabbit hole.

When my energy level is low, it's like I want to do doom-scroll. Don't doom LLM code. Take a break. Go get some tea, walk, exercise. Or just do it tomorrow.

And when your energy level is back, I try to actually read the code / error message myself without the AI coding tool. Sometimes, the answer is just right there.

## Don't tell your colleagues that you are using AI agents. Or do.

I still don't know if I should be embarrassed or proud when my manager or colleagues sees my triple monitors having two AI agents to write code. Once my manager said, "that's cool". I don't know if they meant it or started degrading my confidence in my code :P 

Anyways, I own your code and the results from it. People wil care less and less about how I got there as long as it is good. 

If I hire your own intern, I will be responsible for their outcome, but stakes may be low. In the LLM's case, the intern's work is coming out with your own name. Take pride in my work. Do you review. Don't take transfer this responsibility soley to my code reviewers.

# Final verdict

I am 100% sure that using LLM coding tools has become a crucial aspect for being a productive engineer. However, in order to do this, you first need to be a good, principled engineer, or you are going to produce sloppy work, which is a huge risk to not only your career but also your team's product. 