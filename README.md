# FDIC Regulatory Loan Reasoning Assistant  
**Prompt-Engineered, Regulation-Aligned LLM System**

This project implements a **regulatory reasoning assistant** designed to operate strictly within the **FDIC RMS Manual of Examination Policies – Section 3.2 (Loans)**.  
The system demonstrates how **prompt engineering alone (no fine-tuning)** can constrain a Large Language Model (LLM) to produce **examiner-aligned, non-hallucinated, and policy-compliant regulatory reasoning**.

The assistant provides **regulatory considerations only** and explicitly avoids making **loan approval, rejection, scoring, or pricing decisions**.



## Project Objective

Banks operate under strict regulatory supervision. This project explores how **structured prompt engineering and constraint enforcement** can be used to:

- Encode regulatory policy into machine-readable constraints  
- Enforce examiner-oriented reasoning behavior  
- Prevent prohibited outputs such as loan decisions or unsupported rules  
- Ensure faithful responses grounded in a **single regulatory source of truth**



## Core Capabilities

- Prompt-controlled regulatory reasoning aligned with **FDIC Section 3.2**
- Structured extraction of loan data from **text and images**
- Examiner-style responses focused on **process quality and risk identification**
- Explicit refusal of prohibited actions (loan approvals, scoring, thresholds)
- Scope classification to prevent unnecessary refusals
- Professional chatbot interface for interaction

---

## System Architecture Flow

```text
Loan Application (Text / Image)
        ↓
Structured Data Extraction (JSON, No Inference)
        ↓
Scope Classification (IN / OUT of FDIC Supervision)
        ↓
Prompt-Constrained Regulatory Reasoning
        ↓
Examiner-Oriented FDIC Section 3.2 Analysis
```
## How to Run the Project (Google Colab)

This project is implemented using Google Colab to simplify setup and execution.

**Step 1 — Open the Notebook**

Open the project notebook in Google Colab.

**Step 2 — Install Dependencies**

Run the first cell to install the required libraries.

!pip install openai
!pip install pillow
!pip install pytesseract

**Step 3 — Configure API Key**

Add your API key securely.

import os
os.environ["OPENAI_API_KEY"] = "your_api_key_here"

**Step 4 — Run the Pipeline Cells**

Execute the notebook cells sequentially to:

    1.Load regulatory prompts

    2.Perform structured data extraction from loan input

    3.Classify regulatory scope

    4.Generate FDIC-aligned regulatory reasoning

**Step 5 — Provide Input**

You can test the system with:

     1.Loan application text

     2.Loan document images

The system will extract structured loan information and produce FDIC Section 3.2 regulatory considerations.
## Regulatory Scope

This assistant is restricted to:

FDIC RMS Manual of Examination Policies
Section 3.2 — Loans

All reasoning must remain grounded in this section to ensure policy fidelity and regulatory integrity.
