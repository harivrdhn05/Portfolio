---
layout: post
title: "Can Agentic Systems Close the Gap in Radiology with Production AI Tools?"
summary: "What a radiology paper taught me about LLM orchestration, tool use and why more tools don't automatically mean a better agent."
---

I recently came across an interesting research paper titled **"Can Agentic Systems Close the Gap in Radiology with Production AI Tools?"** While exploring the paper, what caught my attention was not just its application of AI in healthcare, but how the authors demonstrated the potential of **Agentic AI and tool orchestration** to solve complex real-world problems.

As someone interested in Agentic AI, I found this research particularly interesting because it highlights an important idea: building an intelligent system is not just about having a powerful LLM. It is also about how effectively that model can interact with different tools, make decisions, and coordinate multiple tasks.

## The problem with traditional AI models

Traditionally, most AI models are designed to perform specific tasks. One model might identify something in an image, while another might measure it or compare it with previous results. Although these models can perform their individual tasks well, combining their capabilities to complete an entire workflow remains a challenge.

This is where Agentic AI comes into the picture.

## How the approach works

The paper explores an approach where an LLM acts as a central orchestrator. Instead of trying to complete everything in a single response, the system first understands the given task, breaks it into smaller steps, identifies the required tools, and executes them accordingly. It then collects the outputs, analyses the results, and decides whether additional steps are needed before generating the final report.

What I particularly liked was how the system could execute independent tasks in parallel while keeping dependent tasks in sequence. It also had an analysis stage where the orchestrator could identify missing information and revise its original plan. This makes the workflow much more dynamic than a traditional AI system that simply receives an input and generates an output.

## Model Context Protocol (MCP)

Another interesting aspect was the use of **Model Context Protocol (MCP)**. The authors took inspiration from MCP to create a shared interface through which the orchestrator could discover and interact with different tools. In simple terms, it provides a standardized way for an AI system to communicate with external tools, even when they are developed by different providers.

## More tools don't automatically mean a better agent

One of the most interesting findings in this research was that having access to more tools does not automatically make an AI agent better.

The researchers identified two major challenges: the availability of appropriate tools and the ability of the orchestrator to use those tools effectively. In some cases, the required tools were simply unavailable. In other cases, the tools were already available, but the agent failed to call them.

The experiments also showed that adding 99 frequently missing tools helped close approximately 74% of the performance gap between the existing tool catalog and an unlimited tool catalog in their evaluation. Another observation was that smaller models did not achieve the same performance as the larger orchestrator, even when they had access to the same tools.

## My biggest takeaway

We often discuss how to build more powerful LLMs, but perhaps an equally important question is how intelligently we can connect them with tools, external systems, and other models.

Agentic AI is not simply about connecting APIs or calling tools. It is about understanding when to use a tool, why it is needed, how to interpret its output, and when to change the approach.

## Limitations

Of course, the research also has limitations. The experiments were conducted using fictional reports and simulated tool outputs, rather than a fully deployed real-world system. So, the findings demonstrate potential rather than guaranteed real-world performance.

## Final thoughts

Overall, this paper gave me a different perspective on the future of AI systems. I believe the next stage of AI development will not depend only on how powerful individual models become, but also on how effectively they can collaborate with tools and systems to accomplish complex tasks.

**Perhaps the real potential of Agentic AI lies not in making one model do everything, but in making different components work intelligently together.**

Tags: #AgenticAI #ArtificialIntelligence #LLM #MCP #GenerativeAI #AIResearch #Automation
