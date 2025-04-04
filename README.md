# 🎵 Classificador de Gêneros Musicais

### ES413 - Sinais e Sistemas para Engenharia da Computação  
**Alunos:** João Marcelo de Souza Ferreira (jmsf3) e Victor Pessoa Diniz (vpd)  
**Data de Entrega:** Abril de 2025

---

## 📌 Descrição do Projeto

Este projeto tem como objetivo o desenvolvimento de um sistema de classificação automática de gêneros musicais, utilizando técnicas de processamento de sinais e aprendizado de máquina. A base de dados utilizada foi o **GTZAN**, composta por áudios de 10 gêneros diferentes.

A abordagem envolveu a extração de características relevantes dos sinais de áudio e o treinamento de modelos de machine learning capazes de identificar padrões entre os gêneros musicais. As técnicas utilizadas foram baseadas nos fundamentos da disciplina **ES413 - Sinais e Sistemas para Engenharia da Computação**, com destaque para o uso da **Transformada de Fourier** na análise espectral.

---

## ⚙️ Etapas do Projeto

1. **Pré-processamento de Áudio**  
   Segmentação dos sinais em janelas (frames) e preenchimento para uniformidade do comprimento.

2. **Extração de Características**  
   As características extraídas foram agrupadas em três domínios:
   - **Tempo**: Envelope de Amplitude, RMS, Zero-Crossing Rate
   - **Frequência**: Centroid, Bandwidth, Contrast, Flatness, Rolloff, Band Energy Ratio
   - **Tempo-Frequência**: Coeficientes Cepstrais em Frequência Mel (MFCCs)

3. **Modelos de Classificação Avaliados**
   - K-Nearest Neighbors (KNN)
   - Regressão Logística
   - Gradient Boosting
   - Random Forest
   - **Support Vector Machine (SVM)**

4. **Avaliação de Desempenho**
   Foram utilizadas métricas como **acurácia** e **matriz de confusão**. Os dois melhores modelos foram:
   - SVM: 78% de acurácia
   - Random Forest: 69% de acurácia

---

## 🧠 Tecnologias Utilizadas

- **Python**
- `librosa` — extração de características de áudio
- `numpy`, `pandas`, `scipy` — manipulação de dados e operações matemáticas
- `matplotlib`, `seaborn` — visualização de espectros e resultados
- `scikit-learn` — implementação e avaliação de modelos de machine learning

---

## 📈 Resultados Obtidos

O modelo **SVM** foi o que apresentou o melhor desempenho, com uma acurácia de 78%. Ele foi capaz de separar as classes com maior precisão devido à sua capacidade de encontrar hiperplanos ótimos em espaços de alta dimensionalidade, aproveitando a distribuição estatística (média e variância) das características.

Abaixo, uma amostra dos resultados:

| Modelo         | Acurácia |
|----------------|----------|
| SVM            | 78%      |
| Random Forest  | 69%      |

A **matriz de confusão** foi utilizada para avaliar quais gêneros foram mais confundidos entre si (ver relatório para a figura correspondente).

---

## 📚 Conclusão

O projeto demonstrou como técnicas clássicas de processamento de sinais e aprendizado de máquina podem ser eficazes na tarefa de reconhecimento de padrões musicais. O modelo de SVM obteve um bom desempenho geral, mas trabalhos futuros podem explorar arquiteturas mais complexas como redes neurais convolucionais para aprimorar os resultados.
