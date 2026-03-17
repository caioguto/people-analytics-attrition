# People Analytics: Previsão de Attrition (Turnover) 📊

Este projeto foi desenvolvido como parte do Programa Trainee de Estatística 2025.2 na **ICMC Júnior** (USP São Carlos). O foco foi resolver um desafio real de negócios: a retenção de talentos através da identificação de padrões que levam ao desligamento voluntário de funcionários (*attrition*).

---

## 🎯 Objetivo do Projeto
Analisar os fatores que influenciam o turnover organizacional e construir um modelo preditivo capaz de identificar colaboradores em risco de saída, permitindo que o RH tome decisões estratégicas preventivas baseadas em dados.

---

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python
* **Manipulação e Análise:** Pandas e NumPy
* **Visualização:** Seaborn e Matplotlib
* **Machine Learning:** Scikit-Learn e XGBoost
* **Tratamento de Dados:** Manuseio de desbalanceamento via parâmetro `scale_pos_weight`

---

## 📈 Metodologia e Resultados
A base de dados utilizada foi o *IBM HR Analytics Employee Attrition & Performance*. O fluxo de trabalho incluiu:

1. **Análise Exploratória (EDA):** Identificação de que variáveis como idade, renda mensal e senioridade possuem forte correlação com a rotatividade.
2. **Pré-processamento:** Imputação proporcional de dados ausentes, normalização com `StandardScaler` e tratamento de variáveis categóricas para garantir a integridade estatística dos modelos.
3. **Modelagem:** Foram testados modelos de Regressão Logística, Random Forest e Gradient Boosting. O **XGBoost** foi selecionado como modelo final devido ao seu equilíbrio entre sensibilidade e precisão.

### Performance do Modelo Final (XGBoost):
* **Weighted F1-Score:** 87%
* **Recall (Classe Minoritária):** 47% (Aumento significativo na identificação de saídas reais através do ajuste de pesos das classes).
* **Drivers de Turnover:** As variáveis de maior impacto foram **Renda Mensal (Monthly Income)**, **Daily Rate** e **Idade**.

---

## 💡 Conclusões e Insights
O uso do parâmetro `scale_pos_weight` permitiu que o modelo se tornasse mais sensível à classe minoritária ("Saiu") sem comprometer a robustez geral. Os resultados mostram que políticas de retenção focadas em faixas salariais de entrada e monitoramento de colaboradores em início de carreira podem reduzir drasticamente o attrition.

---

## 📁 Estrutura do Repositório
* `data/`: Contém a base de dados utilizada no projeto.
* `notebooks/`: Contém o arquivo `.ipynb` com todo o ciclo de desenvolvimento (EDA e Modelagem).
* `reports/`: Relatório técnico detalhado do projeto.

---

## 📫 Contato
Desenvolvido por **Caio Augusto Marangoni de Mello** e Equipe.
*Estudante de Estatística e Ciência de Dados - USP São Carlos*
