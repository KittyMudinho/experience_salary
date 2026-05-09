# Predição de Salários: O Embate entre R² e Pearson

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
</p>

## 📌 Visão Geral
Este projeto investiga a relação entre o tempo de experiência e o salário, focando no impacto de outliers e na validação estatística através da convergência de métricas. O projeto demonstra que a limpeza de dados nem sempre visa o maior score, mas sim a maior **honestidade estatística**.

## 📊 O Fenômeno da Convergência ($R^2 = r^2$)
Durante o desenvolvimento, após remover uma **inconsistência lógica** (salário negativo) e **outliers**, o modelo atingiu a estabilidade técnica. A convergência das métricas provou que o modelo extraiu o máximo de informação possível da relação linear.

<div align="center">

| Métrica | Valor |
| :--- | :--- |
| **Correlação de Pearson ($r$)** | 0.809 |
| **R² Score (Modelo Final)** | 0.65 |
| **R² Teórico ($0.809^2$)** | ~0.65 |

</div>

> "Correlation is sometimes criticized as having no obvious interpretation for its units. This criticism is mitigated by squaring the correlation. The squared index is often called the coefficient of determination." 
> — **Rodgers, J. L., & Nicewander, W. A. (1988)**

## 🔍 Principais Insights
*   **Representatividade:** A igualdade entre o Pearson ao quadrado e o R² confirma que o *split* de treino e teste representa fielmente o dataset original.
*   **Métricas de Erro:** O MAE (Mean Absolute Error) de 4.23 reflete a dispersão real do mercado de trabalho contida nos dados.

## 🛠️ Tecnologias
* **Manipulação:** Pandas, NumPy
* **Visualização:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (LinearRegression)

---
<p align="center">
Desenvolvido por Gustavo – Computer Science Student
</p>
