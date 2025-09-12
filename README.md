# 🕵️‍♂️ Análise de Tendência de Pessoas Desaparecidas

## 📄 Resumo do Projeto

Este projeto realiza uma análise de dados históricos sobre desaparecimentos no Brasil. Utilizando um modelo de **Regressão Linear**, o objetivo principal é identificar a tendência geral ao longo dos anos, permitindo-nos visualizar se o número de desaparecimentos está aumentando, diminuindo ou se mantendo estável.

> **Objetivo Central:** Transformar dados brutos em uma visualização clara que revele a tendência histórica de desaparecimentos.

---

## 🚀 Tecnologias e Ferramentas

| Tecnologia | Ícone | Função Principal |
| :--- | :---: | :--- |
| **Pandas** | 🐼 | Estruturação e manipulação dos dados. |
| **Scikit-learn** | 🤖 | Construção e treinamento do modelo de Machine Learning. |
| **Matplotlib** | 📊 | Criação de gráficos e visualizações para interpretar os resultados. |

---

## 🛠️ Metodologia e Funcionamento

O fluxo de trabalho foi estruturado em três etapas principais para garantir clareza e eficiência:

1.  **Carregamento e Preparação dos Dados:**
    - O arquivo `pessoas_desaparecidas.csv` é importado para um DataFrame do Pandas.
    - As colunas `Ano` e `Total` são selecionadas como variáveis de interesse para o modelo.

2.  **Criação do Modelo de Regressão:**
    - Um modelo de `Regressão Linear` do Scikit-learn é instanciado.
    - O modelo é treinado (`fit`) com os dados históricos para aprender a relação matemática entre o ano e o número total de desaparecimentos.

3.  **Visualização e Análise de Resultados:**
    - Um gráfico de dispersão (`scatter plot`) é gerado para exibir os dados reais (pontos azuis).
    - A linha de tendência (vermelha), calculada pelo modelo, é sobreposta ao gráfico. Esta linha representa a previsão do modelo e torna a tendência visualmente explícita.

> Em resumo, este projeto é um exemplo prático de como a ciência de dados nos permite extrair insights valiosos de informações do mundo real e comunicar nossas descobertas de forma eficaz.

---

## 📚 Detalhes sobre as Bibliotecas

#### 1. Pandas 🐼
O **Pandas** é a principal biblioteca para manipulação e análise de dados em Python. Ele fornece estruturas de dados flexíveis e eficientes, como o DataFrame, que são essenciais para qualquer projeto de data science.

* **Por que foi essencial?**
    * **Leitura de Dados:** Permitiu carregar o arquivo `.csv` de forma rápida e eficiente.
    * **Organização:** Estruturou os dados em um formato tabular (linhas e colunas), facilitando a seleção das variáveis `Ano` e `Total` para o treinamento do modelo.

#### 2. Scikit-learn (`sklearn`) 🤖
O **Scikit-learn** é um dos frameworks de Machine Learning mais robustos e populares. Ele oferece uma vasta gama de algoritmos prontos para tarefas de classificação, regressão, clusterização e muito mais.

* **Por que foi essencial?**
    * **Modelagem Preditiva:** Forneceu o modelo de `LinearRegression`, ideal para encontrar a relação linear entre duas variáveis (tempo e quantidade).
    * **Análise de Tendência:** O modelo treinado nos permitiu calcular a "melhor linha reta" que se ajusta aos dados, revelando a tendência de crescimento, declínio ou estabilidade ao longo do tempo.

#### 3. Matplotlib 📊
O **Matplotlib** é a biblioteca fundamental para a criação de visualizações estáticas, animadas e interativas em Python. É a ferramenta que transforma análises numéricas em insights compreensíveis.

* **Por que foi essencial?**
    * **Comunicação Visual:** Um gráfico é muito mais intuitivo que uma tabela de números. Com o Matplotlib, foi possível:
        * Plotar os **dados reais** (pontos de dispersão), mostrando a variabilidade ano a ano.
        * Desenhar a **linha de previsão** do modelo, destacando a tendência geral de forma clara e direta.
