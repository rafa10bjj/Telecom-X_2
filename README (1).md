# 📊 Previsão de Churn — Operadora **Telecom X**

## 📌 Descrição do Projeto
Este projeto tem como objetivo **prever o cancelamento de clientes (Churn)** em uma operadora de telecomunicações, usando dados históricos de serviços, perfil e faturamento dos clientes.  

O modelo identifica padrões que ajudam a antecipar quais clientes têm maior probabilidade de cancelar, possibilitando **ações preventivas** para reduzir a evasão.

---

## 🛠 Metodologia

1. **🔍 Análise Exploratória (EDA)**  
   - Estudo de variáveis **categóricas** e **numéricas** usando gráficos e estatísticas.  
   - Identificação de padrões, correlações e comportamentos relevantes.

2. **🧹 Tratamento dos Dados**  
   - Remoção de colunas irrelevantes (`customerID`).  
   - Padronização de categorias (ex.: unificação de “No internet service” para “No”).  
   - Tratamento de **valores ausentes** com mediana.  
   - Análise e tratamento de **outliers**.

3. **⚙ Preparação para Modelagem**  
   - Balanceamento da variável-alvo com **SMOTE**.  
   - Codificação de variáveis categóricas (**One-Hot Encoding**).  
   - Normalização com **StandardScaler** e **MinMaxScaler**.

4. **🤖 Treinamento e Avaliação de Modelos**  
   - Algoritmos testados:  
     - **KNN**  
     - **Random Forest**  
     - **Regressão Logística**  
   - Ajuste de hiperparâmetros com **GridSearchCV**.  
   - Métricas: **Acurácia**, **Matriz de Confusão**, **ROC AUC**, **Relatório de Classificação**.

============================================================
            🎯 MELHOR MODELO PARA ESTA ANÁLISE 🎯             
============================================================

📌 Modelo escolhido: RandomForestClassifier
🔹 Melhores parâmetros: {'max_depth': 10, 'max_features': 'log2', 'min_samples_leaf': 4, 'min_samples_split': 10, 'n_estimators': 200}
📊 Melhor ROC AUC: 84%

✅ Este modelo apresentou a melhor performance entre os testados e será utilizado para as próximas etapas da análise.
---

## 📈 Principais Insights
- **Contratos mensais** e **cobranças mais altas** aumentam o risco de churn.  
- Serviços adicionais como **proteção de dispositivos** e **backup online** reduzem a probabilidade de cancelamento.  
- **Qualidade do suporte técnico** é determinante para retenção.  
- Balanceamento da base melhorou o desempenho dos modelos preditivos.

---

## 💡 Recomendações
1. **📉 Reduzir Churn com Ofertas Segmentadas**  
   - Descontos para clientes com alto risco e contratos mensais.  
   - Pacotes promocionais com serviços adicionais.

2. **🛠 Melhorar Experiência do Cliente**  
   - Investir em suporte rápido e eficiente.  
   - Garantir estabilidade e qualidade do serviço.

3. **📢 Ações Preventivas**  
   - Criar sistema de monitoramento para clientes com alto risco.  
   - Contato proativo e personalizado antes do cancelamento.

---

## 🖥 Tecnologias Utilizadas
- **Python**  
- **Pandas**, **NumPy** — Manipulação e análise de dados  
- **Matplotlib**, **Seaborn** — Visualização  
- **Scikit-learn** — Pré-processamento e modelagem  
- **Imbalanced-learn (SMOTE)** — Balanceamento de dados  
- **Modelos**: KNN, Random Forest, SVM, Naive Bayes, Logistic Regression

---

## ✅ Conclusão
Este trabalho demonstra que é possível **prever churn com boa precisão** combinando EDA sólida, pré-processamento robusto (balanceamento, codificação e normalização) e modelos supervisionados.  
O **pipeline está pronto para reuso** e ajustes com novos dados, servindo como base para monitoramento contínuo e decisões orientadas por dados.

**Próximos passos recomendados:**
- Operacionalizar um **score de risco** (semanal/mensal) para toda a base de clientes.
- Integrar o score ao **CRM** para disparar ações automáticas (ofertas, upgrades, retenção).
- Monitorar **AUC, precisão e recall do positivo (churn)** em produção, com alertas de **data/model drift**.
- Rodar **A/B tests** de campanhas segmentadas para mensurar impacto em churn e LTV.
- Manter um ciclo de **melhoria contínua** com feedback do time de negócio e atualização periódica do modelo.

---

✍ **Autor:** [rafa10]  
📅 **Última atualização:** Agosto/2025  

---

## 📜 Conclusão
Este projeto demonstrou como técnicas de **ciência de dados** e **machine learning** podem ser aplicadas de forma prática para prever o churn de clientes, permitindo que empresas de telecomunicações atuem preventivamente para reter clientes e melhorar a experiência do usuário.  

A combinação de **análise exploratória**, **tratamento de dados**, **balanceamento de classes** e **modelagem preditiva** resultou em modelos robustos e insights acionáveis, que podem servir como base para estratégias de marketing, suporte e fidelização.  

O código e a metodologia apresentados podem ser facilmente adaptados para outros setores que enfrentam problemas semelhantes de evasão de clientes.

