---
title: Betting on AI
date: 2026-09-17 09:00:00 +0200
lang: en
toc: true
description: How a 3D printer, my parents' AI assistants, and the agents I build at work changed the way I think about investing time and money in AI.
categories: [Reflections]
tags: [ai, agents, open-source, 3d-printing]
image:
  path: /assets/posts/2026-09-17-betting-on-ai/cover.jpg
  alt: Different bets on AI, from 3D printing and interchangeable models to modular agents and personal identity, illustrated on a casino table.
---

> **A quick warning:** Despite what the cover image might suggest, this post is about neither stock market investing nor betting on Polymarket. Just a few bets on AI getting better. The casino is purely decorative. 😄
{: .prompt-warning }

A few days ago, my mum told me she thought I had known what was coming. I bought a 3D printer, and three weeks later GPT-6 Astra appeared with a video showing the exact same printer making a rocket. A little too much of a coincidence for her liking.

The truth is, I had no idea when Astra would arrive or what it would improve. But I did think AI was getting close to letting me create my own 3D designs.

It reminded me of a conversation I had with some colleagues: certain decisions are bets on AI getting better. Things you buy, skills you learn, or systems you build become more useful as models improve.

**The idea is to invest your time and money with tomorrow's AI capabilities in mind, alongside what it can already do today.**

Lately, I have made several personal and professional decisions with that in mind. Some have already paid off. Others are still open bets. Here are a few of them, and how I think about the possibility of being wrong.

**Table of contents**

* Contents
{:toc}

## 1. A printer that keeps letting me do more

I had wanted a 3D printer since secondary school, more than ten years ago now. Back then, they were too expensive for me, and I didn't know how to design in 3D anyway.

Over the years, prices came down. When I recently started seeing the first AI-generated designs, I felt it was finally time to buy one. The examples I had seen were pretty basic, literally funnels. But I expected models to keep improving, and **each better model would mean more things I could make with the same printer.**

What I didn't expect was such a sudden jump in 3D capabilities.

Since Astra arrived, my family and I have barely stopped: laboratory parts, decorations, prototypes for industrial components. My dad is even designing molds for a machine at his company by giving the AI instructions and reference images.

![Two gray 3D-printed mold plates with a grid of square cavities and raised blocks.](/assets/posts/2026-09-17-betting-on-ai/printed-mold.jpg){: width="1210" height="1606" }
_A mold my dad printed for his factory, using AI to help with the design._

That was exactly what I hoped to get from the printer: the ability to make useful things for everyday life without designing every one of them by hand.

The speed of it all is what made my mum suspect I had seen a leak about Astra's 3D capabilities. I hadn't. I had simply made a bet on AI getting better.

## 2. Betting on competition and open source

In February and March, I introduced my parents to OpenClaw, a tool that gave them an AI assistant capable of carrying out tasks. They quickly made it part of both their daily lives and their work at the family business.

They liked it so much that they wanted to come with me to ClawCon in Valencia to learn more. My mum and I ended up giving a talk about how she was using agents for administrative work at a small business.

Here is our ClawCon talk (in Spanish):

{% include embed/youtube.html id='MLigY13E9uc' %}

Around that time, changes to access conditions for Anthropic's models put us in a difficult position. Their models worked best for our tasks, and the alternatives we were trying in OpenClaw were giving us poor results. It felt as though we had to move to Claude Cowork or give up on the personal assistant we had built.

That evening, back at the hotel after ClawCon, my dad asked why we didn't just switch to Cowork, as other people were doing. If their models were the best, why make life harder?

My concern was that my parents' business context, information, and processes would become increasingly tied to a product that would be difficult to leave. I saw those access changes as hostile to users, and they had eroded my trust in the company.

I wanted us to be able to replace the model behind their agents without losing their way of working and starting from scratch. So I explained my thinking.

We already had a reference for what “good enough” looked like: we had seen Sonnet and Opus do the work. It seemed reasonable to expect OpenAI and open models to offer alternatives eventually, even if waiting meant accepting some limitations in the meantime.

I told my parents I expected a viable OpenAI alternative around the end of May, and open-source alternatives around September or October.

