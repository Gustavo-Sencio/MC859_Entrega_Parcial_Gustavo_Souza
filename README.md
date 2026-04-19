# Rede de Coautoria Científica da UNICAMP (2021–2025)

Este repositório contém a instância de grafo e os artefatos de análise inicial do projeto da disciplina MC859 sobre redes de coautoria científica associadas à UNICAMP. Os dados foram coletados a partir da base Scopus, considerando publicações no período de 2021 a 2025.

## Conteúdo do repositório

- `coauthorship.graphml`: instância principal do grafo de coautoria
- `analyze_graphml.py`: script utilizado para gerar métricas e visualizações
- `analysis_output/`: saídas da análise inicial, incluindo gráficos, resumos e distribuições em CSV

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

## Métricas principais

- Número de vértices: `24867`
- Número de arestas: `56076`
- Grau médio: `4.5101`
- Número de componentes conexas: `1703`

## Reprodução da análise

Para reproduzir a análise inicial a partir do arquivo GraphML:

```bash
python3 analyze_graphml.py