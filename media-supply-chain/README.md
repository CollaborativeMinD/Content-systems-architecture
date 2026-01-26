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

### 🔄 2. The ETL Integration Workflow

**​Phase A**: Extract (Generation)
​Execute: Run the System Prompt in ChatGPT-4 or Claude 3.
​Validate: Review the <REVIEW> scores in the output. Reject any batch where self-rating averages below 8.5/10.

**​Phase B**: Transform (Serialization)
​Serialize: Copy the validated Markdown Table into Google Sheets.
​Sanitize: Check for "hanging quotes" or special characters that might break CSV parsing.

​Export: Download as .csv (Comma Separated Values).

​**Phase C**: Load & Render (Canva API)
​Target: Open Canva Video Project (Mobile Vertical 1080x1920).
​Map:
​Select Text Element → Connect Data → Quote_Column.
​(Optional) Select Background Element → Connect Data → B-Roll_ID.
​Render: Execute "Bulk Create" to generate 100 pages.
​Load: Batch download as individual .mp4 files.

## ​📝 Architect's Note

​This pipeline demonstrates the "Force Multiplier" effect of combining LLM logic with legacy batch-processing tools. By treating video frames as data containers, we decouple creative effort from production volume.
