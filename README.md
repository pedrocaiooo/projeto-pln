# Classificação de Gêneros Musicais

Este projeto utiliza técnicas de Processamento de Linguagem Natural (PLN) para classificar letras de músicas brasileiras em cinco gêneros principais. O trabalho compara modelos tradicionais (Baseline) com o estado da arte através do **BERTimbau**.

## 🚀 Objetivo
Desenvolver um modelo capaz de identificar o gênero musical de uma música apenas com base em sua letra, lidando com desafios como a sobreposição semântica e o desbalanceamento de dados entre os gêneros.

## 📊 Modelos Comparados
O projeto avalia diferentes abordagens de representação de texto e algoritmos de classificação:

* **Vetorização:** TF-IDF e Word2Vec.
* **Classificadores:** Regressão Logística, Random Forest e Naive Bayes.
* **Deep Learning:** BERTimbau (modelo BERT pré-treinado especificamente para o português).

## 🏆 Resultados
O modelo **BERTimbau** apresentou o melhor desempenho, superando as abordagens tradicionais em quase 10 pontos percentuais no F1-Macro, devido à sua capacidade de entender o contexto semântico das letras.

| Modelo | F1-Macro | F1-Micro |
| :--- | :---: | :---: |
| **BERTimbau** | **0.78** | **0.78** |
| Regressão Logística (TF-IDF) | 0.69 | 0.73 |
| Naive Bayes | 0.58 | 0.61 |
| Random Forest | 0.45 | 0.56 |

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python
* **Principais Bibliotecas:** Scikit-learn, Pandas, NLTK, PyTorch e Hugging Face Transformers.
* **Ambiente:** Google Colab (GPU T4).

---
**Autores:** Adriano Dias, Davi Barros, Pedro Caio e Rhonnye Wendell.
