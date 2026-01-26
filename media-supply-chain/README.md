# Module: Automated Media Supply Chain

### ⚡ System Overview
**Status:** Production (Legacy v2.1)  
**Throughput:** 100+ Assets / Hour  
**Infrastructure:** Serverless / Low-Code (OpenAI, Google Sheets, Canva)

### 🎯 Architecture Goal
To decouple **Creative Direction** from **Production Rendering**. This system utilizes an ETL (Extract, Transform, Load) pattern to generate high-volume social media assets without sacrificing brand fidelity or incurring variable costs.

### 🧩 Technical Stack
* **Extraction Layer:** Large Language Models (LLM) with Recursive QA prompting.
* **Transformation Layer:** CSV Middleware for data serialization and sanitization.
* **Rendering Layer:** Bulk-Create API (Canva) for data mapping and batch export.

### 📊 Performance Data
| KPI | Manual Workflow | Automated Pipeline | Delta |
| :--- | :--- | :--- | :--- |
| **Time-to-Publish** | 45 mins / Asset | 0.6 mins / Asset | **98% Faster** |
| **Error Rate** | High (Fatigue) | Near-Zero (Deterministic) | **Improved** |
| **Cost** | $15-$50 / Asset | ~$0.00 / Asset | **Free Tier** |

---

### 📜 Directory Contents
* `bulk_video_pipeline.md` - Full architectural documentation, system prompts, and integration steps.
