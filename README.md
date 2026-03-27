# DeepChem: Symbolic Machine Learning in PyTorch

This repository contains the preliminary research and prototype for a 
differentiable Symbolic Regression layer implemented in PyTorch. This project 
is being developed as part of a proposal for Google Summer of Code (GSoC) 2026 
with the DeepChem organization.

## Project Goal
The objective is to implement a robust symbolic regression capability within 
DeepChem that avoids external backends (like Julia/PySR) by leveraging 
end-to-end differentiability in PyTorch.

## Current Prototype Features
- **Differentiable Operator Selection:** Uses a soft-gating (Softmax) mechanism 
  to choose between mathematical primitives.
- **Library of Primitives:** Includes `sin`, `square`, `exp`, and `sigmoid`.
- **Optimization:** Demonstrates the ability to "recover" a target function 
  through gradient descent.

## How to Run
The core logic is contained in `DeepChem_symbolicAI_gsoc.ipynb`. You can run 
this directly in Google Colab to see the model converge on simple functions.
