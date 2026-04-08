# 🧬 Investigating Cultural Bias in Large Language Models  
**A Pakistani Cultural Context**
<!-- Replace the link above with your actual banner image once uploaded -->

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![PDF Paper](https://img.shields.io/badge/Paper-PDF-red)](ProjectReport.pdf)
[![Presentation](https://img.shields.io/badge/Presentation-HTML-orange)](presentation.html)
[![Made in Pakistan](https://img.shields.io/badge/Made%20with%20❤️%20in-Pakistan-green)](https://github.com)

**Authors:** Asad Muhammad Naeem, Fatima Attique, Habiba Kamran, Muhammad Umair Habib  
**Date:** April 8, 2026

---

## 📌 Abstract

This research investigates the presence of **Western cultural bias** in seven open-source Large Language Models through a targeted evaluation across Pakistan’s four major cultures — **Punjabi, Sindhi, Balochi, and Pashtun**. Using a novel masked cloze-test methodology with culturally-specific prompts and four rigorous metrics (Bias Ratio, Western Preference Frequency, NER Recognition Rate, and Sentiment Difference), we uncover systematic preferences for Western entities, especially in identity-related domains.

**Core Takeaway:**  
> *Recognizing a cultural entity does **not** guarantee fair treatment of that entity.*

---

## ✨ Key Findings

- **Strongest bias** in socially sensitive categories:  
  - **Male Names**: 55.51% Western preference, Bias Ratio = **4.12**
  - **Literature**: Bias Ratio = **2.58**

- **Lowest bias** in everyday/domestic domains:  
  - **Food** & **Female Dress** show strong local preference

- **Model Performance:**
  | Model                  | Western Preference (F<sub>w</sub>) | Bias Ratio | Cultural Literacy (NER) | Verdict          |
  |------------------------|------------------------------------|------------|--------------------------|------------------|
  | **Mistral-7B**         | **7.6%**                           | **1.00**   | 38–45%                   | **Best Performer** |
  | Qwen-2.5-7B            | 53%                                | **2.8**    | 19%                      | **Worst Performer** |
  | Qalb-1.0-8B / Lughaat  | ~48%                               | 1.2–1.3    | **42%**                  | Highest Literacy |

- Cultural context reduces bias in 8/10 categories but **never eliminates** it.
- Even Urdu-specialized models inherit strong Western priors.

---

---

## 🎥 Interactive Presentation

**[👉 Open Live Presentation](presentation.html)**  
*(Open the HTML file directly in any modern browser — fully responsive, MathJax rendered, keyboard navigation enabled)*

---

## 📖 Full Research Paper

**[Download Complete Paper (PDF)](ProjectReport.pdf)**  
37 pages • 4 metrics • 7 LLMs • 10 cultural categories • Statistical analysis

---

## 🧪 Methodology at a Glance

- **10 Cultural Categories**: Male/Female Names, Food, Drinks, Male/Female Dress, Sports, Events, Arts, Literature  
- **5 Languages**: Punjabi, Sindhi, Balochi, Pashto, Urdu  
- **Prompt Technique**: Masked Cloze Test (`[MASK]`) with **Contextual** vs **Non-Contextual** conditions  
- **Models Evaluated**: Qwen2.5-7B, Gemma-2-2B, Aya-Expanse-8B, Qalb-1.0-8B, Llama-3.2-3B, Mistral-7B, Lughaat-1.0-8B  
- **Metrics**:
  - Bias Ratio \( R = \frac{P(\text{Western})}{P(\text{Local})} \)
  - Western Preference Frequency \( F_w \)
  - NER Recognition Rate (Cultural Literacy)
  - Sentiment Difference \( \Delta S \)

---

## 📊 Results Snapshot (Aggregated)

**Highest Bias Categories** (Averaged across all models)

| Category         | Avg F<sub>w</sub> | Avg Bias Ratio | Avg NER   |
|------------------|-------------------|----------------|-----------|
| Male Names       | **55.51%**        | **4.12**       | 52.78%    |
| Literature       | 49.54%            | 2.58           | 36.32%    |
| Drinks           | 47.55%            | 1.31           | 12.66%    |
| **Food**         | **32.04%**        | **0.64**       | 12.01%    |

*(Full tables available in the paper and presentation)*

---

## 🔮 Future Work & Recommendations

- Evaluation on frontier models (GPT-4o, Claude 3.5, Grok-2)
- Dialectal and intersectional bias analysis
- Long-form generation bias study
- Development of **Cultural RLHF** and culturally-augmented fine-tuning datasets
- Open-sourcing a Pakistani cultural benchmark for LLMs

---

## 📬 How to Cite

```bibtex
@misc{naeem2026culturalbias,
  title        = {Investigating Cultural Bias in Large Language Models: A Pakistani Cultural Context},
  author       = {Asad Muhammad Naeem and Fatima Attique and Habiba Kamran and Muhammad Umair Habib},
  year         = {2026},
  month        = {April},
  howpublished = {\url{https://github.com/muhammad-asad-014/Investigating-Cultural-Bias-in-Large-Language-Models.git}}
}
