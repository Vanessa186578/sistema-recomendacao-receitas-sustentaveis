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

## Ação extensionista — Alimentação e Consumo Consciente de Água

Como parte da ação extensionista, foi desenvolvido e divulgado um formulário online para investigar os hábitos alimentares da comunidade, o conhecimento sobre pegada hídrica e o interesse em recomendações de receitas sustentáveis.

**Formulário:** https://docs.google.com/forms/d/e/1FAIpQLScj7ptZBhjQEQVk4zf6h2rXSvmm0aedbLr0lXsxfuJ1zvwweg/viewform?usp=dialog

### Resultados da pesquisa

A pesquisa recebeu 36 respostas. Entre os principais resultados:

- 75% dos participantes nunca tinham ouvido falar sobre pegada hídrica dos alimentos.
- 86,1% afirmaram que nunca ou raramente consideram o impacto ambiental dos ingredientes ao escolher receitas.
- 41,7% utilizariam um sistema de recomendação que considerasse preferências e pegada hídrica, enquanto 50% responderam talvez.
- 61,1% estariam dispostos a experimentar uma receita diferente com menor pegada hídrica, desde que adequada às suas preferências.
- 91,7% responderam sim ou talvez à possibilidade de considerar o consumo de água na escolha de receitas após conhecer essa relação.]

## Relatório da ação extensionista

Os resultados consolidados da pesquisa, a metodologia e a análise das respostas estão disponíveis no [Relatório da Ação Extensionista](documentacao/relatorio_acao_extensionista.md).

O relatório apresenta apenas dados agregados, sem divulgar respostas individuais dos participantes.

### Contribuições para o projeto

Os resultados indicam uma oportunidade de ampliar a conscientização sobre a pegada hídrica dos alimentos e oferecer recomendações que conciliem preferências pessoais e sustentabilidade.

As respostas foram analisadas de forma descritiva para compreender o público e orientar a proposta extensionista. Não foram utilizadas no treinamento dos modelos de recomendação.

A pesquisa é exploratória e seus resultados representam apenas os participantes do formulário, não sendo generalizáveis à população.

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

## Como executar o projeto

O projeto pode ser executado gratuitamente pelo Google Colab, sem necessidade de instalar Python no computador.

### Passo a passo

1. Acesse https://colab.research.google.com/.
2. Selecione a opção GitHub na janela de abertura de notebooks.
3. Pesquise pelo repositório `Vanessa186578/sistema-recomendacao-receitas-sustentaveis`.
4. Abra o arquivo `notebooks/recomendacao_receitas_planeat_corrigido.ipynb`.
5. Clique em Ambiente de execução > Executar tudo.
6. Aguarde a execução das células para visualizar as análises, recomendações e métricas.

A primeira célula copia os arquivos do repositório para o ambiente temporário do Colab. As demais células carregam os dados, executam os modelos e apresentam os resultados.

### Estrutura do repositório

- `dados/`: arquivos CSV da base Planeat.
- `notebooks/`: código Python e testes do sistema de recomendação.
- `resultados/`: tabela comparativa dos modelos.
- `README.md`: documentação principal.

### Limitações

Os testes foram realizados offline, utilizando dados históricos. O indicador WF foi mantido conforme disponibilizado na base, sem atribuição de unidade física não confirmada. O sistema ainda não foi avaliado com usuários em produção.
