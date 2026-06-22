---
layout: post
title: Early Learnings from Building Pomelli at Google Labs
tags: [llm-products]
date: 2026-06-22

---

Pomelli went from zero user to being introduced in Google Marketing Live in a half of year. Thousands of people worldwide are using it to grow their business. 

<img src="/images/pomelli-launch-2/gml.png" alt="Pomelli at Google Marketing Live" style="max-width: 100%; height: auto; border-radius: 8px;">

We shipped multiple features since the first launch. Photoshoot, Product Catalog, Agent, and many more. The team's momentum is very high. I remember one launch day, we shipped an important in the morning and planned for the next on in the afternoon.

This is all happening in less than a year since I joined Google Labs. The team is growing, too. When I first joined, I could count all engineers with one hand. Now, the team is scaling up so fast that we constantly talk about ways of work and culture. I never knew I could experience such thing in a Big Tech like Google. Perhaps, this is unique to only a few orgs like Labs, where 0-to-1 products are born, die, or grow.

<video autoplay loop muted playsinline src="https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pomelli_agent.mp4#t=0.001" style="width: 100%; border-radius: 8px;"></video>
*Introducing Pomelli agent.*

My first half of 2026 was focused in making Pomelli take off from the ground. While we have a long way to go, we have succeeded in gathering significant amount of attention internally and externally and being used by different small and medium sized businesses. 

I want to share what I have learned so far from working on an experimental AI product. This is not only for sharing my knowledge, but also for my own future reference. I hope my insights are helpful for those who are working on similar projects.

## System Design & Last Mile 

In the era of vibe coding, people say that the cost of writing code has fallen. This may be partially true, but it does not mean that making a good product has become easier. 

Vibe coding is great at creating things for the 1st time as proof-of-concepts or minimal viable prodcuts, but it only gets you to 70-80%. This is already a very impressive progress of AI tools, but it will be very challenging to get a vibe coded app working in scale reliably, once real users come in.

Once real users start using the product, basically it is equivalent as a moving train. Making changes and bug fixes reliably is same as changing the track in front of you and the train engine while the passengers are inside. Since you are not the only user, you can not simply hit "re-generate".

For this reason, system design is still very relevant in making the product scalable and maintainable. AI agents may have the knowledge to do this, but is vulnerable to make short-sighted decisions when it writes code, unless the engineer can orchestrate the work properly. Like I said before, software engineering is larger than coding.

The "last mile" engineering, which takes the 70-80% to 90-100%, is crucial in making a good product. This may mean fixing edge case bugs, improving quality of generative AI outputs via eval & iterations, or reconsidering user workflows based on feedback.

Our team believes that the success of Pomelli came from our focus on last mile efforts before shipping. Many features were a result of team-wide feedback sessions & user research and individual members' obsession of quality.

This also requires willingness to tolerate some less important aspects via ruthless prioritization. Perfectionism should not slow down our velocity.

## Go-to-marketing (GTM) is King
<iframe width="560" height="315" src="https://www.youtube.com/embed/SIkxIWxTNqI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Now hundreds of AI features and products are being launched every day. To cut through the noise and get our stuff into people's attention, go-to-market (GTM) strategy is very important.

Our marketing team is very involved in the product development discussion, so that our product development and GTM strategy align seamlessly. Our team engineers can question & push the marketing plan of the launch they are working on. This shows how strong our sense of ownership is.

Google Labs GTM Team is definitely the #1 important factor in the success of our product. During our Photoshoot launch, a lot of marketing bullets - influencer partnerships, media press, and even Google leadership level (ex. Demis, Josh) amplification - were spot on. 

In this noisy, fast moving world, GTM strategy is king, no matter how good your product is.

## Aligning on what to build is hard

In order to move fast, alignment among the team members, especially different functions like eng, PM, and design, is very important but challenging. 

I still experienced a lot of wasted time & efforts for some features, when we were not very clear on what we wanted to build. In the end, we had to rethink the values this feature wanted to bring to the user and cut out any parts that are not necessary or too difficult to achieve. 

Also, effective communication and decision making are often difficult when the team is moving fast and the scope is constantly keep changing. This could cause a lot of confusion and wasted efforts, risking the team to burn out from constant back-and-forth discussions and implementations.

In a startup like team with such fast moving pace, some of these are probably inevitable. The growing team size will make this pain even larger. However, it does not mean the team cannot do better. 

Our team is constantly trying to improve on this, even though it may cause uncomfortable conversations and tension. Feedback and iteration is the only way that we can keep a well-functioning team that builds a good product.


## Focus on real problems, not the buzz words

Lastly, this is probably the hardest thing to do. I see a lot of people keen on using buzz words like "agent", "harness", etc. to convince the value of their product. This may work for some niche audience, but in reality, most people do not understand or interested in understanding these "AI" concepts. 

They just want to get their problem solved. One core philosophy is to focus on solving the tangible problems of SMBs and be simple and easy so that they can use Pomelli to solve their everyday problems, leaving the underlying complicated tech behind.

--

Working on a new product is very exciting, but once it starts taking off, keeping the momentum and focusing on how the product and team should evolve are even bigger challenges. 

While I'm still learning and processing this journey every day, I wanted to document these early reflections from working on Pomelli during its formative stages.

Let me know if this was interesting, and I'd love to hear your thoughts or discuss further!
