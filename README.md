# 🌌 AURORA: Autonomous Integrated OS (AIOS) Framework

**Aurora** is a modular system architecture designed for Termux/Linux environments, bridging high-level LLM logic with low-level system orchestration.

## 🚀 Key Features
- **Neural Memory (FAISS):** Persistent vector memory using Sentence-Transformers for semantic recall.
- **Phase-Based Orchestration:** A sophisticated startup sequence ensuring system stability and security.
- **Telemetry-Driven Logic:** Real-time monitoring (CPU, RAM, Battery) influencing AI behavior.
- **Speech Integration:** Native Termux:API hooks for voice-command processing.

## 🛠️ Architecture
The system consists of two primary layers:
1. **The Bridge (Python):** Handles the "thinking," vector embedding, and state management.
2. **The Orchestrator (Bash):** Handles the "body," ensuring all services start in the correct order.

## 📂 Project Structure

```
aurora-/
├── demos/
│   ├── bridge_demo.py          # Simplified neural bridge showcase
│   └── orchestrator_demo.sh    # Phase-based system startup demo
├── aurora/
│   ├── scripts/                # Full production modules (50+)
│   └── ...
├── README.md
└── requirements.txt
```

## 🎯 Quick Start (Demo Mode)

### Prerequisites
```bash
pkg install python faiss clang -y
pip install sentence-transformers numpy
```

### Run the Neural Bridge Demo
```bash
cd demos
python3 bridge_demo.py
```

### Run the Orchestrator Demo
```bash
cd demos
bash orchestrator_demo.sh
```

## 💡 Demo vs Production

| Feature | Demo | Production |
|---------|------|------------|
| Modules | 2 core files | 50+ integrated scripts |
| LLM | Sentence-BERT (384D) | Custom Slovak LLM (12L/512D) |
| Memory | FAISS vector store | Multi-tier persistent storage |
| Orchestration | 5-phase startup | Advanced health monitoring + auto-healing |
| Corpus | Demo phrases | 10GB Slovak language corpus |

## 🧠 How It Works

### The Neural Bridge
The bridge uses **Sentence-BERT embeddings** to encode system thoughts into a **FAISS vector database**, enabling semantic memory recall across sessions.

```python
# Simplified concept
vector = embedder.encode(["System reached awareness"])
index.add(vector)  # Persistent memory
```

### The Orchestrator
A bash-based orchestration system that starts services in phases:

1. **Phase 0:** Core heartbeat & memory checks
2. **Phase 1:** Security (firewall, auto-defense)
3. **Phase 2:** Observability (logs, kernel monitoring)
4. **Phase 3:** Brain (data analysis, JSON processing)
5. **Phase 4:** Network (IoT, API monitoring)
6. **Phase 5:** Healing & meta-control

## 🔬 Research Context

This project represents exploration into:
- **Self-modifying systems** that evolve based on telemetry
- **Semantic memory architectures** for long-term AI coherence
- **Slovak language model fine-tuning** on Android hardware constraints

Built entirely on **Android/Termux** as proof that advanced AI systems don't require cloud infrastructure.

## 📊 Technical Stack

- **Python 3.10+**
- **FAISS** (vector similarity search)
- **Sentence-Transformers** (all-MiniLM-L6-v2)
- **Bash** (orchestration scripting)
- **Termux:API** (Android integration)

## 🤝 Contributing

This is a personal research project. While the demo code is open for educational purposes, the production system remains private.

## 📜 License

MIT License - See LICENSE file for details.

## 🎓 Academic Notice

If you reference this work in academic research, please cite:
```
@software{aurora_aios_2026,
  author = {Rado (mefoku52-cmyk)},
  title = {AURORA: Autonomous Integrated OS Framework},
  year = {2026},
  url = {https://github.com/mefoku52-cmyk/aurora-}
}
```

---

**Built on 📱🇸🇰 | Termux + Python + Bash**
