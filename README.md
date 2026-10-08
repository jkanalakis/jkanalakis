# John Kanalakis

**Hands-on AI engineering leader.** I build multimodal and LLM systems that run in production and the teams that ship them.

The last five years hands-on in applied AI: video intelligence, vision-language models, fine-tuned LLMs, retrieval systems. The fifteen before that leading engineering at Netflix, Roku, TiVo, and Cisco, where I scaled consumer platforms to millions of users and earned three Primetime Emmy Awards.

San Francisco Bay Area | [jkanalakis@msn.com](mailto:jkanalakis@msn.com) | [linkedin.com/in/johnkanalakis](https://linkedin.com/in/johnkanalakis)

---

## Selected public implementations

These repositories show how I approach model adaptation, retrieval, service design, and media processing. They include source code and documented entry points; maturity varies, and they are not claims of production readiness or independently benchmarked performance.

### [Deep Recall — contextual memory for LLM applications](https://github.com/jkanalakis/deep-recall)

My most substantial public AI infrastructure project: memory, inference, and orchestration components, with semantic retrieval and user-associated memory records.

- **Engineering focus:** PostgreSQL/pgvector storage, FAISS and Qdrant adapters, API authentication components, and separation of retrieval from inference.
- **Inspect the implementation:** [semantic search](https://github.com/jkanalakis/deep-recall/blob/main/memory/semantic_search.py), [storage adapters](https://github.com/jkanalakis/deep-recall/tree/main/memory/vector_db), and [tests](https://github.com/jkanalakis/deep-recall/tree/main/tests).
- **Start exploring:** [Streamlit memory example](https://github.com/jkanalakis/deep-recall/tree/main/examples/streamlit-memories) and [Docker setup](https://github.com/jkanalakis/deep-recall/blob/main/deployments/docker/README.md). [Kubernetes configurations](https://github.com/jkanalakis/deep-recall/tree/main/deployments/kubernetes) and [monitoring configurations](https://github.com/jkanalakis/deep-recall/tree/main/deployments/monitoring) show the deployment approach.

### [Llama fine-tuning — Unsloth and LoRA](https://github.com/jkanalakis/finetuning-llama-model-for-text-generation-using-unsloth)

A concrete supervised fine-tuning experiment with Llama 3.2 3B: 4-bit model loading, rank-16 LoRA adapters, ShareGPT-style data preparation, training, adapter saving, and generation.

- **Engineering focus:** parameter-efficient adaptation with explicit training settings and a checked-in sample dataset.
- **Inspect and reproduce the workflow:** [training notebook](https://github.com/jkanalakis/finetuning-llama-model-for-text-generation-using-unsloth/blob/main/Notebook/fine-tuning-llama.ipynb), [dataset](https://github.com/jkanalakis/finetuning-llama-model-for-text-generation-using-unsloth/blob/main/data/formatted_dataset.json), and [environment setup](https://github.com/jkanalakis/finetuning-llama-model-for-text-generation-using-unsloth/blob/main/README.md). The notebook is the clearest entry point; GPU and dependency compatibility are required.

### [Fast News Rec — semantic retrieval API experiment](https://github.com/jkanalakis/fast-news-rec)

A compact notebook connecting Sentence Transformers embeddings, a FAISS L2 index, and a FastAPI `/recommend` endpoint over a 1,000-article subset of AG News.

- **Engineering focus:** an inspectable path from corpus ingestion to embeddings, indexing, and top-k API responses.
- **Start here:** [implementation notebook](https://github.com/jkanalakis/fast-news-rec/blob/main/FastNewsRecommender.ipynb). The server implementation lives in the notebook rather than a standalone `app.py`.

### [Video Sentiment — media-to-text analysis prototype](https://github.com/jkanalakis/video-sentiment-ollama)

A Streamlit prototype that extracts video audio with FFmpeg, transcribes it through Google Speech Recognition, applies TextBlob sentiment analysis to transcript chunks, and charts the results.

- **Engineering focus:** modular media processing, transcription, analysis, and visualization.
- **Inspect the pipeline:** [application](https://github.com/jkanalakis/video-sentiment-ollama/blob/main/app.py), [audio/transcription](https://github.com/jkanalakis/video-sentiment-ollama/blob/main/transcription_alternative.py), and [sentiment analysis](https://github.com/jkanalakis/video-sentiment-ollama/blob/main/sentiment_analysis.py). This analyzes spoken content; transcription uses an external service.

**Additional experiments:** [PDF retrieval and Q&A with Ollama](https://github.com/jkanalakis/pdf-chat-ollama/blob/main/pdf_chat.py), and [video frame sampling](https://github.com/jkanalakis/video-image-understanding/blob/main/app.py). The latter implements FFmpeg frame extraction and a Streamlit interface; its Janus image-description integration remains a placeholder.

---

## In development: Tunewright

**Tunewright** is an LLM fine-tuning workbench in development, with an open-source direction. The goal is to make model adaptation reproducible and accessible to small teams. No public source repository or demo is linked here yet; the fine-tuning notebook above is available to inspect today.

Also exploring: evaluation methodology for multimodal systems, efficient inference, and parameter-efficient fine-tuning at practical scale.

---

## Background

**AI Researcher & Engineering Leader, Independent** · 2026–Present
Building and publishing open-source AI infrastructure (*see the projects above*) while evaluating senior AI leadership roles.

**Chief Technology Officer, Infactory** · 2025–2026
Architected a production video intelligence platform turning unstructured video into structured data. Orchestrated GPT-4 Vision, Whisper, YOLO, and SigLIP into a unified inference framework with adaptive model routing. Cut 30+ minutes of processing per match via keypoint scene pre-filtering at 95%+ accuracy; reduced compute 80% through optimized frame sampling with no loss in positional precision.

**Founder & Head of AI, Tendi** · 2023–2025
Built an AI-native personal financial advisor to help close the wealth gap. Trained a deep-learning foundation model from scratch with Hugging Face Transformers; extended GPT-4, Llama 3, and Mistral through RAG, fine-tuning, RLHF, and tool use. Deployed on Kubernetes to scale to millions.

**Chief Technology Officer, Crediture** · 2021–2023
AI-driven credit risk assessment using behavioral patterns and alternative data — extending credit access beyond traditional scoring.

**Director of Engineering, Roku** · 2014–2021
Next-generation OTT streaming platform for Pay TV providers, 6M active devices. ML for content recommendation and personalization. *Primetime Emmy Award.*

**Senior Engineering Manager, Netflix** · 2011–2014
Owned the Xbox streaming experience — 9M+ subscribers on Xbox 360 — through the company's shift from disc-by-mail to global streaming. Ran the team as a startup inside Netflix. *Primetime Emmy Award.*

**Senior Engineering Manager, Cisco** · 2009–2011
Built a team from zero and delivered the complete user experience for umi Home Telepresence — HD video conferencing on the living room TV.

**Engineering Manager, TiVo** · 2006–2008
Next-generation HD interface for the embedded Linux platform, international launch in Australia, and the first release of YouTube on TiVo. *Primetime Emmy Award.*

Earlier: EnvyGames (founder), Neoforma, LoanCity, Betasphere, SpinCircuit.

---

## Tech stack

**AI/ML** · PyTorch · Hugging Face Transformers · LangChain · LlamaIndex · CrewAI · scikit-learn · OpenAI GPT · Llama · Mistral · Vertex AI · RLHF · Fine-tuning · RAG · Vector indexing

**Backend** · Python · FastAPI · Node.js · Django · Express.js · REST APIs · Microservices

**Data** · PostgreSQL · MongoDB · MySQL · Redis · Supabase · Firebase

**Infrastructure** · Docker · Kubernetes · AWS · GitHub Actions · Jenkins

**Frontend** · React · Next.js · Vue.js · SwiftUI · Tailwind CSS · Gradio · Streamlit

---

## Also

**5 granted patents** · **2 published books** · **3 Primetime Emmy Awards**

- *Developing .NET Enterprise Applications* — Apress, 2003
- *The Complete Guide to Torque X* — Course Technology, 2008
- ["Web Services & Java Server Pages"](https://www.drdobbs.com) — Dr. Dobb's Journal, 2002
- ["Examining OS/2 2.1 Threads"](https://www.drdobbs.com) — Dr. Dobb's Journal, 1994

---

*Always up for a conversation about applied AI — what's actually working in production, and what isn't yet.*
