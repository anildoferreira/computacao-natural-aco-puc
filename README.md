# **Otimização de Rota com Colônia de Formigas (Computação Natural)**

Este repositório contém a implementação e análise de um algoritmo de Otimização por Colônia de Formigas (OCF) para resolver o Problema do Caixeiro-Viajante (PCV). O projeto foi desenvolvido como parte da disciplina de Computação Natural da PUC.

O objetivo foi encontrar a rota mais curta para conectar 10 Pontifícias Universidades Católicas (PUCs) localizadas na América do Sul.

## **🗺️ Visualização da Rota Otimizada**

A imagem abaixo mostra a melhor rota encontrada pelo algoritmo, plotada sobre um mapa geoespacial. A distância total da rota otimizada foi de **5826.92**.

*(**Instrução para você:** Insira aqui a imagem final do seu mapa com a rota, como mapa\_rota\_final.png)*

\!\[Imagem do mapa com a rota otimizada\](https://github.com/anildoferreira/computacao-natural-aco-puc/blob/main/Mapa.png?raw=true)

## **🚀 Tecnologias Utilizadas**

* **Linguagem:** Python 3  
* **Bibliotecas Principais:**  
  * geopandas & contextily: Para a criação de visualizações geoespaciais precisas.  
  * numpy: Para cálculos numéricos eficientes.  
  * matplotlib: Para a plotagem dos gráficos.  
  * shapely: Para a manipulação de geometrias (pontos e linhas).

## **🔬 Sobre o Algoritmo**

O algoritmo de Otimização por Colônia de Formigas é uma meta-heurística inspirada no comportamento de formigas reais que buscam o caminho mais curto entre a colônia e uma fonte de alimento. As principais características implementadas são:

* **Feromônio:** As formigas depositam feromônio nas arestas do grafo, influenciando a escolha das próximas cidades pelas outras formigas.  
* **Visibilidade (Distância):** A escolha do próximo nó também é influenciada pela distância (heurística gulosa), preferindo-se cidades mais próximas.  
* **Evaporação:** Para evitar a convergência prematura, o feromônio evapora a uma certa taxa (rho) a cada iteração.

Foram realizados experimentos com os parâmetros alpha (influência do feromônio), beta (influência da distância) e rho (taxa de evaporação) para analisar o impacto na eficiência e qualidade da solução.

## **⚙️ Como Executar**

O projeto foi desenvolvido em um ambiente de notebook (Jupyter/Google Colab).

1. **Clone o repositório:**  
   git clone \[https://github.com/seu-usuario/seu-repositorio.git\](https://github.com/seu-usuario/seu-repositorio.git)

2. **Abra o Notebook:**  
   * Carregue o arquivo AS2\_Codigo\_Anildo\_de\_Abreu Ferreira.ipynb no Google Colab ou em uma instância local do Jupyter.  
3. **Instalação de Dependências:**  
   * O notebook inclui uma célula que instala automaticamente as bibliotecas geopandas e contextily caso não estejam presentes no ambiente.  
4. **Execute as Células:**  
   * Execute todas as células em ordem para ver a análise e os resultados.
