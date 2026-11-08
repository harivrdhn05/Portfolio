---
layout: post
title: "STAIR: Using a Book's Table of Contents to Improve RAG"
summary: "A simple but clever idea from IBM research that makes AI retrieval structure-aware."
---

I was browsing Google and came across an interesting research paper from IBM called STAIR. I read through the whole thing and am fascinated by how easy the concept is!

## To summarise

AI models such as ChatGPT only have knowledge of what they were trained on. This means that they won’t have seen your company documents or textbooks. When asked questions relating to these documents, they may just guess. With RAG, before the AI answers the question, it searches for the correct text within your documents and provides it to the AI model. This is like an open-book exam.

## Limitations of standard RAG

Standard RAG has some limitations. Most systems split the document into small parts of equal length. This doesn’t take into consideration the meaning of the text. An answer could be split between 2 parts and also the part loses context about which chapter it is from. All books have a map of where everything is, the table of contents. This isn’t used in standard RAG.

## How STAIR works

STAIR uses the map of the book. Its name stands for STructure Aware Information Retriever. When a question is asked, the AI sees the question and the full table of contents from the book. The AI will select the section that it believes will contain the answer. As the AI can only select real sections, it can’t create a fake section. This is what we do when we open a book and look at the contents page.

The best thing is that nothing is complex. The researchers have taken advantage of the structure of the document.

## Where it works best

This works best with documents that have a clear structure. Textbooks, manuals and reports. I’m excited to see where this will go.

Source: arXiv 2609.03874

Tags: #RAG #AI #IBM #LLM
