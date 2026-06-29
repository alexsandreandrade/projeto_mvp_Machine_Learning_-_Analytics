# MVP Sprint - Machine Learning & Analytics

## 👤 Autor
Alesandre José Sá Barreto de Andrade
Matrícula: 4052025002499

## 🎯 Objetivo
Este projeto foi desenvolvido como entrega do MVP da sprint de Machine Learning & Analytics da pós-graduação em Análise de Dados e Analytics da PUC-RJ.

O objetivo é construir e avaliar modelos de Machine Learning para prever o valor total gasto em pedidos da Starbucks, utilizando informações sobre os clientes, características dos pedidos, canais de atendimento e produtos adquiridos.

A variável alvo do projeto é `total_spend`, que representa o valor total gasto em cada pedido. Como se trata de um valor numérico contínuo, o problema foi tratado como uma tarefa de regressão.

## ▶️ Como executar
Abra o arquivo `MVP_Machine_Learning_Analytics.ipynb` diretamente na raiz deste repositório.

OU

Abra o notebook no Google Colab pelo link abaixo:
[Abrir no Google Colab](https://colab.research.google.com/drive/1FjHwH0NfLmQsXKe34iA_st6Xk1sFYvRu#scrollTo=RsDEwLIGwo2C)

Execute todas as células em ordem, do início ao fim, sem necessidade de configuração adicional.

## 📊 Dataset
Base utilizada: Starbucks Customer Ordering Patterns
Fonte: [Kaggle](https://www.kaggle.com/datasets/likithagedipudi/starbucks-customer-ordering-patterns)

O dataset reúne informações como:
- pedidos realizados
- valores gastos
- canal de atendimento
- características dos clientes
- categorias de bebidas
- quantidade de itens por pedido
- número de customizações
- presença de itens de comida
- tempo de preparação e entrega
- nível de satisfação do cliente

## 🧠 Problema de Machine Learning
O problema desenvolvido neste MVP é de regressão.

O modelo tem como objetivo prever o valor total gasto em um pedido (`total_spend`) a partir das demais informações disponíveis na base de dados.

## 🔎 Etapas do projeto
O trabalho foi desenvolvido seguindo as principais etapas de um projeto de Machine Learning:
- Definição do problema
- Escolha e apresentação do dataset
- Análise exploratória dos dados
- Verificação de valores ausentes e duplicados
- Análise da variável alvo
- Tratamento de atributos
- Engenharia de atributos a partir de data e horário
- Remoção de colunas identificadoras
- Divisão entre treino e teste
- Pré-processamento com pipeline
- Construção de modelo baseline
- Treinamento de modelos candidatos
- Otimização de hiperparâmetros
- Avaliação final dos modelos
- Discussão de limitações
- Conclusão

## 🤖 Modelos avaliados
Foram avaliados os seguintes modelos:
- `DummyRegressor` utilizado como baseline
- Regressão Linear
- Random Forest
- Random Forest otimizado com `GridSearchCV`

## 📈 Principais resultados

| Modelo | MAE | RMSE | R² |
|---|---|---|---|
| Baseline | 4,4351 | 5,5680 | 0,0000 |
| Regressão Linear | 0,8300 | 0,9773 | 0,9692 |
| Random Forest | 0,8153 | 0,9577 | 0,9704 |
| Random Forest Otimizado | 0,8001 | 0,9290 | 0,9722 |

O melhor desempenho foi obtido com o Random Forest otimizado, que apresentou os menores erros de previsão e o maior valor de R² entre os modelos avaliados, superando amplamente o baseline.

## 📁 Arquivos disponíveis no repositório
- `MVP_Machine_Learning_Analytics.ipynb` — notebook Google Colab com o desenvolvimento completo do MVP
- `starbucks_customer_ordering_patterns.csv` — dataset original obtido no Kaggle

## ⚙️ Tecnologias utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
