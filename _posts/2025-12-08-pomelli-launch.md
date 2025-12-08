---
layout: post
title: My 1st Google Labs Product Launch - Pomelli
tags: [llm-products]

---

Launching a product is exciting, until the server goes down after 3 hours. Users were complaining on Twitter and Discord that they cannot get in.

I joined Google Labs this July and was fortunate enough to get a chance to experience a product launch only after 3 months! Let me share what happened and some thoughts.

## What is Pomelli

[Pomelli](https://labs.google/pomelli) is an AI marketing tool for small and medium sized businesses. It understands each business and brand and helps one to easily create marketing campaigns and creatives, tailed to each business. Read more in the [Google Keyword Blog](https://blog.google/technology/google-labs/pomelli/).


![bdna](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_1.width-1000.format-webp.webp)
*Generate the business DNA*

![campaign](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_2.width-1000.format-webp.webp)
*Create your marketing campaigns*

![creatives](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_3.width-1000.format-webp.webp)
*Generate in-brand creatives.*

<iframe width="560" height="315" src="https://www.youtube.com/embed/rsWPISYv6tQ?si=1c4Hfq0Wfldlvi0J" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

This was a beta launch, now only available in USA, Canada, Australia, and New Zealand. Hopefully, we can launch in more countries next year!

## Launch Day

The morning we launch, the team was thrilled. We had a live dashboard to see real traffic coming in. It was supposed to be a relatively a silent launch, but we got a lot of attention in X (Twitter) and other channels. 

But then the things were not working after 3 hours. Our servers were not responding properly. Users started complaining that they cannot go to the next stage of the product. 

Apparently, things were melting on the component that I worked on. We had to analyze what's going on and figured some part of the code was problematic. I had to do an emergency bug fix to cut that part of the code out, without too much sacrifice of the original feature.

I deployed the code, hoping that things would work again. However, it didn't. By this time, users were blocked for several hours. We were even considering to put the curtains down, saying that we will be back later. 

But then my amazing colleague detected another, potentially relevant, issue in the server. He started working on a fix. Things came back to normal. We announced to the users that we experienced a distruption due to unexpected amount of traffic, but we fixed the issue.

It was almost midnight when things concluded. We could all go to bed that day.

## Takeaways


### Good problem to have

Our PM director, Jaclyn, wrote in [her blog](https://blog.jaclynkonzelmann.com/p/embracing-the-success-disaster), reflecting the launch. 

She called this the **Sucess Disaster**. Because we were successful to get attention and traffic, problems revealed. 

> "This is the kind of problem you want to have. The reason things went wrong was because something went incredibly right."

This view blew me away, not only because it is such a positive perspective, but also because it is such an accurate take. We would have never caught this issue with only hundreds of users, but only by having thousands or even more users using the product.

In the end, we are having unbelieveable amounts of users coming in and trying out our product!

### Early Experiment

The philosophy of Google Labs is to launch early and validate fast. In a huge company like Google, it may be hard to have this kind of mentality and environment. Google Labs is literally a product labatory to avoid falling into such trap. 

Just go take a look at https://labs.google and see what we are doing. There are many things that are hard to imagine a large company like Google would work on.

After launching Pomelli, I am now starting to understand and experience what this philosophy actually means.

### The bigger picture

That does not mean that we are aiming for small things. We are launching fast, but these are just seeds of something that is potentially much bigger. 

For example, Pomelli is not just another content generation tool, but it may become an ultimate operating platform for small and medium sized businesses, which Google has traditionally not been great at. 

Forbes already analyzed the potential of our product - https://www.forbes.com/sites/solrashidi/2025/10/31/will-googles-ai-bet-pay-off/

For this reason, we need to think big and look multiple steps ahead, but need to start somewhere.

--

This launch is one of the highlights of my whole programming career. I'm very happy that I decided to join this org and team and launch something with the team so fast.

I am learning and experiencing a lot of interesting product and engineering problems, so I'm looking to write more on those things.