GPT-5.5 arrived on April 23, about a month earlier than I had expected. I also started hearing from people successfully running their Hermes personal assistants entirely on open models, such as DeepSeek V4.1 and GLM 5.3. Those alternatives were working for people roughly three months ahead of my expectations.

The result was that we kept the freedom to choose which model their agents used. For my parents, that has a very practical value: they can keep working without depending so heavily on one company's decisions.

If pricing, terms, or privacy conditions change, or something better comes along, they can replace the model without rebuilding their entire workflow.

**My bet was on competition between models continuing to grow, and on keeping our setup flexible enough to benefit from it.**

## 3. Building systems that benefit from better models

We have run into a similar problem at work.

You start building an agent and discover that the model isn't quite up to the task. It skips steps, chooses the wrong tool, needs overly detailed prompts or guardrails, or takes too many attempts to finish.

One solution is to guide it more closely: break the work into steps, add checks, and hard-code some of the decisions. That surrounding set of tools, instructions, and controls is what we usually call a *harness*.

All of that can be necessary. But it can also leave you with a system built too tightly around one model's limitations.

When a better model arrives, taking advantage of it requires redoing much of the work. Or you keep forcing it through ten steps because the previous model got lost when given more freedom.

That's why I try to distinguish between the parts of a system that serve a business requirement and the parts that compensate for a temporary limitation of the AI.

Permissions and checks on results have reasons of their own to exist. A rigid sequence we added because the model couldn't organize its work might become simpler with the next generation.

**The bet is to design for what is coming while adapting to what you have, so that a better model can translate into a better product.**

That might mean a modular harness whose layers can be removed as they become unnecessary. It might also mean experimenting with a solution that is expensive today but could become viable if cheaper models can perform the same task.

A good set of regression tests makes this much more practical. If you can benchmark an agent's actual results, you can quickly evaluate changes to both the model and the harness.

In our case, this approach has helped us turn model improvements into cleaner implementations and lower running costs, with less time spent reworking code.

You still have to test and measure. A new model doesn't automatically make every agent better. But the architecture can make it much easier to benefit when it does.

## 4. Bets that are still open

Three other ideas are influencing how I spend my time. I don't yet know how well they will hold up.

### Writing code by hand will matter less; knowing what to build will still matter

I spend more and more time designing solutions, working with agents, and checking results.

I still read papers and learn how systems work. That knowledge helps me design better solutions, catch mistakes, and come up with my own ideas. I also try to understand the business better: the easier it becomes to build something, the more important it seems to know what is worth building.

### A recognizable identity and body of work will become more valuable

As AI-generated content becomes more abundant, I think knowing who is behind something, what they do, and how they think will matter more.

That's one reason I am sharing more projects and experiences publicly, both here and on social media. For years, people had been telling me to write about the things I talk about in person. This summer, I finally started doing it more often.

I want people to know my work, and I want to make room for the conversations and chance encounters that can lead to new opportunities.

### More software will have an agent as its direct user

I am already developing tools that people will access through their agents. That makes me pay more attention to APIs, the Model Context Protocol (MCP), skills, and tools: the interfaces that let an agent use my software.

For the person behind the agent, the benefit is straightforward. They can ask their assistant to carry out a task without learning another application.

## 5. What if it takes longer than I expect?

Of course, any of these bets can go wrong. Progress can take longer than expected, costs can stay too high, or limitations we haven't yet understood can get in the way.

With the printer, things moved faster than I expected. Other decisions may take longer to pay off, or may never pay off at all.

That's why, when I buy something, I try to make sure it is useful today. When I learn a technology, I prefer knowledge that will still be useful even if my prediction is wrong. And when I build a system with future models in mind, I try not to compromise what already works.

At the same time, my working assumption is that models will keep improving. I want to avoid rigid decisions built around today's capabilities that will be difficult to undo later.

My rough planning heuristic is that once models start making progress on a benchmark, they may get close to saturating it within a year or so. I treat that as an expectation, not a rule, and I am much less confident about predictions more than two years out.

So when I see a model starting to solve a new kind of task, I ask myself:

> **What decision should I make today if, a year from now, this works well and is cheap?**

The answer is changing what I buy, how I work, and what I learn. These bets are what that looks like in practice.
