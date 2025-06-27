# MultiModalBench
A Lightweight Benchmark Suite for Multimodal AI
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Docker](https://img.shields.io/badge/ready-to-run-docker-compose-brightgreen)](#quick-start)
[![Streamlit Cloud](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://your-live-demo.streamlit.app)

---

## ✨ Key Features
| Category | What you get | Why it matters |
|----------|--------------|----------------|
| **Plug-and-play models** | One-line `huggingface_hub` or local `.pt/.safetensors` loading | Compare any vision, text, or audio model without code changes |
| **Unified datasets** | `datasets/` hosts standardized JSON/Parquet for <br>‒ *Images*: COCO-10k subset <br>‒ *Text*: WikiText-2 <br>‒ *Audio*: LibriSpeech-mini | No more mismatched file formats |
| **Holistic metrics** | Quality → `BLEU`, `ROUGE`, `FID`, `CLIP-Score`  <br> Efficiency → latency / peak VRAM via *PyTorch Profiler*  | Mirrors Stanford HELM & DAWNBench philosophy |
| **Web leaderboard** | Auto-generated Streamlit dashboard with sortable tables, latex plots, and downloadable CSV | Share results with a URL instead of a PDF |
| **Docker-first** | `docker compose up` → reproducible GPU environment in 5 min | Same scores on any workstation or cloud |

---

## 🖥️ Quick Start

```bash
# 1. Clone
git clone https://github.com/your-handle/multibench && cd multibench

# 2. Spin up full stack (API + Streamlit) – requires NVIDIA GPU
docker compose up --build

# 3. Open dashboard
