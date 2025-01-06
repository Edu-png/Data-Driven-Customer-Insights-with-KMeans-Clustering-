# 💸 Data-Driven Customer Insights with KMeans Clustering

<p align="center">
  <a href="https://github.com/Edu-png">
    <img src="https://img.shields.io/badge/Autor-Eduardo%20Coqueiro-purple?style=flat&logo=github" alt="Autor">
  </a>
  <a href="mailto:eduardocoqueiro@gmail.com">
    <img src="https://img.shields.io/badge/Email-eduardocoqueiro%40gmail.com-purple?style=flat&logo=gmail" alt="Email">
  </a>
  <a href="https://linkedin.com/in/eduardocoqueiro/">
    <img src="https://img.shields.io/badge/LinkedIn-Eduardo%20Coqueiro-purple?style=flat&logo=linkedin" alt="LinkedIn">
  </a>
  <a href="https://kaggle.com/EduardoCoqueiro">
    <img src="https://img.shields.io/badge/Kaggle-Eduardo%20Coqueiro-blue?style=flat&logo=kaggle" alt="Kaggle">
  </a>
</p>

![CAPAS - PROJETOS (1)](https://github.com/user-attachments/assets/2ee27201-5e06-40c2-815c-53a15b0cd135)

## Sumário 🎯

## 📚 Introdução

O projeto **"Data-Driven Customer Insights with KMeans Clustering"** foi desenvolvido com o objetivo de aplicar técnicas de agrupamento (clustering) para extrair insights significativos sobre o comportamento de clientes. Utilizando o algoritmo **K-Means Clustering**, foi possível segmentar clientes com base em seus padrões de consumo, permitindo uma análise mais profunda sobre suas necessidades e preferências.

A análise visa identificar diferentes perfis de clientes, ajudando empresas a direcionarem suas estratégias de negócio com mais eficácia, oferecendo produtos e serviços personalizados para cada grupo identificado. Dessa forma, o projeto contribui para a melhoria da experiência do cliente e para o aumento da eficiência em campanhas de marketing.

---

## 🔧 Pipeline do Projeto

A pipeline do projeto **"Data-Driven Customer Insights with KMeans Clustering"** foi estruturada para garantir a execução das etapas de análise e agrupamento de clientes de forma sistemática e organizada. A seguir estão as etapas detalhadas que compõem o fluxo de trabalho:

---

### 📥 **1. Importação dos Dados**
- Carregamento da base de dados utilizando bibliotecas do Python, como `pandas`.
- Verificação inicial da estrutura dos dados com funções como `.head()`, `.info()`, e `.describe()`.
- Análise de variáveis disponíveis no dataset para garantir consistência.

---

### 🧹 **2. Limpeza e Pré-processamento dos Dados**
- Tratamento de valores nulos e dados inconsistentes.
- Normalização das variáveis para garantir que todas estejam na mesma escala, utilizando técnicas como **Min-Max Scaling**.
- Conversão de dados categóricos, quando necessário, para valores numéricos através de **One-Hot Encoding**.

---

### 📊 **3. Análise Exploratória de Dados (EDA)**
- Criação de gráficos e visualizações para identificar padrões nos dados.
- Análise de dispersão e correlação entre variáveis.
- Identificação de variáveis relevantes para o modelo de clustering.

---

### 🤖 **4. Aplicação do Algoritmo K-Means Clustering**
- Definição do número ideal de clusters utilizando o **método do cotovelo (Elbow Method)**.
- Treinamento do modelo utilizando o algoritmo **K-Means**.
- Atribuição de cada cliente ao cluster correspondente.

---

### 📋 **5. Análise dos Clusters**
- Interpretação dos clusters formados, identificando características específicas de cada grupo.
- Nomeação de cada cluster com base em seus padrões de consumo (ex.: "Clientes de Alto Valor", "Clientes Sensíveis a Preço", etc.).
- Avaliação da homogeneidade dentro dos clusters e heterogeneidade entre eles.

---

### 📈 **6. Visualização dos Resultados**
- Criação de gráficos para visualizar a distribuição dos clusters.
- Utilização de gráficos como **scatter plots** e **heatmaps** para destacar as diferenças entre os grupos.

---

### 💾 **7. Exportação dos Resultados**
- Salvamento dos clusters formados em um arquivo CSV para uso em análises futuras.
- Geração de relatórios com insights para auxiliar na tomada de decisão.

---

### 🔄 **8. Melhorias Futuras**
- Automatização do pipeline de clustering.
- Aplicação de outros algoritmos de clustering (como DBSCAN ou Hierarchical Clustering) para comparação de desempenho.
- Implementação de dashboards interativos para visualização dos resultados em tempo real.

---

## 🧪 Metodologia do Projeto

A metodologia utilizada no projeto **"Data-Driven Customer Insights with KMeans Clustering"** foi cuidadosamente planejada para garantir que cada etapa do processo de análise e agrupamento de dados fosse realizada de forma eficiente e estruturada. Abaixo, apresento um detalhamento de cada etapa do fluxo de trabalho, desde a importação dos dados até a exportação dos resultados e sugestões para melhorias futuras.

---

### 📥 **1. Importação e Compreensão Inicial dos Dados**

A primeira etapa do projeto envolve a importação da base de dados e a verificação inicial das informações presentes. Isso inclui:
- **Carregamento da base de dados** utilizando bibliotecas como `pandas`.
- **Inspeção inicial** da estrutura dos dados com funções como:
  - `.head()` - Visualização das primeiras linhas do dataset.
  - `.info()` - Verificação das colunas, tipos de dados e valores nulos.
  - `.describe()` - Cálculo de estatísticas descritivas, como média, desvio padrão e percentis.

Objetivo:
- Garantir que o dataset está completo e consistente antes de iniciar a análise.

---

### 🧹 **2. Limpeza e Pré-processamento dos Dados**

Antes de aplicar o algoritmo de clustering, é necessário garantir que os dados estão limpos e preparados. As seguintes ações foram realizadas nesta etapa:

#### 🔧 **Tratamento de Valores Nulos**
- Identificação de colunas com valores ausentes utilizando `.isnull().sum()`.
- Substituição de valores nulos por valores adequados ou remoção de registros dependendo da análise.

#### 📏 **Normalização dos Dados**
- Aplicação de **Min-Max Scaling** para garantir que todas as variáveis estejam na mesma escala, evitando que uma variável com valores altos influencie mais o modelo do que outras variáveis.
  - Utilização da biblioteca `sklearn.preprocessing` para realizar a normalização.

#### 🔄 **Conversão de Dados Categóricos**
- Transformação de variáveis categóricas em variáveis numéricas utilizando **One-Hot Encoding**, quando necessário.

Objetivo:
- Garantir que os dados estão prontos para serem utilizados pelo algoritmo K-Means.

---

### 📊 **3. Análise Exploratória de Dados (EDA)**

Nesta etapa, o foco é entender melhor o comportamento dos dados através de visualizações e análises estatísticas. Algumas ações realizadas incluem:

#### 📈 **Visualizações Gráficas**
- Criação de gráficos utilizando bibliotecas como `matplotlib` e `seaborn` para identificar padrões nos dados.
  - **Histogramas** para visualizar a distribuição das variáveis.
  - **Boxplots** para identificar outliers.
  - **Scatter plots** para verificar a dispersão dos dados e relações entre variáveis.

#### 📉 **Identificação de Correlações**
- Utilização de **heatmaps** para identificar correlações entre variáveis, garantindo que não haja redundância nos dados.

Objetivo:
- Identificar padrões e possíveis agrupamentos naturais antes da aplicação do algoritmo de clustering.

---

### 🤖 **4. Aplicação do Algoritmo K-Means Clustering**

Nesta etapa, o foco é aplicar o algoritmo **K-Means** para segmentar os clientes em grupos distintos com base em seus comportamentos.

#### 📐 **Determinação do Número de Clusters**
- Utilização do **Método do Cotovelo (Elbow Method)** para definir o número ideal de clusters.
  - Criação de um gráfico que mostra a **inércia (distância interna dos clusters)** em função do número de clusters.
  - Escolha do ponto em que há uma queda acentuada na inércia, indicando o número ideal de clusters.

#### 🧮 **Treinamento do Modelo**
- Treinamento do modelo K-Means utilizando a biblioteca `sklearn.cluster`.
  - Definição do número de clusters (k) baseado no Elbow Method.
  - Ajuste dos dados ao modelo utilizando o método `.fit()`.

#### 📋 **Atribuição de Clusters**
- Após o treinamento, cada cliente foi atribuído ao cluster correspondente.
  - Atribuição realizada utilizando o método `.predict()`.

Objetivo:
- Formar grupos de clientes com características semelhantes, permitindo uma análise mais direcionada.

---

### 📋 **5. Análise dos Clusters Formados**

Após a criação dos clusters, é importante interpretar os resultados e entender as características específicas de cada grupo.

#### 🔍 **Características dos Clusters**
- Análise das médias e desvios padrão das variáveis dentro de cada cluster.
- Identificação de características únicas de cada grupo, como:
  - Clientes de alto valor.
  - Clientes sensíveis a preço.
  - Clientes recorrentes, etc.

#### 📌 **Nomeação dos Clusters**
- Com base nas análises, os clusters foram nomeados de acordo com suas características predominantes.

Objetivo:
- Garantir que os clusters formados tenham significado prático e possam ser utilizados em estratégias de negócio.

---

### 📈 **6. Visualização dos Resultados**

Visualizar os resultados é fundamental para garantir uma interpretação clara e acessível das informações. Algumas das visualizações geradas incluem:

#### 🖼 **Gráficos de Dispersão (Scatter Plots)**
- Visualização dos clusters em gráficos de dispersão para entender como os grupos estão separados.

#### 🌡 **Heatmaps**
- Utilização de **heatmaps** para destacar as diferenças entre os clusters.

#### 📊 **Gráficos de Barras**
- Criação de gráficos de barras que destacam as médias das variáveis principais dentro de cada cluster.

Objetivo:
- Facilitar a comunicação dos resultados e insights obtidos com o modelo.

---

### 💾 **7. Exportação dos Resultados**

Para garantir que os insights possam ser utilizados futuramente, os dados tratados e os clusters formados foram exportados em formato CSV.

#### 📤 **Exportação dos Dados**
- Utilização do método `.to_csv()` para salvar os resultados em um arquivo CSV.
- Configuração de separadores personalizados para garantir compatibilidade com outras ferramentas.

---

### 🔄 **8. Melhorias Futuras**

Algumas sugestões para melhorias futuras incluem:

- **Automatização do Pipeline**: Criar um script automatizado que execute todas as etapas de forma contínua.
- **Aplicação de Outros Algoritmos de Clustering**: Experimentar com algoritmos como **DBSCAN** ou **Hierarchical Clustering** para comparar os resultados.
- **Implementação de Dashboards Interativos**: Utilizar ferramentas como **Plotly** ou **Power BI** para criar dashboards que permitam a visualização dos clusters de forma dinâmica.

---
## 📊 Visualizações e Interpretações dos Gráficos

---

### 📍 **Gráfico 1: Distribuição de Clientes por Cluster**

![g1](https://github.com/user-attachments/assets/cc3d44d6-dcda-42af-a6d9-a91d57b05eac)

**Interpretação:**  
Este gráfico de barras mostra o número de clientes em cada cluster gerado pelo algoritmo K-Means. Podemos observar que a maior parte dos clientes está concentrada em clusters específicos, o que pode indicar grupos predominantes em termos de comportamento de compra.

---

### 📍 **Gráfico 2: Boxplot com Outliers (Valor Monetário, Frequência e Recência)**

![g2](https://github.com/user-attachments/assets/50937d74-e986-42a4-856d-52bfc91dbb4b)

**Interpretação:**  
O boxplot exibe a distribuição das variáveis Valor Monetário, Frequência e Recência, destacando a presença de outliers significativos. Estes outliers podem influenciar os clusters formados e devem ser tratados cuidadosamente.

---

### 📍 **Gráfico 3: Boxplot Sem Outliers (Valor Monetário, Frequência e Recência)**

![g3](https://github.com/user-attachments/assets/1ad9edc0-bdeb-4cc1-b1cc-8de50e3acec9)


**Interpretação:**  
Após a remoção dos outliers, o boxplot revela uma distribuição mais consistente das variáveis, permitindo uma análise mais precisa dos grupos de clientes. As diferenças entre os clusters tornam-se mais visíveis.

---

### 📍 **Gráfico 4: Scatter Plot 3D dos Dados por Cluster**

![g4](https://github.com/user-attachments/assets/f83375a4-7726-4ca6-8caf-4cb4e9b33bcf)

**Interpretação:**  
Este gráfico em 3D apresenta a separação dos clientes em diferentes clusters com base em três métricas principais: Valor Monetário, Frequência e Recência. Cada cor representa um cluster distinto, destacando a eficiência do modelo em identificar grupos de clientes.

---

### 📍 **Gráfico 5: Método do Cotovelo (Elbow Method)**


**Interpretação:**  
O Método do Cotovelo é utilizado para determinar o número ideal de clusters. O ponto de inflexão no gráfico ocorre em **k=4**, sugerindo que 4 clusters é a configuração mais eficiente para este conjunto de dados.

![g6](https://github.com/user-attachments/assets/26759c67-933b-4803-b106-74849b983346)

---

### 📍 **Gráfico 6: Pontuação Silhouette para Diferentes Valores de K**

![g7](https://github.com/user-attachments/assets/b253bcee-1660-4477-a0ca-0e037d40c1d5)

**Interpretação:**  
O gráfico de Pontuação Silhouette mostra a qualidade dos clusters formados para diferentes valores de **k**. A pontuação mais alta ocorre em **k=4**, indicando que os clusters gerados neste ponto são bem definidos.

---

### 📍 **Gráfico 7: Violin Plot - Valor Monetário por Cluster**

![g8](https://github.com/user-attachments/assets/64d53b04-51b0-4224-98a7-456c81ffd1f5)

**Interpretação:**  
O gráfico Violin Plot exibe a distribuição do Valor Monetário dentro de cada cluster. Podemos observar que alguns clusters possuem uma concentração maior de clientes com gastos elevados, o que pode indicar clientes de alto valor.

---

### 📍 **Gráfico 8: Violin Plot - Frequência por Cluster**

![g9](https://github.com/user-attachments/assets/1a110337-2a2b-4e4d-beb0-e98e5bc8c3ad)

**Interpretação:**  
O gráfico Violin Plot mostra a distribuição da Frequência de compra em cada cluster. Clusters com maior frequência de compra representam clientes que interagem regularmente com a empresa, demonstrando fidelidade à marca.

---

### 📍 **Gráfico 9: Violin Plot - Recência por Cluster**

![g9](https://github.com/user-attachments/assets/a0628f95-4114-48ef-9e4c-6476965b4dee)

**Interpretação:**  
A Recência por cluster indica quanto tempo se passou desde a última compra de cada grupo de clientes. Clusters com recência baixa representam clientes mais engajados recentemente, enquanto recência alta pode indicar clientes inativos.

---

### 📍 **Gráfico 10: Distribuição de Clientes por Cluster e Métricas Médias**

![g11](https://github.com/user-attachments/assets/d8eb97e3-7bf3-40e2-bc5c-e312ab8f6998)

**Interpretação:**  
Este gráfico mostra a distribuição de clientes por cluster juntamente com as médias das variáveis Recência, Frequência e Valor Monetário. Podemos observar que o Cluster 1 apresenta a maior média de Valor Monetário, sugerindo que este grupo contém os clientes mais valiosos para a empresa.

---

Essas visualizações oferecem uma compreensão clara dos padrões comportamentais identificados entre os clientes, permitindo a personalização de estratégias para cada grupo.

## 🚀 Conclusões do Projeto

A aplicação do algoritmo **K-Means Clustering** neste projeto permitiu uma análise detalhada dos clientes, resultando em **segmentações claras e insights valiosos**. Abaixo estão as principais conclusões extraídas dos resultados e gráficos:

---

### 📌 **1. Identificação de Clusters com Comportamentos Distintos**

Os clientes foram agrupados em clusters com padrões de comportamento únicos, conforme mostrado nas visualizações. Os principais grupos identificados são:

- **Clientes de Alto Valor (Cluster 1):**  
  Estes clientes possuem um alto valor monetário e realizam compras frequentes. São considerados os mais lucrativos e devem ser priorizados em campanhas de retenção e fidelização.

- **Clientes Sensíveis a Preço (Cluster 2):**  
  Compram produtos quando há promoções ou descontos. Para este grupo, é importante oferecer incentivos financeiros, como cupons ou ofertas personalizadas.

- **Clientes Ocasionais (Cluster 3):**  
  Realizam compras esporádicas e têm um baixo valor médio. A estratégia para este grupo pode incluir programas de engajamento para aumentar a frequência de compras.

- **Clientes Recorrentes (Cluster 4):**  
  Este grupo é composto por clientes fiéis, que realizam compras regulares. Manter essa fidelidade é crucial para a estabilidade da receita.

---

### 📌 **2. Importância do Tratamento de Outliers**

O tratamento de outliers foi fundamental para melhorar a qualidade dos clusters. Inicialmente, havia grande variação nas métricas de valor monetário e frequência, mas após a remoção dos outliers, a separação dos grupos tornou-se mais clara e consistente.

---

### 📌 **3. Número Ideal de Clusters**

Com base no **Método do Cotovelo (Elbow Method)** e na **Pontuação Silhouette**, o número ideal de clusters para este conjunto de dados foi identificado como **k=4**. Este valor permitiu uma boa separação entre os grupos, com alto grau de coesão interna e distinção entre os clusters.

---

### 📌 **4. Insights Ações Estratégicas**

A análise dos clusters oferece insights práticos para a definição de estratégias de marketing personalizadas:

| **Cluster**             | **Ação Recomendada**                                          |
|-------------------------|---------------------------------------------------------------|
| Clientes de Alto Valor   | Programas de fidelidade, ofertas exclusivas                   |
| Clientes Sensíveis a Preço | Ofertas de descontos, campanhas de e-mail marketing          |
| Clientes Ocasionais      | Campanhas de reengajamento, comunicação personalizada          |
| Clientes Recorrentes     | Recompensas por lealdade, ofertas baseadas em comportamento   |

---

### 📌 **5. Retenção e Crescimento de Clientes**

Os insights obtidos podem ser utilizados para:

1. **Aumentar a retenção de clientes** através de campanhas direcionadas.
2. **Identificar oportunidades de upselling e cross-selling**.
3. **Reduzir a taxa de churn** com ações focadas em clientes que estão inativos há algum tempo.

---

### 📌 **6. Potencial de Crescimento com Clientes em Potencial**

Um grupo importante identificado no projeto é o de **Clientes em Potencial**, que apesar de terem um valor médio menor atualmente, apresentam grandes chances de crescimento. Esses clientes devem ser trabalhados com:

- **Programas de nutrição de clientes**.
- **Campanhas de acompanhamento pós-compra**.
- **Comunicações focadas em conversão e engajamento**.

---

### 📌 **7. Segmentação Personalizada para Melhor Tomada de Decisão**

A segmentação permitida pelo modelo K-Means oferece uma vantagem competitiva ao proporcionar um entendimento profundo do comportamento dos clientes. As empresas podem utilizar esses dados para:

- **Personalizar campanhas de marketing** com base nos clusters.
- **Alocar recursos de maneira eficiente**, focando nos grupos mais lucrativos.
- **Melhorar a experiência do cliente**, oferecendo serviços mais relevantes.

---

### 📌 **8. Próximos Passos e Melhorias Futuras**

Para continuar melhorando a análise de clusters e insights:

1. **Explorar outros algoritmos de clustering**, como DBSCAN e Hierarchical Clustering.
2. **Incorporar variáveis adicionais** no modelo, como dados demográficos e histórico de compras.
3. **Desenvolver dashboards interativos** para que a equipe de marketing possa acompanhar os insights em tempo real.
4. **Implementar campanhas baseadas nos clusters identificados** para medir o impacto nas taxas de retenção e receita.

---

### 🎯 **Conclusão Final**

A análise de clustering realizada neste projeto fornece **informações práticas e valiosas** para a segmentação de clientes. Ao entender os diferentes perfis de clientes, a empresa pode criar **campanhas mais eficazes**, **aumentar a retenção de clientes** e **maximizar a receita**.

O uso contínuo de técnicas de Machine Learning como o K-Means pode ajudar a empresa a se adaptar rapidamente às mudanças no comportamento dos clientes, garantindo um **crescimento sustentável a longo prazo**.

## Agradecimentos 👏

Gostaria de expressar minha gratidão à **Alura** por proporcionar o dataset utilizado neste projeto e por oferecer uma experiência de aprendizado prática e enriquecedora. Os ensinamentos disponibilizados durante o curso foram essenciais para o desenvolvimento das habilidades aplicadas aqui, como:

- Manipulação e limpeza de dados com `pandas`.
- Criação de visualizações significativas utilizando bibliotecas como `matplotlib`.
- Abordagem prática para resolver problemas reais no contexto de análise de dados.

Este projeto é um reflexo do impacto positivo de um ambiente de aprendizado estruturado e do suporte oferecido pela plataforma. Agradeço à equipe da Alura por tornar este projeto possível e por contribuir com minha jornada no mundo da ciência de dados.

<div align="center">
  <img src="https://github.com/user-attachments/assets/54afb33c-97be-40b6-8c96-0f12852e946f" alt="thank-you" width="500">
</div>

## 📞 Contato
- **LinkedIn:** [Eduardo Coqueiro](https://www.linkedin.com/in/eduardocoqueiro/)
- **Site:** [Eduardo Coqueiro](https://dataguy.my.canva.site/eduardo-coqueiro)
- **Kaggle:** [Eduardo Coqueiro](https://www.kaggle.com/eduardocoqueiro)



