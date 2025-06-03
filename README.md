# FLAIRS-38 Tutorial: Breaking Machine Learning Models with Adversarial Attacks and its Variants

**Presenter:** Pavan Reddy  
**Library:** [Adversarial Lab](https://github.com/pavanreddy-ml/adversarial-lab)  
**Colab Notebooks:** See the `notebooks/` folder.  
📌 **IMPORTANT:** In Colab, go to `Runtime > Change runtime type` and select **GPU (T4)**.

---

## 🧠 Overview

This tutorial provides an in-depth guide to adversarial machine learning with a mix of theory and hands-on coding. You'll learn how to:
- Understand the fundamentals of adversarial robustness
- Execute white-box and black-box attacks
- Analyze the implications of adversarial vulnerabilities
- Use `Adversarial Lab`, a framework-agnostic toolkit supporting both PyTorch and TensorFlow

---

## 📚 Tutorial Flow

### 🧩 Part 1: Introduction & Motivation
- What are adversarial examples?
- Real-world examples: stop signs, hidden voice commands, adversarial T-shirts
- Why robustness matters: implications in safety-critical systems
- Key terminology (perturbations, white-box vs. black-box, targeted vs. untargeted attacks)

### 🏗️ Part 2: ML Foundations Refresher
- Supervised learning, loss functions, and gradients
- How input gradients can be used to "train" the input
- Visualizations of decision boundaries and misclassifications

### ⚙️ Part 3: Custom Attack Method
- The core attack method used in the tutorial
- Perturbation visualization and intuition
- Advantages of the method

---

## 💣 White-Box Attacks (Hands-On)

White-box attacks assume full access to the model.

### Attacks Covered:
- **FGSM (Fast Gradient Sign Method)**
- **PGD (Projected Gradient Descent)**
- **CW (Carlini & Wagner)**
- **DeepFool** (minimal perturbation finder)
- **SmoothFool** (low-frequency, transferable perturbations)

### Concepts:
- Gradients, perturbation norms, target vs. untargeted attacks
- Visualization of optimization and perturbation processes

---

## 🕳️ Black-Box Attacks (Hands-On)

Black-box attacks assume only API-level access (input-output).

### Techniques:
- **ZOO (Zeroth Order Optimization)** – gradient-free optimization
- **Transfer Attacks** – adversarial examples from a surrogate model
- **Boundary Attack** – decision-based method with label-only feedback
- **Square Attack** – random search via localized patches

---

## 🧪 Additional Adversarial Techniques

- **Data Poisoning** (label flipping, backdoor injection)
- **Universal Perturbations**
- **Adversarial Patch Attacks**
- **Membership Inference**
- **Model Inversion/Extraction**
- **One-Pixel Attack**
- **Attacks in Other Domains:** audio, reinforcement learning, graphs, 3D

---

## 🛡️ Defenses and Mitigations

- **Adversarial Training** – most effective, robust boundaries
- **Input Preprocessing** – compression, blurring, feature squeezing
- **Certified Defenses** – provable robustness
- **Runtime Detection** – anomaly-based detection
- **Model Ensembles & Randomization** – reduce attack success
- **Prompt Filtering** (for LLMs)

---

## 📈 Why This Matters

- Drives understanding of how models interpret data
- Informs policy, regulation, and AI safety standards
- Enables better red teaming and robust system design
- Provides new tools for data augmentation and privacy auditing

---

## 📦 Setup & Requirements

- Laptop with internet and browser access
- Google Colab (ensure GPU is not already exhausted)
- No local installation required — all dependencies handled in notebooks
- Printed or digital reference material will be provided (if allowed)

---

## 🧰 About Adversarial Lab

**Adversarial Lab** is a unified, framework-agnostic Python library for adversarial ML.  
Supports **TensorFlow** and **PyTorch**.  
Enables fast prototyping of new attacks and defenses.

---
