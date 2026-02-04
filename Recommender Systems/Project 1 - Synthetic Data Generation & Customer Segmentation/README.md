# Ioannis Michalopoulos - MSc Data Science, Athens University Of Economics And Business Department of Informatics
# Recommender Systems – Assignment 1  
# Synthetic Data Generation & Customer Segmentation # 

## Overview
This project is part of a recommender systems assignment focused on **synthetic data generation**, **user modeling**, and **customer segmentation**.  
The goal is to simulate a realistic recommendation scenario by generating entities, users with distinct personalities, user–item ratings, and then learning the underlying customer segments from observed feedback.

The implementation is provided as a Jupyter Notebook and follows the exact function specifications defined in the assignment requirements.

---

## Domain
The chosen recommendation domain is **movies**.

Each movie is represented by a rich set of attributes (e.g., genre, duration, popularity, rating, etc.), allowing for expressive user preferences and diverse recommendation behavior.

---

## Project Structure
The notebook implements **four required functions**, each corresponding to a core step in the recommendation pipeline:

### 1. `generate_entities(num_entities)`
Generates a configurable number of recommendable entities (movies).

- Each entity has **at least 10 distinct attributes**
- Attributes are designed to be meaningful for modeling user preferences
- Output is a structured dataset of entities

---

### 2. `generate_users(num_users)`
Generates a population of users belonging to **five distinct customer segments**.

- Each user is assigned to exactly one segment
- Each segment represents a unique personality type
- Personalities are defined using **combinations of at least 5 entity attributes**
- The function documentation includes a **descriptive paragraph** explaining the behavior and preferences of each segment

---

### 3. `generate_ratings(users, entities, num_ratings, noise_percentage)`
Generates **binary like/dislike ratings** for user–entity pairs.

- Ratings are primarily driven by user personality rules
- A configurable **noise parameter** introduces randomness, simulating real-world uncertainty and imperfect behavior
- Output represents implicit feedback commonly used in recommender systems

---

### 4. `learn_segments(ratings)`
Learns and identifies the underlying customer segments from the generated ratings.

- Uses observed user–item interactions only
- Attempts to recover the original user groupings
- Prints and interprets the discovered segments

---

## Methodology
The project follows a **simulation-first approach**:

1. Generate entities with structured attributes  
2. Define realistic user personas based on attribute preferences  
3. Simulate noisy user feedback  
4. Apply learning techniques to rediscover latent user segments  

This mirrors common challenges in recommender systems where true user preferences are hidden and must be inferred from interaction data.

---

## How to Run
1. Open the notebook in **Google Colab** or a local Jupyter environment
2. Run all cells sequentially
3. Adjust parameters (number of users, entities, ratings, noise) to explore different scenarios

---

## Key Assumptions & Limitations
- User preferences are rule-based and synthetic
- Ratings are binary (like/dislike), not numerical
- Segment learning is limited by the amount of noise introduced
- The focus is on **conceptual clarity**, not production-level recommendation accuracy

---

## Assignment Compliance
- All required functions are implemented  
- Function names exactly match the assignment specification  
- Domain selection is appropriate for recommendations  
- User personalities are creative and well-documented  



