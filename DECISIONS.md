# Decisions

## Decision 1: Why this project (2026-11-10)
- Why I chose to build a RAG system with an evaluation harness:
- What "success" means in numbers (a guess is fine, I will revise it):
- What I expect to be the hardest part: how to wrie these and answer in notepad

Why I Chose This Project - Most students focus only on building the project. I want to build one that actually works and shows numbers, not one that I trust blindly. I will compare each method myself so I know which works better for which kind of query. That will make me sharper when I make decisions in production later, and it will give me a chatbot that answers real questions well.

What success means in numbers - Success is easier to judge when it has two parts, a quality target and a comparison target

The best method answers at least 40 of my 50 questions correctly (80%).
The best method beats the simple-chunking baseline by at least 10 percentage points.
The correct source chunk appears in the top 5 retrieved results for at least 85% of questions.
In offline mode, the local model answers in under 10 seconds on my laptop.
These are guesses. I will revise them after the first results and note why.

What I expect to be the hardest part - Writing 50 good questions with correct answers by hand, because they need to cover different kinds of queries (exact facts, vague questions, questions that need several sections) and I have to find each answer myself. The second hard part is deciding how to judge whether the chatbot’s answer is correct, because two answers can be worded differently and both be right.