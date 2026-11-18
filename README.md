# Sistema de Recomendação de Receitas Sustentáveis para Redução da Pegada Hídrica

## Sobre o projeto

Este projeto tem como objetivo desenvolver um sistema de recomendação de receitas que considere as preferências dos usuários e, simultaneamente, incentive escolhas alimentares mais sustentáveis, levando em conta o indicador de pegada hídrica (Water Footprint - WF).

A proposta busca equilibrar a personalização das recomendações com a conscientização sobre o impacto ambiental dos alimentos, contribuindo para o Objetivo de Desenvolvimento Sustentável 12 (ODS 12) — Consumo e Produção Responsáveis.

## Objetivos

- Desenvolver um sistema de recomendação de receitas.
- Analisar os históricos de interação dos usuários.
- Comparar diferentes técnicas de recomendação.
- Incorporar o indicador de pegada hídrica ao processo de recomendação.
- Avaliar o equilíbrio entre a relevância das recomendações e a sustentabilidade.

## Base de dados

O projeto utiliza dados da plataforma Planeat, disponibilizados no conjunto de dados Water Footprint Recommender System Data, da plataforma Kaggle.

As informações utilizadas incluem:

- Receitas e seus ingredientes.
- Indicador de pegada hídrica das receitas.
- Histórico de interações dos usuários com as receitas.

## Técnicas utilizadas

Foram exploradas as seguintes abordagens:

- Recomendação por popularidade.
- Filtragem colaborativa (Collaborative Filtering).
- Filtragem baseada em conteúdo (Content-Based).
- Sistema híbrido (Hybrid).
- Filtragem colaborativa com ajuste pelo indicador de pegada hídrica.

## Avaliação

O desempenho dos modelos foi comparado por meio das métricas:

- Precision@10.
- Recall@10.
- Média do indicador de pegada hídrica (WF) das receitas recomendadas.

## Resultados principais

A abordagem colaborativa com ajuste sustentável apresentou uma redução aproximada de 33,7% na média do indicador WF das receitas recomendadas, em comparação com o modelo colaborativo original.

Essa redução ocorreu com uma queda relativa aproximada de 4,2% no Recall@10, indicando um equilíbrio inicial entre personalização e sustentabilidade.

Os resultados foram obto e Produção Responsáveis, da Organização das Nações Unidas (ONU).

Autores

Felipe dos Santos Costa
Felipe Yuji Nakanishi
Raphael Camargo Eugenio da Silva
Vanessa Biesek Bartnicki

Universidade Presbiteriana Mackenzie — 2026
