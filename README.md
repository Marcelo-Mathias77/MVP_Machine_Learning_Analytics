# MVP da Disciplina Machine Learning &amp; Analytics - PUC Rio

Aluno: Marcelo Chagas Mathias Netto

**Projeto de Classificação de Clientes em Campanhas de Marketing Bancário**

**Resumo do Projeto**
Este projeto de Machine Learning tem como objetivo principal construir e avaliar um modelo preditivo capaz de determinar se um cliente de uma instituição bancária irá subscrever um depósito a prazo. Utilizando o dataset Bank Marketing do repositório UCI, o projeto aborda um problema de classificação binária, fornecendo insights valiosos para otimizar futuras campanhas de marketing.

**Metodologia**

O desenvolvimento do projeto seguiu as seguintes etapas:

1. Carga e Exploração de Dados: O dataset foi carregado, e uma análise exploratória inicial foi realizada para entender a estrutura dos dados, identificar a distribuição das variáveis e, crucialmente, reconhecer o alto desbalanceamento da variável-alvo.

2. Pré-processamento e Engenharia de Atributos: As colunas categóricas foram codificadas usando OneHotEncoder e as colunas numéricas foram padronizadas com StandardScaler. O dataset foi dividido em conjuntos de treino e teste de forma estratificada para preservar a proporção de classes.

3. Modelagem e Treinamento: Três modelos de classificação foram implementados e avaliados:

Regressão Logística (como linha de base)

Random Forest Classifier

XGBoost Classifier

4. Otimização de Hiperparâmetros: Foi utilizado o GridSearchCV para otimizar os hiperparâmetros do Random Forest e do XGBoost, buscando maximizar o desempenho dos modelos.

5. Avaliação e Análise de Resultados: O desempenho dos modelos foi avaliado usando métricas robustas para datasets desbalanceados, como ROC AUC, F1-Score, Precisão e Recall, em vez de apenas a acurácia.

**Principais Resultados e Conclusão**

A análise de desempenho revelou que o XGBoost Classifier (Otimizado) foi o modelo com a melhor performance geral. Ele obteve a maior pontuação ROC AUC de 0.81 no conjunto de teste, demonstrando uma excelente capacidade de discriminar entre clientes que subscrevem e aqueles que não.

O projeto conclui que é possível prever com alta precisão a conversão de clientes em campanhas de marketing, o que permite que as instituições financeiras direcionem seus esforços para o público com maior probabilidade de sucesso, resultando em maior eficiência e redução de custos.
