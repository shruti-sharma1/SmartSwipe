## 📋 Week 2 Assignment


This Week 2 assignment gives you hands-on practice with the mathematical foundation that powers SmartSwipe. By the end, you'll understand exactly how a machine *learns* from data — which is the core question behind everything we're building.

This week you'll work with:

**Supervised Learning & Regression**
- Understanding the difference between supervised and unsupervised learning
- Implementing linear regression from scratch using only NumPy
- Understanding gradient descent — how a model improves itself iteratively
- Evaluating model performance using R², MAE, and MSE

**Classification & Model Evaluation**
- Understanding what a decision boundary is
- Measuring model quality beyond just accuracy
- Understanding train/test split and why it matters
- Getting intuition for overfitting vs underfitting

Take your time to experiment. Use visualizations to build intuition — a plot often explains more than a formula.

**Submit by: [date]**

---

### 📚 Resources

**Supervised Learning & The ML Workflow**
- 📹 [Machine Learning Fundamentals — StatQuest](https://www.youtube.com/watch?v=Gv9_4yMHFhI) — Start here. Best 15-minute intro to what ML actually is.
- 📄 [What is Supervised Learning? — IBM](https://www.ibm.com/think/topics/supervised-learning) — Covers the core terminology: labels, features, training.
- 📹 [Linear Regression — StatQuest](https://youtu.be/7ArmBVF2dCs) — Intuition first, math second.
- 📄 [Everything About Linear Regression — Analytics Vidhya](https://www.analyticsvidhya.com/blog/2021/10/everything-you-need-to-know-about-linear-regression/) — Solid reference article.

**Gradient Descent — How Models Actually Learn**
- 📹 [Gradient Descent, Step by Step — StatQuest](https://www.youtube.com/watch?v=sDv4f4s2SB8) — The most important video this week.
- 📄 [Gradient Descent Unraveled — Towards Data Science](https://towardsdatascience.com/gradient-descent-unraveled-3274c895d12d/) — Readable walkthrough with visuals.
- 📄 [Types of Optimizers — arxiv](https://arxiv.org/pdf/1609.04747) ⭐ *Only for the curious* — SGD, Adam, and beyond.

**Model Evaluation**
- 📹 [Train/Test Split — StatQuest](https://www.youtube.com/watch?v=fSytzGwwBVw) — Short and essential (~6 min).
- 📹 [Bias/Variance Tradeoff — StatQuest](https://www.youtube.com/watch?v=EuBBz3bI-aA) — Overfitting vs underfitting, explained visually.
- 📄 [Confusion Matrix — Towards Data Science](https://towardsdatascience.com/understanding-confusion-matrix-a9ad42dcfd62) — For when you move from regression to classification.
- 📄 [Why MSE though? — Daily Dose of DS](https://blog.dailydoseofds.com/p/why-mean-squared-error-mse) ⭐ *Only for the curious*

**Features & Representations**
- 📄 [Feature Engineering — Google ML Crash Course](https://developers.google.com/machine-learning/crash-course/representation/feature-engineering) — Read "Qualities of Good Features" section. Directly relevant to SmartSwipe.
- 📄 [What are Embeddings? — Towards Data Science](https://towardsdatascience.com/neural-network-embeddings-explained-4d028e6f0526) — Preview of where we're headed in Week 3.

---

### 🗂️ Task 1 — Dataset Exploration

You've been provided with `dataset.csv`. Before building any model, understand your data.

- Load the dataset using Pandas and inspect its shape, columns, and data types
- Check for missing values and think about how you'd handle them
- Plot distributions of at least 3 features using Matplotlib or Seaborn
- Identify which column you'd use as the **target variable** (what you want to predict) and which as **features** (what you use to predict it)
- Think about which features seem most useful and why — write your reasoning as a comment in the notebook

---

### 🗂️ Task 2 — Linear Regression from Scratch

Implement linear regression **without using sklearn, PyTorch, or any ML library** — only NumPy.

- Implement gradient descent to learn the weights
- Train your model on 80% of the data, test on the remaining 20%
- Plot the **loss curve** (loss vs. number of iterations) to verify your model is learning
- Report MSE and R² score on the test set
- Compare your results with sklearn's `LinearRegression` — they should be close

*The goal isn't a perfect model. It's understanding that learning = repeatedly adjusting weights to reduce error.*

---

### 🗂️ Task 3 — Polynomial Regression & Overfitting

Extend your linear regression to handle non-linear relationships.

- Add polynomial features (degree 2 and degree 5) to your input
- Train a model on each and compare test performance
- Plot predictions for degree 1, 2, and 5 on the same graph
- Answer in your notebook: which degree overfits? How can you tell from the plot?

---

### 🗂️ Task 4 — Logistic Regression + Evaluation

Apply the logistic regression you studied in Week 1 to a classification task. You can use sklearn here.

- Pick a binary classification problem from your dataset (or use `sklearn.datasets.load_breast_cancer()`)
- Split into train/test, fit a `LogisticRegression` model
- Report: accuracy, confusion matrix, precision and recall
- Plot the confusion matrix as a heatmap
- Answer: is accuracy enough to evaluate this model? Why or why not?

---

### 📦 Deliverables

| File | Contents |
|------|----------|
| `week2_exploration.ipynb` | Tasks 1 and 4 — EDA notebook and logistic regression evaluation |
| `linear_regression.py` | Task 2 — Linear regression implemented from scratch |
| `polynomial_regression.py` | Task 3 — Polynomial regression with overfitting analysis |
---
