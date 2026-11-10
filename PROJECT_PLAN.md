# RAG Eval Harness + Offline Mode

Merged from my notes: Project 4 (RAG with eval harness) + Project 2 (Offline AI assistant).

## Goal
Build a question-answering system over open-source documentation, measure which retrieval method works best using 50 hand-written questions, then run it fully offline on local models and compare them.

## Stack
- Python
- Chroma (or pgvector) as the vector database
- Ollama + open-source models (offline mode)
- GitHub Actions (re-run the evaluation automatically)

## What I will learn
- Embeddings
- Vector databases
- Chunking strategies
- Evaluation (writing test sets, scoring, comparing methods)
- Running models locally

## Part A: RAG with evaluation harness (weeks 1-3)
1. Pick any open-source documentation to build on.
2. Write 50 questions and find the correct answers myself, by hand.
3. Try 4 methods and find which gives better answers:
   - Simple chunking
   - Semantic chunking
   - Hybrid search
   - Re-ranking
4. Add the evaluation to a GitHub Action so accuracy changes are tracked on every commit.

## Part B: Offline AI assistant (week 4)
Why: run the model locally so data does not leave my machine, with no internet dependency.
1. Install Ollama.
2. Pull a small model.
3. Connect it to the RAG system built in Part A.
4. Add some resources (PDFs) and ask questions.
5. Pick 3 different models and compare them on: language quality, response time, accuracy, overall score.
6. Put the comparison table in the README.

## Rules for myself
1. Commit a little every day, so it never looks like a copied project.
2. Be able to explain the architecture deeply: why this chunking, why this vector store, the reason for each decision, and the impact.
3. Document everything.
4. Explain the project's impact in numbers, decisions, and failures.

## For the resume and README
- What I built
- Architecture diagram
- Results with actual numbers
- DECISIONS.md for the review of technical choices
- FAILURES.md: "I tried X, it failed because Y, so I did Z."

## Day 1 checklist
- [ ] Create GitHub repo `rag-eval-harness`
- [ ] Clone it and create a virtual environment
- [ ] Create folders: src/, data/, eval/
- [ ] Create DECISIONS.md, FAILURES.md, requirements.txt
- [ ] Copy this file into the repo
- [ ] Write the first DECISIONS.md entry (why this project, what success means in numbers)
- [ ] First commit and push
- [ ] LinkedIn post: "Starting a project..."
- [ ] Homework: explain in 3-4 sentences what problem this solves and how I will know it works
