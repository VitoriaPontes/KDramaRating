# 🎥 Predição de Avaliações de K-Dramas com Aprendizado de Máquina

Este projeto tem como objetivo prever a média de avaliações de usuários para os 100 K-Dramas mais populares do site **MyDramaList**, uma rede social voltada para fãs de mídia asiática. Com o crescente impacto global dos dramas coreanos, entender os fatores que influenciam sua recepção pode ser decisivo para orientar futuras produções.

## 📌 Objetivo

Criar modelos preditivos para estimar a nota média dos K-Dramas a partir de características como gênero, ano de lançamento, elenco principal, número de episódios, entre outros atributos descritivos e qualitativos.

## 📊 Base de Dados

- **Fonte:** [MyDramaList - Top 100 K-Dramas](https://mydramalist.com)
- **Variável alvo:** `Rating` (média das avaliações dos usuários)
- **Principais variáveis independentes:**
  - Nome da obra
  - Gêneros
  - Tags
  - Atores principais
  - Ano
  - Número de episódios
  - Duração média
  - Número de espectadores

## 🧪 Metodologia

O projeto está estruturado em quatro etapas principais:

1. **Contextualização e Análise Exploratória**  
   Introdução ao fenômeno dos K-Dramas, descrição das variáveis e estatísticas iniciais.

2. **Pré-processamento**  
   Limpeza dos dados, codificação de variáveis categóricas, análise de correlação e balanceamento do conjunto.

3. **Modelagem Estatística e de Machine Learning**  
   Foram testados vários modelos:
   - Regressão Logística
   - Árvore de Decisão
   - Random Forest
   - XGBoost
   - Rede Neural (MLP)

   Também foi aplicado ajuste de hiperparâmetros com **RandomizedSearchCV**.

4. **Avaliação de Desempenho**  
   As métricas utilizadas incluem:
   - Acurácia
   - F1-Score
   - Precisão e Revocação
   - Matriz de confusão

## 🧠 Destaque: Rede Bayesiana

Como diferencial, o projeto incluiu a construção de uma **Rede Bayesiana** para explorar a inferência probabilística entre as variáveis categóricas e a nota final. Essa abordagem permite não apenas previsão, mas interpretação causal entre os elementos da narrativa e o sucesso da obra.

## 📈 Principais Resultados

- Modelos baseados em **florestas aleatórias** e **XGBoost** apresentaram melhor desempenho.
- Atores e gêneros mostraram forte associação com a nota média.
- As tags e temas recorrentes influenciam diretamente a percepção do público.

## 🛠️ Tecnologias Utilizadas

- `Python`, `Pandas`, `Scikit-Learn`, `XGBoost`
- `pgmpy` (para Redes Bayesianas)
- `Seaborn` e `Matplotlib` (visualizações)
- `RandomizedSearchCV` (otimização)

## 👩‍💻 Autora

Projeto desenvolvido por **[Seu Nome Aqui]** como parte da disciplina de Projeto de TI.