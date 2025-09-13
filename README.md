# Task 2 – Recipe Chatbot (Local LLM Integration)

## 📌 Overview
This project sets up a local AI chatbot using **FastAPI** and **Transformers**.  
When a user enters ingredients (e.g., `Egg, Onion`), the chatbot suggests a recipe.

---

## ▶️ How to Run

### 1. Start the API server
Go into the folder and run:
    cd task2_chatbot
    python -m uvicorn app:app --reload

This will start the API on http://127.0.0.1:8000.

---

### 2. Run the chatbot client
Open a new terminal, activate the virtual environment again, then run:
    cd task2_chatbot
    python chatbot_cli.py

---

### 3. Example Run
**Input:**
    Egg, Onion

**Output:**
    🍲 Suggested Recipe:
    Egg Onion Masala: sauté onions, add spices, scramble eggs, finish with coriander.

---

## 📊 Fine-Tuning (Optional, Bonus)
1. Install extra dependency:
    pip install datasets

2. Run training script:
    python train_recipes.py

This will create a folder model_recipes/ with the fine-tuned model.

3. Restart API:
    python -m uvicorn app:app --reload

Now the chatbot will use the fine-tuned model.

---

## ✅ Deliverables
- **API** using FastAPI  
- **Chatbot client (CLI)** to interact with API  
- **Custom dataset (recipes)** provided  
- **Optional fine-tuning** with train_recipes.py
