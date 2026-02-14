📌 Auto Tagging Support Tickets Using LLM

(AI/ML Engineering – Advanced Internship Task 5)

📖 Overview

This project implements an automated support ticket tagging system using Large Language Models (LLMs).

The system classifies free-text support tickets into predefined categories using:

✅ Zero-shot learning

✅ Few-shot prompting

✅ Top-3 tag prediction

✅ Performance evaluation (Precision, Recall, F1-score)

This project demonstrates modern NLP techniques using Hugging Face Transformers.

🎯 Objective

Automatically categorize customer support tickets into relevant tags without traditional supervised training.

The system compares:

Zero-shot classification

Few-shot prompting

🗂 Dataset

A synthetic support ticket dataset was created for this project.

Columns:

ticket_text → Raw customer complaint text

true_tag → Ground truth category

Categories Used:

Billing

Technical Issue

Account Access

Sales

🛠 Technologies Used

Python

Hugging Face Transformers

PyTorch

Scikit-learn

Google Colab

Pre-trained model used:

facebook/bart-large-mnli (Zero-shot classification model)

⚙️ Methodology
1️⃣ Data Loading

The dataset is loaded using pandas.

2️⃣ Zero-Shot Classification

We use a pre-trained Natural Language Inference (NLI) model to classify text into candidate labels without training.

3️⃣ Top-3 Prediction

The classifier returns probability-ranked labels.
The top 3 most probable tags are stored for each ticket.

4️⃣ Evaluation

Top-1 predictions are evaluated using:

Precision

Recall

F1-score

5️⃣ Few-Shot Prompting

We enhance performance by providing examples in the prompt before classification.

📊 Results

Successfully generated top-3 predicted tags per ticket.

Compared zero-shot vs few-shot performance.

Evaluated classification metrics using sklearn.

The model performs well for structured ticket categories with minimal configuration.
