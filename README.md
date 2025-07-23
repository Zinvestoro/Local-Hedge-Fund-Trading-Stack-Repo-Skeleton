# Local Hedge‑Fund Trading Stack

This repository houses a self‑contained, multi‑container quantitative‑trading lab that can run entirely on an RTX 4070 workstation.

* **Data Ingestion ** – Apache Kafka 3 + QuestDB 9.
* **Backtests** – NautilusTrader (Rust/Python) & ABIDES.
* **ML / RL** – PyTorch 2.2 + FinRL‑DeepSeek.
* **Observability** – Prometheus + Grafana + Loki.

## Quick start
```bash
# build and start everything
make up            # or:  docker compose up -d --build

# tear down
make down
