# Content Tone Converter

> Rephrase the same information for different audiences by adjusting tone and style. Built for non-technical users: just say how you want it to sound.

[English](./README.en.md) · [中文](./README.md)

## What it is

Content Tone Converter is a Skill for the WorkBuddy AI assistant. Its core job is to rephrase the same information for a target reader by switching tone and style, without changing the underlying facts or conclusions.

It is built for users with no technical background. You do not need to know prompt engineering or write any code. Just say something like "make this easier to understand" or "turn it into a formal report", and you get a ready-to-use result.

Its most distinctive value is that the before/after difference is visible at a glance. Every conversion makes the expression barrier feel lower immediately, which is why it is easy to adopt and easy to recommend to others.

## Features

The skill ships with four conversion modes that can be used alone or combined.

| Mode | Name | Best for | Trigger example |
| --- | --- | --- | --- |
| 1 | Tech doc to friendly narrative | API docs, code comments, jargon-heavy text | "Explain this tech doc to a layperson" |
| 2 | Casual chat to formal report | Chat logs, meeting fragments, spoken ideas | "Turn this into a formal report" |
| 3 | Stiff formal to casual social tone | Corporate buzzwords, paper abstracts, manuals | "Make it more casual, like a social post" |
| 4 | Apply Wang Chen writing rules | Chinese text that should follow the house style | "Polish this using my writing rules" |

Modes can be combined. For example "make this tech doc casual" equals Mode 1 plus Mode 3.

## Quick start

### Install

Send the line below directly to your Agent software. No manual steps are required (use the copy button on the top right of the code block to copy the link in one click):

```
Install this Skill https://github.com/wangchentalk/content-tone-converter
```

And hand it to your Agent software (such as WorkBuddy, Doubao, traeWork, Qwen Office), then simply wait for the agent software to install it automatically. Agent software that supports this includes WorkBuddy, Doubao, traeWork, Qwen Office, and similar tools. After you hand over the link, wait for it to finish installing on its own.

Agent software that supports this includes WorkBuddy, Doubao, traeWork, Qwen Office, and similar tools. After you hand over the link, wait for it to finish installing on its own.

### Use

Describe the tone you want in plain language. Trigger examples:

- "Explain this technical doc to a layperson."
- "Here is my chat with ops, turn it into a formal report."
- "This sounds too corporate, make it casual."
- "Polish this with my writing rules: no em dashes, add sources."
- "Make it social and sign off with my brand."

The skill detects which mode applies and returns the result.

## The four modes

### Mode 1: Tech doc to friendly narrative

Rewrites jargon-heavy text with everyday analogies and a "why, what, how" narrative. Output reads well aloud and ends by stating what it means for the reader.

**Example**

> **Source**
> LLMs achieve parallel computation through the Transformer architecture, use self-attention to capture long-range dependencies between tokens, and align with human preferences via RLHF.
>
> **Converted**
> Think of a large model as a learner who has read a vast library. It relies on a method called Transformer to digest whole passages at once instead of memorizing word by word. Self-attention lets it spot which words relate to each other even when far apart. Then RLHF steps in: humans score its answers and gradually tune its output toward what people actually want. That is why, when you talk to it, it feels like it understands the context. These mechanisms are what make that feeling real.

### Mode 2: Casual chat to formal report

Distills chat logs and spoken ideas into a three-part report: background, current status, next steps. Fills in subjects, dates, and owners.

### Mode 3: Stiff formal to casual social tone

Rewrites corporate or academic text into a relaxed, conversational short piece fit for social feeds, newsletters, or video voice-over.

**Example (social tone + brand sign-off)**

> **Converted**
> Your phone app is about to get easier to use. We have been quietly putting it on a diet, making buttons easier to tap and the screen easier on the eyes, so you take fewer wrong turns. Feel it yourself in the next update, and if something still feels off, tell us anytime.
>
> I am AI·Wang Chen Shuo, breaking down practical AI for everyday people. More hands-on methods at https://wangchenai.com

### Mode 4: Apply Wang Chen writing rules

One-click house style: remove em dashes, drop "not A but B" flip phrasing, add a dialectical perspective, cite sources, and curb emoji and empty slogans.

## File structure

```
content-tone-converter/
├── SKILL.md                # Main skill file: mode rules and flow
├── references/
│   ├── examples.md         # Before/after samples for all four modes
│   └── style-rules.md      # Wang Chen writing rules (Mode 4 constraints)
├── README.md               # Chinese (default)
└── README.en.md            # English
```

## Brand

This skill belongs to the personal IP "AI·Wang Chen Shuo" (AI·王陈说).

- Brand: AI·Wang Chen Shuo
- Site: https://wangchenai.com

Principle: the brand and site are attached only when the user asks for it or when the output is clearly meant for public release. They are never forced into every conversion.

## License

Free to use and modify. When redistributing or building on it, please keep the original attribution (AI·Wang Chen Shuo).
