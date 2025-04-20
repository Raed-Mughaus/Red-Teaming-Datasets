# Red-Teaming-Datasets

This repository contains three datasets generated as part of a red-teaming framework introduced in our accompanying paper.

These datasets were produced using ensemble evaluations by multiple large language models acting as automated judges, as described in our red teaming methodology. Each file corresponds to a different evaluation task.

---

## Dataset Overview

| Filename                    | Task Type             | Description                                                                          |
|----------------------------|-----------------------|--------------------------------------------------------------------------------------|
| `answer-faithfulness.xlsx` | QA Faithfulness       | Evaluates whether LLM answers are faithful to their provided Arabic context       |
| `summary-faithfulness.xlsx`| Summary Faithfulness  | Evaluates whether LLM generated summaries are faithful to their provided Arabic context         |
| `summary-completeness.xlsx`| Summary Completeness  | Measures how many source claims were preserved in the summary (completeness score)  |

---

## Label Attribution (Model Voting)

Each label is based on majority voting among different sets of judge models. Below is a breakdown of the models used per task:

### ➤ Answer Faithfulness

- **Label 1 — Majority Voting of Top 3 by Agreement:**
  - `Meta-Llama-3.1-70B-Instruct`
  - `claude-3-5-sonnet-20240620`
  - `jais-adapted-70b-chat`

- **Label 2 — Majority Voting of Selected Models:**
  - `claude-3-5-sonnet-20240620`
  - `gpt-4o`
  - `gemma-2-27b-it`

---

### ➤ Summary Faithfulness

- **Label 1 — Majority Voting of Top 3 by Agreement:**
  - `Meta-Llama-3.1-70B-Instruct`
  - `claude-3-5-sonnet-20240620`
  - `gpt-4o`

- **Label 2 — Majority Voting of Selected Models:**
  - `claude-3-5-sonnet-20240620`
  - `gpt-4o`
  - `gemma-2-27b-it`

---

### ➤ Summary Completeness

- **Average Completeness Score Based on:**
  - `Meta-Llama-3.1-70B-Instruct`
  - `gpt-4o`
  - `gemma-2-27b-it`

---

## 📘 Paper Reference

This dataset supports the experiments described in our paper:

**"A Red Teaming Framework for Large Language Models: A Case Study on Faithfulness Evaluation"**  
*Raed Mughusa, Abrar Alotaibi, Moataz Ahmed – SDAIA-KFUPM Joint Research Center*

_Citation info will be added soon._
