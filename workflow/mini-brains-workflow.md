# Mini Brains Workflow

![Mini Brains Workflow](../assets/mini-brain-workflow.png)

---

## Where this comes from

This workflow is inspired by **Andrej Karpathy’s LLM Wiki pattern**  
https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f

The core idea behind that pattern is simple but powerful: instead of retrieving knowledge every time you ask a question, the system builds a structured knowledge base that evolves over time.

What you’ll see here is a practical extension of that idea.

Instead of stopping at knowledge, this workflow goes one step further.

It turns knowledge into behavior.

---

## A different way to work with AI

Most people use AI in a loop.

They ask something, get an answer, adjust the prompt, and try again. It works, but it’s reactive. Every interaction starts from scratch, and the quality depends on how well you guide the model in that moment.

At some point, it starts to feel like you’re not building anything.

You’re just getting better at asking.

---

This workflow changes that.

Instead of reacting to outputs, you build a system that produces them.

Not through code.

Through structure, intention, and iteration.

---

## It starts with what you already have

Everything begins with your material.

Articles, transcripts, notes, documents, videos. The same resources you already use to prepare your classes.

Nothing fancy.

Nothing new to learn.

These sources are kept as they are. They are not modified or rewritten. They remain your reference point, your ground truth.

---

## You don’t do it alone

You work with an agent.

That agent can be OpenClaw, Claude Code, Hermes, or any system capable of reading and writing across files.

But the important part is not the tool.

It’s the relationship.

You’re not asking the agent to give you answers.

You’re asking it to help you build something.

It reads your material, helps organize it, connects ideas, and keeps everything updated as your understanding evolves.

Over time, it stops feeling like a tool.

It starts feeling like a collaborator.

If you want to see the actual instruction file used to guide an agent through this process, see:

[Agent Instructions for Building Mini Brains](../agent-instructions/instructions.md)

---

## From content to knowledge

As you begin adding sources, something changes.

Instead of isolated documents, your material starts forming a structure. Ideas connect. Concepts appear across different sources. Relationships become visible.

This is the LLM-Wiki layer.

Your raw content is transformed into structured knowledge.

Not automatically and not blindly, but through a process where the agent reads, proposes changes, updates pages, and keeps track of how everything evolves.

You stay in control of the direction.

The system handles the maintenance.

---

## From knowledge to design

This is where the workflow becomes uniquely yours.

Before anything becomes a Mini Brain, you pause.

You review the knowledge.

You decide what matters.

You define what the system should do, what it should avoid, and how it should behave.

This is not generation.

This is design.

You are shaping the system intentionally, together with the agent.

---

## The result is not an answer

It’s a Mini Brain.

A single `.md` file that contains everything the system needs:

- the knowledge it uses  
- the rules it follows  
- the boundaries it respects  
- the way it responds  

You can load it into an AI tool, use it, share it, or modify it.

It behaves the same way wherever it goes.

---

## Why this works

The power of this workflow comes from control.

You’re not relying on the model to decide what matters.

You define it.

You don’t need massive datasets.

You need the right **factual anchors**.

Key concepts. Important facts. Definitions. Constraints.

These anchors define the baseline.

The model still does the work of connecting ideas and expanding explanations, but always grounded in what you provided.

---

## Why this matters for educators

Students already use AI.

For them, it’s natural.

What they often lack is not access, but structure.

They don’t need more answers.

They need better ways to think, question, and work with information.

---

This workflow gives you that.

It allows you to prepare your material intentionally, shape how AI behaves, and guide how students interact with it.

Not generic outputs.

Your perspective.

Your structure.

Your classroom.

---

## This is a loop, not a pipeline

You don’t run this once.

You keep evolving it.

You add new sources, refine your knowledge, redesign Mini Brains, and improve the system over time.

What starts as a few files becomes something else.

A personal assistant.

A structured repository.

A second brain.

All working together.

---

## The idea behind it

Before you design how AI behaves, you need to design what it knows.

This workflow gives you a way to do both.

Not by coding.

By thinking, curating, and designing with intention.

---
## Want to start simpler?

If this workflow feels like too much to start with, there’s a simpler way.

You can use the **Meta Mini Brain**.

Instead of building the full system, you provide:

- some knowledge  
- a goal  
- a bit of context  

And the AI generates a Mini Brain for you.

👉 [Simplified Workflow](../workflow/simplified-workflow.md)
