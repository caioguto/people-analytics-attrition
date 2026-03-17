# People Analytics: Previsão de Attrition (Turnover) 📊

Este projeto foi desenvolvido como parte do processo de formação na **ICMC Júnior**, focado em resolver um problema real de negócios: a retenção de talentos. O objetivo é identificar padrões que levam ao desligamento de funcionários e prever futuras saídas utilizando Machine Learning.

---

## 🎯 Objetivo do Projeto
Analisar os fatores que influenciam o turnover organizacional e construir um modelo capaz de prever a rotatividade de funcionários com alta precisão, permitindo que o RH tome decisões estratégicas preventivas.

---

## 🛠️ Tecnologias e Ferramentas
**Linguagem:** Python
**Manipulação e Análise:** Pandas e NumPy
**Visualização:** Seaborn e Matplotlib
**Machine Learning:** Scikit-Learn e XGBoost
**Tratamento de Dados:** SMOTE (Synthetic Minority Over-sampling Technique) para balanceamento de classes

---

## 📈 Metodologia e Resultados
A base de dados utilizada foi o *IBM HR Analytics Employee Attrition & Performance*. O fluxo de trabalho incluiu:

1. **Análise Exploratória (EDA):** Identificação de que funcionários mais jovens e com menor renda possuem maior tendência ao attrition.
2. **Pré-processamento:** Tratamento de variáveis categóricas via Label Encoding e aplicação de SMOTE para lidar com o desbalanceamento da base.
3. **Modelagem:** Foram testados modelos de Regressão Logística e Random Forest, mas o **XGBoost** apresentou o melhor desempenho após o ajuste de hiperparâmetros via Grid Search.

### Performance do Modelo Final (XGBoost):
**F1-Score:** 87%
**Recall:** 94% (foco em identificar o máximo de funcionários em risco) 
**Drivers de Turnover:** As variáveis mais importantes foram **Hora Extra (Overtime)**, **Renda Mensal** e **Idade**.

---

## 💡 Conclusões e Insights
O modelo demonstrou que intervenções focadas em planos de carreira para colaboradores em início de trajetória e monitoramento de cargas horárias excessivas podem reduzir significativamente os custos de contratação e treinamento da empresa.

---

## 📁 Estrutura do Repositório
`notebooks/`: Contém o arquivo `.ipynb` com todo o ciclo de desenvolvimento do modelo.
* `data/`: (Opcional) Armazenamento da base de dados utilizada.
`reports/`: Relatório técnico detalhado do projeto.

---

## 📫 Contato
Desenvolvido por **Caio Augusto Marangoni de Mello** *Estudante de Estatística e Ciência de Dados - USP São Carlos*
