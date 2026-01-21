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
