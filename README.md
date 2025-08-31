# Using LLMs to Explain k-Means Clustering

This repository contains a simple **Jupyter Notebook** that demonstrates how to use **Large Language Models (LLMs)** (e.g., ChatGPT) to **explain and teach k-Means clustering**.  

The example is based on a small synthetic **Customer Segmentation dataset**, where each customer is described by:

- **Age** (years)  
- **Annual Income (k$)**  
- **Spending Score (1–100)** → a relative score indicating how much a customer spends (higher = frequent/high-value shopper, lower = occasional/low-value shopper).  

---

## 🎯 Purpose

- Show how **LLMs can provide intuitive explanations** of clustering for different audiences (e.g., “Explain k-Means as if I were a 15-year-old”).  
- Compare **good vs. bad prompts** when asking LLMs about clustering.  
- Use a small dataset to **visualise clusters** and then ask the LLM to explain the algorithm steps.  
- Highlight how to use LLMs **responsibly** (synthetic data only, schema-only prompts, or generic practice prompts).  

---

## 🗂️ Dataset

A small synthetic dataset of 10 customers is embedded directly in the notebook:  

| CustomerID | Age | Annual_Income (k$) | Spending_Score |
|------------|-----|---------------------|----------------|
| 1          | 19  | 15                  | 39             |
| 2          | 21  | 15                  | 81             |
| 3          | 20  | 16                  | 6              |
| 4          | 23  | 16                  | 77             |
| 5          | 31  | 17                  | 40             |
| 6          | 22  | 17                  | 76             |
| 7          | 35  | 18                  | 6              |
| 8          | 23  | 18                  | 94             |
| 9          | 64  | 19                  | 3              |
| 10         | 30  | 19                  | 72             |

---

## 🏫 Example LLM Prompts

- ❌ **Bad Prompt:** `"Explain clustering."` (too vague)  
- 😐 **So-So Prompt:** `"Explain k-Means clustering."` (generic, no context)  
- ✅ **Good Prompt:**  
