# Repositório de Algoritmos de Machine Learning

Bem-vindo a este repositório! O objetivo aqui é fornecer implementações claras , em formato de Jupyter Notebooks, de diversos algoritmos e conceitos fundamentais de Machine Learning. Cada notebook é autônomo e focado em um único tópico, contendo tanto o código funcional quanto explicações teóricas.

## Estrutura do Repositório

Cada conceito ou algoritmo listado abaixo possui seu próprio notebook (`.ipynb`) neste repositório.

- `correlacao.ipynb`
- `regressao_linear.ipynb`
- `regressao_multivariavel.ipynb`
- `regressao_logistica.ipynb`
- `maxima_verossimilhanca.ipynb`
- `entropia_shannon.ipynb`
- `metodos_de_distancia.ipynb`
- `knn_k_nearest_neighbors.ipynb`
- `arvore_de_decisao.ipynb`
- `svm_support_vector_machine.ipynb`

---

## Visão Geral e Comparação dos Algoritmos

### Conceito de Informação

| Conceito | Descrição | Caso de Uso |
| :--- | :--- | :--- |
| **Correlação** | Mede a força e a direção da relação linear entre duas variáveis. Varia de -1 (correlação negativa perfeita) a +1 (correlação positiva perfeita). 0 indica ausência de correlação linear. | Análise Exploratória de Dados (EDA), para entender a relação entre features e identificar multicolinearidade. |
| **Máxima Verossimilhança (MLE)** | Um método para estimar os parâmetros de um modelo estatístico. A MLE busca os valores dos parâmetros que maximizam a probabilidade (verossimilhança) de observar os dados que foram coletados. | Base para muitos algoritmos de ML, como Regressão Logística. Usado para ajustar distribuições de probabilidade a um conjunto de dados. |
| **Entropia de Shannon** | Mede o nível de incerteza ou "surpresa" em uma variável aleatória. Quanto maior a entropia, mais incerto é o resultado. | Usada em Árvores de Decisão (critério de Ganho de Informação) para escolher a melhor feature para dividir os dados. Também fundamental em teoria da informação. |
| **Métodos de Distância** | Funções matemáticas que calculam a "distância" ou "similaridade" entre dois pontos (vetores) em um espaço. Essencial para algoritmos baseados em proximidade. | **KNN** (para encontrar vizinhos), **Clustering** (para agrupar pontos similares), sistemas de recomendação. A escolha da métrica (Euclidiana, Cosseno, etc.) depende da natureza dos dados. |

### Algoritmos de Regressão

| Algoritmo | Tipo | Descrição | Quando Usar |
| :--- | :--- | :--- | :--- |
| **Regressão Linear** | Supervisionado | Modela a relação entre uma variável dependente (contínua) e uma variável independente, ajustando uma linha reta aos dados. | Para prever valores contínuos (ex: preço de uma casa baseado no seu tamanho). Relação esperada é linear. |
| **Regressão Multivariável** | Supervisionado | Uma extensão da Regressão Linear, onde a variável dependente é modelada com base em **duas ou mais** variáveis independentes. | Similar à linear, mas quando o resultado depende de múltiplos fatores (ex: prever salário baseado em idade, anos de experiência e nível de educação). |
| **Regressão Logística** | Supervisionado | Apesar do nome "regressão", é um algoritmo de **classificação**. Ele prevê a probabilidade de uma ocorrência, mapeando qualquer valor real para um valor entre 0 e 1. | Para problemas de classificação binária (Sim/Não, Aprovado/Reprovado) ou multiclasse. |

### Algoritmos de Classificação

| Algoritmo | Tipo | Como Funciona | Prós e Contras |
| :--- | :--- | :--- | :--- |
| **KNN** | Supervisionado | Classifica um novo ponto de dado com base na classe majoritária de seus 'K' vizinhos mais próximos. É um algoritmo "preguiçoso" (não aprende um modelo, apenas armazena os dados). | **Prós:** Simples de entender e implementar. **Contras:** Lento em tempo de predição para grandes datasets, sensível a features irrelevantes e à escala dos dados. |
| **Árvore de Decisão** | Supervisionado | Cria um modelo semelhante a um fluxograma, onde cada nó interno representa um teste em um atributo (feature), cada ramo representa o resultado do teste e cada folha representa uma classe. | **Prós:** Fácil de interpretar e visualizar. **Contras:** Propenso a overfitting (pode ser mitigado com poda ou usando Random Forests). |
| **SVM** | Supervisionado | Encontra o "hiperplano" que melhor separa as classes de dados no espaço de features, maximizando a margem (distância) entre os pontos mais próximos de cada classe (vetores de suporte). | **Prós:** Eficaz em espaços de alta dimensão, bom desempenho com margem de separação clara. **Contras:** Computacionalmente caro para treinar, menos interpretável que uma árvore de decisão. |

## Como Usar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git)
    ```
2.  **Navegue até o diretório:**
    ```bash
    cd NOME_DO_REPOSITORIO
    ```
3.  **Instale as dependências:**
    ```bash
    pip install numpy pandas scikit-learn matplotlib seaborn jupyter
    ```
4.  **Execute o Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  Abra qualquer um dos arquivos `.ipynb` para ver e executar o código.
