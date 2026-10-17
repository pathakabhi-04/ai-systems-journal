# AI Systems Journal

Learning log for AI agent efficiency and system design. Third-year CS, started October 2026.

Background: computer vision, NLP, machine learning, deep learning. What I'm adding here is
LLM engineering, agent orchestration, and the system design that surrounds both.

## What's in here

| Folder | What it holds |
|---|---|
| [`00-foundations/`](00-foundations/) | Small exercises: serving models, tool calling, eval harnesses, cost logging |
| [`01-design-sketches/`](01-design-sketches/) | One system design problem a week, sketched in 20 minutes then critiqued |
| [`02-prompt-library/`](02-prompt-library/) | Prompts I reuse, refined over time |
| [`03-weekly-log/`](03-weekly-log/) | What I built each week, what it cost in tokens, what I'd do differently |

## Projects

Each lives in its own repository.

| Project | What it shows | Repo |
|---|---|---|
| LLM cost router | A classifier routes easy queries to a cheap model, hard ones to a strong model. Cost vs quality measured against always using the strong model. | _not started_ |
| Vision + LLM pipeline | A CV pre-stage crops and extracts so the LLM sees a small region instead of a full image. | _not started_ |
| RAG with measured retrieval | Retrieval, reranking and caching as separate designed components, scored against a real eval set. | _not started_ |
| ML agent from scratch | Plan, act, observe over a CSV and a goal, with a hard cost cap and context management. | _not started_ |

## The idea

Low token count isn't the goal. Efficiency plus judgment is: a correct, verified result without
flailing. Every technique that cuts tokens turns out to be a system design decision — filtering
before an expensive stage, caching, routing, managing state. So every project here ends with an
architecture diagram and a table of cost against quality.
