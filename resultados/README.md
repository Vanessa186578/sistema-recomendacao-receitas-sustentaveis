# Resultados dos Modelos

Esta pasta reúne os resultados preliminares da avaliação offline dos modelos de recomendação.

## Comparação dos modelos

## Comparação dos modelos

| Modelo | Recall@10 | Média WF |
|---|---:|---:|
| Popularidade | 17,88% | 556,75 |
| Colaborativo | 19,37% | 420,04 |
| Baseado em conteúdo | 3,17% | 346,42 |
| Híbrido | 12,66% | 378,73 |
| Colaborativo + WF | 18,25% | 279,78 |

## Principais observações

- O modelo colaborativo apresentou o maior Recall@10.
- O ajuste sustentável reduziu em aproximadamente 33,7% a média do indicador WF em relação ao modelo colaborativo original.
- A queda relativa no Recall@10 foi de aproximadamente 4,2%.
- Os resultados foram obtidos em testes offline com dados históricos.

## Limitações

Os resultados são preliminares e não representam testes com usuários reais em funcionamento. A unidade física do indicador WF ainda precisa ser confirmada na documentação da base.
