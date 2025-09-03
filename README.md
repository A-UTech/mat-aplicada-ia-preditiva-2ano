# AutoML

Este projeto implementa um **notebook AutoML** capaz de receber **qualquer base de dados tabular** (CSV), realizar o pré-processamento adequado e testar automaticamente diferentes algoritmos de **Machine Learning**, escolhendo o melhor modelo de acordo com as métricas de avaliação.

---

## Funcionalidades

- Leitura de qualquer dataset `.csv`, identificando automaticamente o delimitador.  
- Tratamento de **dados faltantes** (substituição por moda/mais frequente).  
- Codificação de variáveis categóricas (`LabelEncoder`).  
- Normalização de variáveis numéricas (`StandardScaler`).  
- Teste automático de **5 algoritmos de ML**:
  - Regressão Linear  
  - Decision Tree (critério = `"gini"`)  
  - Decision Tree (critério = `"entropy"`)  
  - Naive Bayes  
  - KNN  
- Seleção do **melhor modelo** com base em métricas de avaliação.  
- Visualizações gráficas:  
  - 📉 Para classificação: Matriz de Confusão + Gráfico comparando acurácias + Métricas: Precisão, Recall e F1-Score.  
  - 📈 Para regressão: Gráfico **y verdadeiro vs y predito**.  

---

## Estrutura do Projeto

```
.
├── ia-preditiva.ipynb # Notebook principal
└── README.md          # Este arquivo
```

---

### Dependências necessárias
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

---

## Exemplo de Saída

### 🔹 Classificação
- **Matriz de Confusão** (sem gridlines):  
<img src="docs/matriz_confusao_example.png" alt="" width="400"/>


- **Comparação de Modelos (Acurácia):**
<img src="docs/comparacao_modelos_example.png" alt="" width="400"/>


- **Comparação de Modelos (Métricas):**
<img src="docs/metricas_example.png" alt="" width="400"/>


---

✍️ Desenvolvido por: **[Rafael Cruz]**
