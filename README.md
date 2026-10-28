# 🫀 Análise Exploratória e Preditiva de Fatores de Risco Cardiovascular

Uma análise exploratória e estatística aprofundada sobre biomarcadores metabólicos, hábitos comportamentais e indicadores demográficos, com o objetivo de mapear padrões críticos associados ao risco de eventos cardiovasculares.

---

## 📌 Contexto & Objetivos

Doenças cardiovasculares continuam entre as principais causas de mortalidade global. Este estudo investiga a interdependência entre **fatores biométricos** (IMC, idade, frequência cardíaca), **biomarcadores laboratoriais** (colesterol, triglicerídeos) e **estilo de vida** (horas sedentárias, nível de atividade física) para:

* Compreender o peso relativo de cada indicador no desenvolvimento de condições de risco.
* Tratar inconsistências e mapear anomalias/outliers clínicos relevantes.
* Estabelecer uma linha de base analítica para modelagem preditiva e suporte a decisões de triagem em saúde.

---

## 🛠️ Tecnologias & Bibliotecas

* **Linguagem & Manipulação:** Python (Pandas, NumPy)
* **Visualização de Dados:** Matplotlib, Seaborn
* **Análise Estatística & Machine Learning:** SciPy, Scikit-Learn *(modelagem linear baseline)*
* **Ambiente de Desenvolvimento:** Jupyter Notebook / Google Colab

---

## 🔬 Pipeline do Estudo

1. **Tratamento & Limpeza de Dados:**
   * Tratamento de valores ausentes (*imputation* estratégica) e remoção de redundâncias.
   * Padronização de tipos de dados e detecção de assimetrias.
2. **Estatística Descritiva & Diagnóstico:**
   * Cálculo de medidas de tendência central (médias, medianas) e dispersão (IQR, desvio padrão).
   * Mapeamento de separatrizes e percentis críticos.
3. **Distribuições & Detecção de Outliers:**
   * Análise de skewness/kurtosis via histogramas e densidade (KDE).
   * Identificação de outliers em perfis metabólicos por meio de Boxplots e Z-Score.
4. **Análise de Correlação & Relação Clínica:**
   * Matrizes de correlação (Pearson/Spearman) cruzando biomarcadores e variáveis de estilo de vida com o desfecho clínico.
5. **Modelagem Baseline:**
   * Ajuste de modelos lineares preliminares para mensurar o poder preditivo e a significância dos coeficientes.

---

## 📊 Principais Descobertas (Key Findings)

* **Prevalência Crítica:** **36%** da coorte analisada apresenta risco cardiovascular moderado a elevado.
* **Biomarcadores Determinantes:** Níveis de **colesterol**, **triglicerídeos** e **IMC** apresentaram o maior impacto relativo na classificação de risco.
* **O Paradoxo do Estilo de Vida:** Variáveis de hábitos diários (como horas sedentárias) demonstraram correlação direta fraca isoladamente, indicando que seu efeito é mediado principalmente pelas alterações metabólicas cumulativas (idade, peso e predisposição).
* **Anomalias Clínicas:** A presença de outliers acentuados em triglicerídeos e colesterol reflete subgrupos de vulnerabilidade metabólica aguda que exigem atenção clínica diferenciada.

---

## 📁 Estrutura do Repositório

```text
├── data/
│   ├── raw/             # Dados brutos originais
│   └── processed/       # Dados tratados e limpos
├── notebooks/           # Notebooks de EDA e modelagem passo a passo
├── reports/             # Figuras salvas e relatórios técnicos gerados
├── requirements.txt     # Dependências do projeto
└── README.md
