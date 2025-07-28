#  Problem Statement
In any organization that handles customer service, support tickets can pile up quickly. These tickets come in as free-form text, and it's up to the support team to figure out what each one is about—whether it's a billing issue, a technical problem, an account access request, or something else. Manually reading and tagging each ticket takes time and can lead to mistakes, especially when the volume is high.

The goal of this project is to automate that tagging process using large language models (LLMs). Instead of relying on rule-based systems or manual effort, we’ll use models that can understand the content of each support ticket and assign relevant tags to it.

We'll experiment with a few different methods:

1. Zero-shot learning, where the model guesses the category without seeing any training examples.

2. Few-shot learning, where we give the model a few examples to learn from in the prompt.

3. Fine-tuned models, where we train the model on a labeled dataset to make it more accurate.

In the end, the system should be able to return the top 3 most likely categories for any incoming ticket. This would make it easier for support teams to prioritize and handle issues more efficiently.

---

This project automates the classification (tagging) of customer support tickets into predefined categories using modern NLP techniques:

- ✅ Zero-shot classification (`facebook/bart-large-mnli`)
- ✅ Fine-tuned BERT-based classifier (`distilbert-base-uncased`)
- ✅ Simulated few-shot classification using prompt augmentation

---

## 🚀 Features

- Automatically tag support tickets with the top relevant category.
- Compare three classification techniques:
  - **Zero-shot** with large language models (LLMs)
  - **Fine-tuned** transformer-based classifier
  - **Simulated Few-shot** classification without using text generation
- Generate confidence scores and visualizations
- Easily extendable to other datasets or domains

---

## 📁 Dataset

This notebook uses a **sample dataset of support tickets**, each labeled into one of the following categories:

- `account_access`
- `refund`
- `technical_issue`
- `integration`
- `billing`

Each ticket is a sentence representing a customer support issue or request.

---

## 🛠️ Installation

Clone this repository or open the notebook in Colab or Jupyter Notebook.

```bash
pip install -r requirements.txt
```

---

## 📓 How to Use

1. Run all cells in `Auto_Tagging_Support_Tickets.ipynb`
2. Inside the notebook:
   - Generate synthetic data
   - Initialize `SupportTicketTagger`
   - Use methods like:
     - `zero_shot_tagging(tickets)`
     - `fine_tune_model()`
     - `simulate_few_shot_with_classifier(tickets)`
     - `evaluate_model(predictions)`
3. View results and metrics like:
   - Accuracy
   - Confusion matrix
   - Prediction confidence

---

## 💡 Notes

- You can replace the `sample_dataset` with your own support tickets CSV or JSON.
- The GPT-2 based few-shot generation method is optional and not required for classification logic.
- The code is modular and designed for clarity and educational purposes.

---

## 📬 Author

Nouman Bashir  
📧 Email: noumanbashir923@gmail.com  
🔗 GitHub: https://github.com/bnouman

---
