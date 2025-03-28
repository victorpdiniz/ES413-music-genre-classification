# Reconhecedor de Gêneros Musicais

### ES413 - Sinais e Sistemas Para Engenharia da Computação  
**Alunos:** João Marcelo de Souza Ferreira e Victor Pessoa Diniz  

## Descrição do Projeto
Este projeto tem como objetivo desenvolver um classificador de gêneros musicais utilizando o dataset **GTZAN**. A classificação será baseada na extração de características espectrais do áudio por meio da **Transformada de Fourier**, seguindo princípios estudados na disciplina de Sinais e Sistemas.

## Estrutura do Projeto
O projeto é dividido nas seguintes etapas:
1. **Pré-processamento dos Dados**: Normalização dos sinais de áudio e remoção de ruídos.
2. **Extração de Características**: Utilização da Transformada de Fourier para obter espectrogramas e características como **MFCCs (Mel-Frequency Cepstral Coefficients)** e **chroma features**.
3. **Seleção de Características**: Análise das características mais relevantes para a classificação.
4. **Treinamento do Modelo**: Utilização de técnicas de Machine Learning como **SVM (Support Vector Machines), Redes Neurais** ou **Random Forest**.
5. **Avaliação e Validação**: Medidas de desempenho como **acurácia, matriz de confusão e F1-score** serão utilizadas para avaliar o modelo.

## Tecnologias Utilizadas
- **Linguagem:** Python
- **Bibliotecas:**
  - `librosa` para extração de características do áudio
  - `numpy` e `scipy` para operações matemáticas
  - `matplotlib` para visualização dos espectrogramas
  - `scikit-learn` para treinamento e avaliação dos modelos de Machine Learning

## Como Executar
1. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/reconhecedor-generos.git
   cd reconhecedor-generos
   ```
2. Instale as dependências:
   ```sh
   pip install -r requirements.txt
   ```
3. Execute o script de treinamento:
   ```sh
   python train.py
   ```
4. Para realizar previsões em novos áudios:
   ```sh
   python predict.py caminho/do/arquivo.wav
   ```

## Resultados Esperados
Ao final do projeto, esperamos obter um modelo capaz de classificar automaticamente os gêneros musicais do dataset GTZAN com alta precisão. Gráficos espectrais e tabelas de desempenho serão apresentados para justificar a escolha do modelo.

---

Este projeto foi desenvolvido como parte da disciplina **ES413 - Sinais e Sistemas Para Engenharia da Computação**.

