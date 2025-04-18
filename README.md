# 🧠 Customer Segmentation com RFM e K-Means  
*Identificando perfis de clientes com Machine Learning para estratégias de marketing mais eficientes*

---

## 📑 Visão Geral

Este projeto tem como objetivo realizar a **segmentação de clientes** utilizando a metodologia **RFM (Recência, Frequência, Valor Monetário)** combinada com o algoritmo de **clusterização K-Means**, a fim de identificar perfis distintos de consumidores e apoiar decisões de negócio baseadas em dados.

---

## ⚙️ Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 🔍 Etapas do Projeto

1. **Carregamento e Limpeza dos Dados**
   - Leitura dos dados de vendas.
   - Remoção de valores nulos e transações canceladas.
   - Cálculo do valor total de cada compra (`TotalPrice`).

2. **Engenharia de Atributos**
   - Conversão de datas.
   - Cálculo das métricas RFM:
     - **Recency**: Dias desde a última compra.
     - **Frequency**: Número de compras únicas.
     - **Monetary**: Valor total gasto.

3. **Análise Exploratória**
   - Estatísticas descritivas.
   - Verificação de outliers com boxplots.

4. **Modelagem**
   - Normalização dos dados com `StandardScaler`.
   - Definição do número ideal de clusters com o **método do cotovelo**.
   - Treinamento do modelo K-Means e avaliação com o **Silhouette Score**.

5. **Visualização dos Resultados**
   - Gráficos de dispersão dos clusters.
   - Análise de pares (pairplot).

6. **Insights e Recomendações de Negócio**
   - Segmentação dos clientes em 4 clusters:
     - 🟢 **Cluster 0**: Clientes VIP – Alta frequência e alto valor.
     - 🟡 **Cluster 1**: Novos Clientes – Recentes, porém com baixo engajamento.
     - 🔴 **Cluster 2**: Clientes Inativos – Não compram há muito tempo.
     - 🔵 **Cluster 3**: Regulares de Baixo Valor – Compram com frequência, mas gastam pouco.

---

## 💡 Recomendações Estratégicas

| Cluster | Estratégia |
|--------|------------|
| **VIPs** | Fidelização e exclusividade |
| **Novos** | Ofertas de boas-vindas |
| **Inativos** | Campanhas de reativação |
| **Regulares** | Promoções para aumento do ticket médio |
