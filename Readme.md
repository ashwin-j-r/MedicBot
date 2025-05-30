# 🩺 Medical Chatbot using LLaMA

This project aims to build a medical chatbot by fine-tuning the LLaMA 3 model on a curated dataset of medical question-answer pairs. The goal is to create a reliable, instruction-following language model that can help users with general medical queries.

---

## 📊 Dataset

The training dataset has been collected from multiple open-source sources on Kaggle. It includes medical Q&A data in both `.csv` and `.json` formats, with approximately **280,000 question-response pairs**.

Here are some of the datasets used:

- [AI Medical Chatbot (Kaggle)](https://www.kaggle.com/datasets/yousefsaeedian/ai-medical-chatbot)
- [Medical Chatbot Dataset (Kaggle)](https://www.kaggle.com/datasets/saifulislamsarfaraz/medical-chatbot-dataset)
- [Dataset for medical related chatbots (Kaggle)](https://www.kaggle.com/datasets/tusharkhete/dataset-for-medicalrelated-chatbots)
- [Medical Chatbot (Kaggle)](https://www.kaggle.com/datasets/vinayakbhat123/medical-chatbot)

> **Note:** The data needs to be **preprocessed** into the format compatible with **LLaMA 3.2 fine-tuning**, which requires each entry to follow the structure:
```json
<|begin_of_text|><|start_header_id|>user<|end_header_id|>

What is France's capital?<|eot_id|><|start_header_id|>assistant<|end_header_id|>