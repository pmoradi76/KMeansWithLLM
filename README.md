# k-Means Workshop: Customer Segmentation

This repository contains a **Jupyter Notebook** for teaching *k-Means clustering* using a simple customer segmentation example.  
It is designed to support **interactive workshops** (e.g., VU Block Model classes), where students engage in pre-class preparation, in-class activities, and post-class reflection.  

---

## 📊 Dataset

We use a **synthetic Customers dataset** with 10 rows and three features:  

- **Age** (years)  
- **Annual Income (k$)**  
- **Spending Score (1–100)** → a relative score indicating how much a customer tends to spend (higher = frequent/high-value shopper, lower = occasional/low-value shopper).  

The dataset is small and easy to visualise in 2D (Income vs. Spending Score), making it ideal for class discussion.  

---

## 🎯 Learning Objectives

By the end of the activity, students will be able to:  

1. **Differentiate Classification vs Clustering** with real-world examples.  
2. Define a **cluster** and understand the **objective function** of k-Means:  
   \[
   J = \sum_{i=1}^{k} \sum_{x \in C_i} ||x - \mu_i||^2
   \]  
   where \( \mu_i \) is the centroid of cluster \(i\).  
3. Run and visualise k-Means clustering for **k=2, k=3, k=4**.  
4. Discuss **how to choose k** (intuition, elbow method, silhouette score).  
5. Understand **limitations of k-Means** (spherical clusters only, sensitivity to outliers, must predefine k).  
6. Practise **responsible AI use with LLMs** (what to share vs. what not to share).  

---

## 🏫 Teaching Flow

- **Pre-class activity**  
  - Watch a short video on clustering.  
  - Review notes on supervised (classification) vs unsupervised (clustering).  
  - Try a simple LLM prompt:  
    *“Explain customer clustering as if I were a high-school student, using a shopping mall example.”*  

- **In-class activity**  
  1. Show dataset scatter plot → ask: *“How many clusters do you see?”* (students vote via Padlet/Mentimeter).  
  2. Reveal k=2, k=3, k=4 cluster results using k-Means.  
  3. Discuss good vs. bad clusters.  
  4. Explore the **objective function** and algorithm steps.  
  5. Integrate **LLMs in teaching and learning**:  
     - Teacher uses LLM to explain steps interactively.  
     - Students design prompts and test outputs.  
  6. Responsible AI discussion: three scenarios for using LLMs  
     - ✅ Schema + synthetic data allowed  
     - ⚠ Schema only  
     - 🚫 No schema or data (generic practice prompts only)  

- **Post-class activity**  
  - Read about cluster evaluation (Elbow & Silhouette).  
  - Reflection task: *“What did the LLM get right/wrong when explaining clustering? How did you validate it?”*  

---

## ⚙️ Installation & Running

Clone this repo and set up a Python environment:  

```bash
git clone https://github.com/<YOUR_USER>/kmeans-workshop.git
cd kmeans-workshop
python -m venv .venv
source .venv/bin/activate    # Windows: .venv\Scripts\activate
pip install -r requirements.txt
pip install jupyter
jupyter notebook
