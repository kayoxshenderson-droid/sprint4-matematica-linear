# Challenge Sprint 4 — Classificação de Produção de Energia Renovável

Projeto desenvolvido para o **Challenge Sprint 4 da FIAP**, utilizando Python e técnicas de Machine Learning para realizar a classificação de dados relacionados à produção de energia renovável.

## 📌 Sobre o projeto

Neste projeto foi utilizado o dataset **Renewable Energy Production Dataset (2010–2020)**, disponibilizado no Kaggle.

O objetivo foi preparar os dados, analisar a correlação entre as variáveis e desenvolver um modelo de classificação capaz de identificar diferentes categorias de produção de energia:

* **Low**
* **Medium**
* **High**

Para a classificação, foi utilizada a **Regressão Logística Multinomial**, modelo de classificação linear disponível na biblioteca Scikit-learn.

---

## 🎯 Objetivos

O projeto foi dividido em três etapas principais:

### 1. Análise do dataset

* Carregamento do dataset utilizando Pandas;
* Encoding da variável `Energy_Class`;
* Construção da matriz de correlação;
* Análise das correlações entre as variáveis;
* Definição das features utilizadas no modelo.

### 2. Aplicação do modelo

Foi utilizada a **Regressão Logística Multinomial** para realizar a classificação.

Foram analisados dois cenários:

| Cenário   | Treinamento | Teste |
| --------- | ----------: | ----: |
| Cenário 1 |         60% |   40% |
| Cenário 2 |         85% |   15% |

Nos dois cenários foram mantidas condições semelhantes, incluindo `random_state=42`, permitindo uma comparação mais adequada.

### 3. Avaliação do modelo

O desempenho foi analisado utilizando:

* Matriz de confusão;
* Acurácia;
* Precisão;
* Recall;
* F1-Score;
* Comparação entre os dois cenários.

---

## 🧠 Modelo utilizado

### Regressão Logística Multinomial

A Regressão Logística foi escolhida por ser um modelo de classificação linear.

O modelo estabelece suas fronteiras de decisão a partir de combinações lineares das features, permitindo classificar as observações entre as categorias `Low`, `Medium` e `High`.

Antes do treinamento, as features numéricas foram padronizadas utilizando `StandardScaler`.

---

## 📊 Resultados

Os dois cenários apresentaram resultados próximos, permitindo comparar o efeito de diferentes proporções entre dados de treinamento e teste.

### Cenário 1 — 60% treino / 40% teste

* **Acurácia:** aproximadamente 79%
* **Recall — Low:** 52,11%
* **Precisão — Low:** 92,50%

### Cenário 2 — 85% treino / 15% teste

* **Acurácia:** aproximadamente 78%
* **Recall — Low:** 62,96%
* **Precisão — Low:** 80,95%

Os resultados mostram que os dois cenários apresentaram desempenho semelhante, embora algumas métricas tenham variado entre as divisões dos dados.

---

## 🛠️ Tecnologias utilizadas

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 📊 Matplotlib
* 🎨 Seaborn
* 🤖 Scikit-learn
* 📓 Jupyter Notebook / Google Colab

---

## 📂 Estrutura do projeto

```text
Challenge-Sprint-4/
│
├── analise.ipynb
├── Renewable_Energy_Data.csv
└── README.md
```

---

## ▶️ Como executar

1. Clone ou baixe este repositório.
2. Abra o arquivo `analise.ipynb` no Jupyter Notebook ou Google Colab.
3. Certifique-se de que o arquivo `Renewable_Energy_Data.csv` esteja disponível no ambiente.
4. Execute as células do notebook em ordem.

---

## 🎥 Vídeo do projeto

No vídeo são apresentados o desenvolvimento do projeto, a análise dos dados, o modelo utilizado e os resultados obtidos.

🔗 **[Assistir ao vídeo no YouTube]([COLE_AQUI_O_LINK_DO_YOUTUBE](https://youtu.be/HjEJut5B504
))**

---

## 👨‍💻 Integrantes

| Integrante                   |     RM |
| ---------------------------- | -----: |
| **Gustavo Zagato Bottechia** | 569420 |
| **Davi Q. Zuolo**            | 571669 |
| **Daniel Vilela Mana**       | 571632 |
| **Kayo Henderson**           | 570706 |

---

## 📚 Dataset

**Renewable Energy Production Dataset (2010–2020)**
Dataset disponibilizado no Kaggle e utilizado como base para a análise e classificação de produção de energia renovável.

---

## 📌 Conclusão

O projeto permitiu aplicar conceitos de preparação de dados, análise de correlação, classificação supervisionada e avaliação de modelos de Machine Learning.

A comparação entre os cenários de 60/40 e 85/15 possibilitou observar como diferentes proporções entre treinamento e teste podem influenciar as métricas de avaliação do modelo.
