# 🏦 Previsão de Aprovação de Empréstimos com Redes Neurais (MLP)

Projeto de aprendizado de máquina focado na classificação e análise de risco de crédito para concessão de empréstimos, utilizando Redes Neurais Artificiais (Multilayer Perceptron - MLP).

---

## 🎯 Objetivo
Construir um pipeline completo de Machine Learning para prever a aprovação ou rejeição de crédito com base no perfil socioeconômico e histórico financeiro do solicitante, avaliando diferentes arquiteturas de redes neurais.

---

## 📊 Dataset
O conjunto de dados contém registros de solicitações de empréstimo com 14 variáveis, cobrindo:
- **Perfil do Solicitante:** Idade, gênero, escolaridade, renda anual, tempo de experiência profissional e tipo de moradia.
- **Dados do Empréstimo:** Valor solicitado, finalidade, taxa de juros e percentual da renda comprometido.
- **Histórico Financeiro:** Tempo de histórico de crédito, pontuação de crédito (score), registros de inadimplência prévia e status de aprovação (`loan_status` - variável alvo).

---

## ⚙️ Pipeline do Projeto
1. **Data Profiling & EDA:** Análise descritiva, detecção de outliers e distribuições das variáveis contínuas e categóricas.
2. **Data Cleaning:** Tratamento de inconsistências lógicas de idade/experiência e remoção de outliers de renda extrema.
3. **Pré-processamento:** Divisão treino/teste (70/30), mapeamento binário, *One-Hot Encoding* para atributos nominais e normalização de variáveis contínuas com `StandardScaler` (sem data leakage).
4. **Modelagem:** Implementação e ajuste de hiperparâmetros com `MLPClassifier` (Scikit-Learn), explorando variações de topologia de neurônios, taxa de aprendizado e convergência.

---

## 🛠️ Tecnologias Utilizadas
- **Python**
- **Manipulação & Análise:** `pandas`, `numpy`
- **Machine Learning:** `scikit-learn`
- **Visualização:** `matplotlib`, `seaborn`
- **Ambiente:** Jupyter Notebook / Google Colab
