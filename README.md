## MVP da Disciplina Machine Learning &amp; Analytics - PUC Rio

Aluno: Marcelo Chagas Mathias Netto

**Projeto de Classificação de Clientes em Campanhas de Marketing Bancário**

**Resumo**

Este projeto de Machine Learning tem como objetivo construir e avaliar um modelo capaz de prever se um cliente de um banco português irá subscrever um depósito a prazo. Utilizando o dataset Bank Marketing do repositório UCI, o projeto aborda um problema de classificação binária e fornece insights para otimizar futuras campanhas de marketing.

**Metodologia**

O projeto seguiu as seguintes etapas:

**Carga e Exploração de Dados**

Carregamento do dataset e análise exploratória para compreender a estrutura, distribuição das variáveis e o desbalanceamento da variável-alvo.

**Pré-processamento e Engenharia de Atributos**

Codificação de variáveis categóricas com OneHotEncoder e padronização de variáveis numéricas com StandardScaler.

Divisão do dataset em treino e teste de forma estratificada para preservar a proporção das classes.

**Modelagem e Treinamento**

Implementação e avaliação de dois modelos principais:

* Regressão Logística (baseline)

* Random Forest Classifier

**Criação de pipelines** para garantir reprodutibilidade e aplicação correta das transformações de dados.

**Otimização de Hiperparâmetros**

Utilização do GridSearchCV para ajustar os hiperparâmetros do Random Forest, visando maximizar o desempenho no conjunto de treino com validação cruzada.

**Avaliação e Análise de Resultados**

Métricas utilizadas: ROC AUC, F1-Score, Precisão e Recall, devido ao desbalanceamento do dataset.

Comparação de desempenho entre modelos padrão e otimizado.

**Principais Resultados**

O Random Forest otimizado apresentou o melhor desempenho, com ROC AUC de 0.9498, equilíbrio entre precisão e recall, e generalização adequada no conjunto de teste.

A variável duration (duração do último contato) foi um preditor muito forte, mas seu uso deve ser cauteloso em cenários de produção, pois só está disponível após a chamada.

**Conclusão**

O projeto demonstra que é possível prever com alta precisão quais clientes têm maior probabilidade de subscrever um depósito a prazo. Isso permite que instituições financeiras direcionem suas campanhas de forma mais eficiente, aumentando a taxa de conversão e reduzindo custos operacionais.
