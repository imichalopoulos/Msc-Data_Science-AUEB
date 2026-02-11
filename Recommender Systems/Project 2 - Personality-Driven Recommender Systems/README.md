# Ioannis Michalopoulos - MSc Data Science, Athens University Of Economics And Business Department of Informatics
# Recommender Systems – Assignment 2
# Personality-Driven Recommender Systems

## Overview

This project implements and evaluates neural recommender systems using a fully synthetic, personality-driven dataset in the technology products domain. The objective is to simulate realistic user–item interactions and analyze how increasing feature richness affects recommendation performance.

The project is structured into three notebooks:
1. Dataset generation
2. Simple two-tower recommender
3. Complex two-tower recommender

---

## Project Structure

├── Ioannis_Michalopoulos_RecSys_Ex2_part1_Dataset_Generation.ipynb

├── Ioannis_Michalopoulos_RecSys_Ex2_part2a_SimpleRec.ipynb

├── Ioannis_Michalopoulos_RecSys_Ex2_part2b_ComplexRec.ipynb

└── README.md



---

## Dataset Generation

The first notebook creates a synthetic dataset designed to mimic realistic recommendation scenarios.

Key elements:
- User generation with personality profiles
- Product generation with categorical, numerical, and textual attributes
- Personality-driven behavioral rules for rating and interaction simulation
- Controlled sparsity (<10% interaction density)

Outputs:
- Users dataset
- Items dataset
- User–item interactions dataset

This dataset forms the basis for training and evaluating the recommender models.

---

## Simple Recommender (Two-Tower Model)

The second notebook implements a neural two-tower architecture using a subset of user and item attributes.

Architecture:
- User tower encodes user features into embeddings
- Item tower encodes item features into embeddings
- Interaction score computed via embedding similarity

Focus:
- Basic feature engineering
- Negative sampling
- Train/holdout split
- Offline evaluation
- Personalized recommendation generation

---

## Complex Recommender (Enhanced Two-Tower Model)

The third notebook extends the simple model by incorporating all available features.

Enhancements:
- Integration of richer categorical, numerical, and textual attributes
- Higher-capacity neural architecture
- Improved modeling of personality–product alignment

Objective:
To evaluate the impact of richer feature representations on recommendation performance.

---

## Technologies

- Python
- NumPy
- Pandas
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Key Concepts

- Synthetic behavioral data simulation
- Sparse interaction matrix design
- Two-tower neural recommendation architecture
- Feature engineering
- Embedding learning
- Offline evaluation with holdout validation

---

## How to Run

1. Install dependencies:

pip install numpy pandas scikit-learn tensorflow

