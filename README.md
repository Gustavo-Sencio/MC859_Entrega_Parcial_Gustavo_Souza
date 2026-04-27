# Rede de Coautoria Científica da UNICAMP (2021–2025)

Este repositório contém a instância de grafo e os dados usados para a constução do mesmo. Os dados foram coletados a partir da base Scopus, considerando publicações no período de 2021 a 2025.

## Conteúdo do repositório

- `coauthorship.graphml`: instância principal do grafo de coautoria
- `OutrosDados/`: Dados iniciais em CSV

## Definição do grafo

O grafo é não direcionado.

- Cada vértice representa um autor
- Cada aresta representa a existência de ao menos uma coautoria entre dois autores
- O peso da aresta corresponde ao número de artigos publicados em conjunto pelo par de autores

Atributos dos vértices:
- `author_id`
- `nome`
- `universidade`
- `cidade`
- `macro_area_principal_no_recorte`
- `macro_areas_no_recorte`
- `temas_no_recorte`
- `article_count`

## Métricas principais

- Número de vértices: `24867`
- Número de arestas: `56076`
- Grau médio: `4.5101`
- Número de componentes conexas: `1703`
