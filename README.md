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

Na reconstrução dos testes, o modelo colaborativo apresentou Recall@10 de 19,37% e média WF de 420,04.

Com a inclusão do critério de sustentabilidade, o Recall@10 passou para 18,25% e a média WF foi reduzida para 279,78.

Isso representa uma redução aproximada de 33,4% na média do indicador WF, com uma queda relativa de aproximadamente 5,8% no Recall@10.

Os resultados foram obtidos por avaliação offline, utilizando dados históricos da plataforma Planeat. Não representam uma validação com usuários em tempo real.

## Autores

Felipe dos Santos Costa

Felipe Yuji Nakanishi

Raphael Camargo Eugenio da Silva

Vanessa Biesek Bartnicki

Universidade Presbiteriana Mackenzie — 2026
