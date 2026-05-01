### Aaweg Bhaladhare

I build evaluation harnesses and agent infrastructure. Pune, India — open to remote.

Currently looking for **AI Product Owner / Forward-Deployed / LLM-eval** roles where the day-one job is "make the model honest about what it doesn't know."

---

#### What I'm working on

**[`priorityjudge`](https://github.com/Aawegg/priorityjudge)** — a multi-pass agent that grades plans and PRDs on priority-definition quality. Extractor → 5 independent dimension scorers → deterministic citation verifier → synthesizer. Built for the Cursor-based APO recruiting quest.

> **9887 / 10000** on a hand-rated calibration set. Spearman ρ = 1.0 against the human ranking. 96.5% citation precision (the verifier caught the 3.5% the LLM hallucinated). Test-retest CV = 0.4%.

The win comes from architecture, not the model. A single-shot Gemini baseline with the same rubric and same calibration set is the head-to-head ablation, run by [`benchmarks/run_baseline.py`](https://github.com/Aawegg/priorityjudge/blob/main/benchmarks/run_baseline.py).

#### Selected work

- **[`priorityjudge`](https://github.com/Aawegg/priorityjudge)** — APO-native plan scorer with verified citations. Python, Gemini, OpenClaw skill, GitHub Actions CI, Docker.
- **[`nibblecore`](https://github.com/Aawegg/nibblecore)** — 4-bit quantization kernels for Apple Silicon, benchmarked against `llama.cpp`. C++ / SIMD / Metal.
- **[`Story-Character-Extractor`](https://github.com/Aawegg/Story-Character-Extractor)** — RAG pipeline that pulls structured character profiles from short stories. Embeddings + vector DB + LLM extraction.
- **[`Melody-Generation-using-LSTM`](https://github.com/Aawegg/Melody-Generation-using-LSTM)** — LSTM trained on monophonic MIDI to generate new melodies in the same idiom.

#### Background

Ex-Turing AI evaluation team-lead — designed grading rubrics, spotted reward-hacking, and rewrote prompts that bumped agreement from "throw darts" to "actually scores reasoning". I care most about the boring half of agent work: making outputs measurable, falsifiable, and hard to fake.

Hardware-friendly software is the other half. `nibblecore` is what happens when "make inference cheap on the laptop you already own" turns into a side quest.

#### Stack I reach for

Python (pydantic, pytest, click) · Gemini / Anthropic / OpenAI APIs · OpenClaw multi-agent orchestration · Cursor with custom rules · C++17 / SIMD / Metal · Next.js for the rare time a UI is the right answer.

#### Reach me

[LinkedIn](https://linkedin.com/in/aaweg-bhaladhare) · `aaweg.22110711@viit.ac.in`
