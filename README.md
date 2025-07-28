README.md
# Fabric Forks

**Fabric Forks** is the **official public registry** for all **forkable agents, AI models, and royalty-enabled assets** built on the **Fabric 1.0 Universal AI Fabric** platform.

This repository powers the **Fabric agent economy**, enabling developers to:
- 📦 **Publish** new AI models and agents for the Fabric ecosystem  
- 🌱 **Fork** existing agents to build upon proven execution lineages  
- 💎 **Earn royalties** and XP as your forks are reused globally  
- 🧾 **Track provenance** for every agent and model version  

---

## 📂 Directory Structure

fabric-forks/
├── edge-vision-v2/
│ ├── 1.0.0/
│ │ ├── model.yaml
│ │ ├── weights/
│ │ └── training/
│ └── 1.1.0/
│ ├── model.yaml
│ └── ...
├── agent-repacker/
│ ├── 1.0.0/
│ └── 1.1.0/
└── ...


- Each agent/model is stored in a dedicated folder  
- Semantic versioning: `MAJOR.MINOR.PATCH`  
- Each version contains:
  - `model.yaml` — Manifest (metadata, provenance, royalty rules)  
  - `weights/` — Model weights and binaries  
  - `training/` — Scripts, datasets, reproducibility files  

---

## 🚀 Publishing a New Model

1. Prepare your model directory following the structure above  
2. Validate your manifest:
   ```bash
   fab model validate path/to/model.yaml
Submit a PR to add your model or use the CLI:
fab model publish models/my-agent/1.0.0/model.yaml
Once merged, your model is publicly forkable and royalties are tracked automatically
🔐 Provenance and Royalties

Every fork generates:
XP for the original developer
Royalty payouts tracked by fab-treasury
Provenance is enforced via Fabric’s audit trail and policy kernel
🛠️ Tools

fab model validate — Verify manifest compliance
fab model publish — Push models to this registry
fab claim — Claim royalties from forks
📜 License

Apache 2.0 — Fabric is free and open-source.
Developers earn revenue only through forks and royalty flows.

