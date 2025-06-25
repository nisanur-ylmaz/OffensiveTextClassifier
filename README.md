# Saldırgan Metin Sınıflandırma Sistemi

Bu proje, Türkçe metinlerde saldırgan ifadeleri tespit etmek ve bu ifadeleri **hakaret (INSULT)**, **cinsiyetçilik (SEXIST)**, **ırkçılık (RACIST)**, **küfür (PROFANITY)** gibi türlere ayırmak amacıyla geliştirilmiştir.

## 🔍 Proje Özeti

- **Model:** [BERTurk](https://huggingface.co/dbmdz/bert-base-turkish-cased)
- **Amaç:** Cümlelerin saldırgan olup olmadığını ve saldırgan ise hangi türde olduğunu belirlemek
- **Yöntem:** İki aşamalı sınıflandırma (Binary + Multi-Class)

## 🧰 Kullanılan Teknolojiler

- Python
- PyTorch
- Transformers (Hugging Face)
- scikit-learn
- Jupyter Notebook

## 📊 Başarı Sonuçları

- **Accuracy:** %91.24
- **Precision:** %90.7
- **Recall:** %89.3
- **F1-Score:** %90.0

## 🚀 Başlatma Adımları

```bash
pip install transformers datasets accelerate scikit-learn
