# Assignment Plagiarism Intelligence Agent (AICTE – IBM SkillsBuild Internship)

An Agentic AI academic integrity assistant built exclusively on **IBM watsonx Orchestrate**, **IBM Granite (`ibm/granite-3-8b-instruct`)**, and native **Retrieval-Augmented Generation (RAG)** to evaluate student assignments against institutional course material.

## Author Details
* **Name:** Praveenkumar
* **Specialization:** Computer Science Engineering (Cyber Security)
* **Program:** AICTE – IBM SkillsBuild Virtual Internship on Agentic AI
* **Problem Statement:** PS-10 — AI-Driven Plagiarism Intelligence for Student Assignments

## IBM Technology Stack
* **Orchestration:** IBM watsonx Orchestrate
* **Foundation Model:** IBM Granite (`ibm/granite-3-8b-instruct`)
* **Knowledge Grounding (RAG):** watsonx Orchestrate Native Knowledge Base (`course_reference_notes.txt`)
* **Authentication & Cloud:** IBM Cloud IAM

## Agent Workflow (`agent_workflow.json`)
1. **Input Ingestion:** Accepts student assignment excerpts and course context.
2. **RAG Knowledge Retrieval:** Searches uploaded `course_reference_notes.txt` for verbatim and semantic overlap.
3. **IBM Granite Reasoning:** Computes an Originality Score (`0%–100%`), identifies overlapping passages, and drafts citation recommendations.
4. **Ethical Guardrail Output:** Returns a structured four-part report with a mandatory faculty-review disclaimer.

## Repository Contents
* `agent_workflow.json` — Agent architecture and orchestration workflow definition
* `Assignment_Plagiarism_Intelligence_Agent.pptx` — 16-slide project presentation
* `course_reference_notes.txt` — RAG reference knowledge source
* `problem_statement.txt` — Formal PS-10 problem specification