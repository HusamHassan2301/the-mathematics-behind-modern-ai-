# Chapter 1 — Numbers, Operations, and Why They Matter

---

## Overview

Modern AI systems do not store meaning directly.
They store numbers.

This chapter introduces the numerical foundation of artificial intelligence:

* what numbers are used
* how they are represented
* how operations on them produce learning

Everything in AI — from embeddings to neural networks — begins here.

---

## Core Idea

> Meaning is geometry.
> Geometry is numbers.
> Therefore, meaning is numbers.

---

## Key Questions

* What kinds of numbers exist in computation?
* Why are real numbers (ℝ) essential for AI?
* Why is one number not enough to represent meaning?
* How do simple operations lead to learning?

---

## What You Will Learn

* the difference between integers (ℤ) and real numbers (ℝ)
* floating-point representation (float16, float32, float64)
* vectors as elements of ℝ^d
* embeddings as numerical representations of meaning
* basic arithmetic operations in model training
* how these concepts appear in real AI systems

---

## AI Connection

In modern language models:

1. words are converted into integers (token IDs)
2. integers are mapped into vectors in ℝ^d
3. vectors are processed through layers using arithmetic operations

This transformation is the foundation of all machine learning systems.

---

## Files in This Folder

## 📂 Files in This Folder

- [`ch01_numpy.ipynb`](./ch01_numpy.ipynb)  
  → concept-first implementation using NumPy  

- [`ch01_pytorch.ipynb`](./ch01_pytorch.ipynb)  
  → real-world implementation using PyTorch  

- [`exercises.md`](./exercises.md)  
  → experiments and exploration  

- [`solutions.md`](./solutions.md)  
  → short guidance and answers  

- `figures/`  
  → diagrams and visual explanations  

---

## How to Use This Chapter

1. Read the chapter in the book
2. Review this overview
3. Run the NumPy notebook (intuition)
4. Run the PyTorch notebook (application)
5. Solve the exercises
6. Check the solutions

---

## Key Mathematical Notation

* ℤ — integers
* ℝ — real numbers
* ℝ^d — vectors of dimension *d*

---

## Insight

> A word is not stored — it is located.

Each word is represented as a point in a high-dimensional space.
Closeness in that space corresponds to similarity in meaning.

---

## Status

Chapter 1 is under active development.
Notebooks and exercises will be expanded.
