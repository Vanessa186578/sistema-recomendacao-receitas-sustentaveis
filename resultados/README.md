# Resultados dos Modelos

Esta pasta reúne os resultados preliminares da avaliação offline dos modelos de recomendação.

## Comparação dos modelos

| Modelo | Precision@10 | Recall@10 | Média WF |
|---|---:|---:|---:|
| Popularidade | 1,17% | 11,73% | 550,1 |
| Colaborativo | 1,34% | 13,41% | 407,3 |
| Baseado em conteúdo | 0,41% | 4,10% | 388,6 |
| Híbrido | 0,82% | 8,19% | 379,5 |
| Colaborativo + WF | 1,28% | 12,85% | 270,1 |

## Principais observações

- O modelo colaborativo apresentou o maior Recall@10.
- O ajuste sustentável reduziu em aproximadamente 33,7% a média do indicador WF em relação ao modelo colaborativo original.
- A queda relativa no Recall@10 foi de aproximadamente 4,2%.
- Os resultados foram obtidos em testes offline com dados históricos.

## Limitações

Os resultados são preliminares e não representam testes com usuários reais em funcionamento. A unidade física do indicador WF ainda precisa ser confirmada na documentação da base.
