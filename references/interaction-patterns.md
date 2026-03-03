# Interaction Patterns and AI Skill Formation

Reference material for the learning-partner skill. Based on Anthropic's randomized controlled trial: "How AI assistance impacts the formation of coding skills" (Shen & Tamkin, 2026).

Source: https://www.anthropic.com/research/AI-assistance-coding-skills

## Study Summary

52 software engineers were tasked with learning a new Python library (Trio, for async programming). Half used an AI assistant, half coded by hand. All took a quiz immediately after.

- **AI group average score**: 50%
- **Hand-coding group average score**: 67%
- **Difference**: 17% (nearly two letter grades, p=0.01)
- **Largest gap**: Debugging questions

The AI group finished slightly faster, but the speed gain was not statistically significant.

## Low-Scoring Interaction Patterns

These patterns led to quiz scores below 40%. They share a common trait: the developer offloaded thinking to the AI instead of building their own understanding.

### AI Delegation (n=4)
- Wholly relied on AI to write all code
- Completed tasks fastest
- Encountered few or no errors during the task
- Scored poorly because they never engaged with the material

**Why it's harmful**: Speed without comprehension. The developer ships code they can't debug, modify, or explain.

### Progressive AI Reliance (n=4)
- Started by asking 1-2 questions independently
- Gradually delegated all code writing to AI
- Lost engagement on the second task entirely

**Why it's harmful**: Starts well but erodes. The initial effort creates false confidence that "I understand enough" when the understanding is shallow.

### Iterative AI Debugging (n=4)
- Wrote some code independently
- Relied on AI to debug or verify their code
- Asked many questions, but aimed at getting AI to solve problems rather than understanding them
- Were also slower at completing tasks

**Why it's harmful**: High activity masking low learning. The developer is busy interacting with AI but never builds the mental model needed to debug independently.

## High-Scoring Interaction Patterns

These patterns led to quiz scores of 65% or higher. The common trait: the developer maintained cognitive engagement even while using AI.

### Generation-Then-Comprehension (n=2)
- Generated code using AI, then manually copied/pasted it
- After code was working, asked follow-up questions to understand it
- Not particularly fast, but scored well

**How to encourage this**: After providing a code solution, prompt the developer to explore why it works. Ask "Does the relationship between X and Y make sense?" or "What would happen if you changed Z?"

### Hybrid Code-Explanation (n=3)
- Asked for code generation alongside explanations of the generated code
- Spent more time reading and understanding the explanations
- Took longer but showed higher comprehension

**How to encourage this**: Always pair code with reasoning. Explain why this approach was chosen over alternatives. Highlight tradeoffs and what could go wrong.

### Conceptual Inquiry (n=7)
- Asked only conceptual questions ("How does X work?", "What's the difference between Y and Z?")
- Used improved understanding to write code independently
- Encountered many errors but resolved them independently
- Second fastest overall (after pure AI delegation)
- Highest learning outcomes

**How to encourage this**: Lead with concepts before code. When the developer asks "how do I do X", explain the underlying pattern first. Let them attempt the implementation. Guide with hints rather than solutions.

## Key Insight: Debugging Is the Biggest Casualty

The largest score gap between AI and non-AI groups was on debugging questions. This makes sense:

- Developers who used AI encountered fewer errors during the task
- Developers who coded by hand hit errors, struggled with them, and built debugging intuition
- The debugging skill gap is especially concerning because debugging is the primary skill needed to validate AI-generated code

This means the most important behavior for a learning partner is **not fixing bugs immediately**. Let the developer sit with the error, form a hypothesis, and attempt a fix. The discomfort of being stuck is where debugging skill is built.

## Practical Implications

### Time Investment

The high-scoring patterns were not significantly slower than low-scoring ones. Conceptual inquiry was the second-fastest overall. The cost of learning is not speed -- it's cognitive effort.

### The Developer's Intent Matters

The study found that developers who scored well actively chose to engage. They asked "why" questions, requested explanations, and explored concepts. This was a deliberate choice, not an accident.

A learning-partner skill can nudge developers toward these patterns, but it cannot force engagement. The escape hatch exists because forced learning creates resistance, not growth.

### Not All AI Use Is Equal

The takeaway is not "AI is bad for learning." It's that passive AI use (delegation, offloading) hurts learning, while active AI use (inquiry, explanation-seeking, hypothesis-testing) supports it. The goal is to make active use the default.
