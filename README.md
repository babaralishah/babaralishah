# Babar Ali Shah

**ML Research Engineer · Dublin, Ireland**
**PhD Applicant — Trustworthy Generative AI, Retrieval-Augmented Systems, Answerability**

[Portfolio](https://babaralishah.github.io) · [LinkedIn](https://www.linkedin.com/in/babar-ali-shah-data-scientist/) · [ORCID](https://orcid.org/0009-0007-2002-3735) · [Zenodo](https://doi.org/10.5281/zenodo.21101145) · [Email](mailto:syedbabar957@gmail.com)

---

## About

I'm a machine learning research engineer working at the intersection of retrieval-augmented generation and trustworthy AI — specifically, the problem of **answerability**: how a system can tell whether it has enough grounding to answer a query reliably, and when it should abstain instead of guessing.

Over the past three years I've built RAG pipelines end to end — chunking, embedding, hybrid retrieval, reranking, generation, and evaluation — and worked under contract via [Turing](https://www.turing.com) on evaluation, red-teaming, and dataset-design projects supporting AI training programmes at Amazon, Google, and Salesforce. I'm now applying to PhD programmes to study answerability and abstention formally, rather than as an engineering afterthought.

## Research questions I keep coming back to

- To what extent do retrieval-side design choices — chunking, hybrid search, reranking — determine the answerability of a query in a heterogeneous knowledge base?
- Under what conditions should a production LLM withhold a response rather than generate an uncertain or hallucinated answer?
- What are the systematic failure modes of frontier language models under adversarial input perturbation?
- How reliably do language model agents plan and execute multi-step tool use under ambiguous constraints?

## Featured projects

### [rag-stack](https://github.com/babaralishah/rag-stack) — a fully local RAG system
Ollama · sentence-transformers · FAISS · FastAPI · Streamlit · Docker

A document question-answering system that runs entirely on local infrastructure, with no paid APIs. Ingests PDFs, chunks with overlapping windows, retrieves via a persistent FAISS index, and generates grounded answers with source citations (file, page, snippet). The part most relevant to my research: a similarity-threshold guardrail that returns "I don't know" when retrieval confidence is too low, rather than forcing an answer.

→ [Live demo on Hugging Face Spaces](https://babaralishah-rag-llm-app.hf.space/)

### Modular RAG ablations — chunking, retrieval, reranking
Hybrid BM25 + dense retrieval · cross-encoder reranking · Gemini API

A self-directed ablation study varying chunking strategy, embedding model, retrieval architecture, and reranking method independently, isolating their effect on retrieval quality and answer faithfulness. Found hybrid retrieval consistently outperforms single-modality retrieval on corpora with high vocabulary mismatch — the empirical basis for the manuscript below.

## Publications

**["What Improves RAG? A Controlled Ablation Study of Retrieval Augmentation Strategies in Biomedical Question Answering"](https://doi.org/10.5281/zenodo.21101145)**
Shah, B.A. (2026). Zenodo preprint (not peer-reviewed).
A systematic ablation across five retrieval configurations and eight retrieval metrics, showing where hybrid retrieval and neural reranking help, and where keyword-expansion strategies degrade semantic retrieval baselines.

## Applied research experience (contract work via Turing)

| Project | For | Focus |
|---|---|---|
| LLM Abstention & Answerability Evaluation | Amazon Nova | Multi-turn abstention corpora, instruction-following evaluation |
| Adversarial Robustness & Red-Teaming | Amazon Nova | Failure taxonomy: hallucination, instruction drift, safety evasion |
| Agentic Reasoning & Tool-Use Benchmarking | Salesforce (Tau-Bench) | Multi-step agent evaluation tasks, banking domain |
| Multimodal Bias Evaluation & SFT Dataset Design | Google Gemini | Bias/alignment evaluation, function-calling SFT datasets |

Full write-ups, methodology, and findings for each: [babaralishah.github.io](https://babaralishah.github.io)

## Currently

Studying evaluation methodologies for large vision-language models, and preparing PhD applications on answerability prediction in retrieval-augmented systems.

## Open to

Collaboration on open-source LLM evaluation frameworks, RAG benchmarking, or joint work with researchers and PhD applicants in trustworthy generative AI.

## Skills

**Research & evaluation:** experimental design, ablation studies, benchmark construction, annotation protocols, adversarial testing, error analysis
**RAG & retrieval:** FAISS, BM25, hybrid search, query rewriting, cross-encoder reranking, chunking strategies
**LLM alignment:** RAGAS, SFT, RLHF, red-teaming, hallucination mitigation
**Engineering:** Python, SQL, JavaScript, Docker, AWS, GCP, PostgreSQL, MongoDB, ClickHouse, Airflow

---

<sub>Dublin, Ireland · syedbabar957@gmail.com</sub>
