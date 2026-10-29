# Customer Experience Analytics — Metodologia

## Objetivo

Analisar indicadores de atendimento, satisfação, reclamações e qualidade, identificando tendências e segmentos que merecem investigação.

## Dados e granularidade

- `base_satisfacao_clientes.csv`: registros sintéticos, um registro por `id_atendimento`.
- `evolucao_mensal_reclamacoes.csv`: evolução mensal agregada de reclamações.
- `Dim_Calendario`: dimensão de datas do modelo semântico.

## Processo analítico

1. Importação e transformação de dados no Power Query.
2. Modelagem semântica e calendário.
3. Medidas DAX para volumes, médias, taxas e variações.
4. Comparações temporais e recortes por canal, região e categoria.
5. Visualização e interpretação descritiva de resultados.

## Indicadores e direção desejada

| Indicador | Interpretação |
| --- | --- |
| Taxa de reclamações | Menor é melhor |
| Taxa de reincidência em 30 dias | Menor é melhor |
| Taxa de resolução | Maior é melhor |
| SLA cumprido | Maior é melhor |
| CSAT médio | Maior é melhor; escala de 1 a 5 |
| NPS | Maior é melhor; escala de −100 a 100 |

As cores de desempenho representam regras analíticas adotadas no estudo, não metas universais. Comparações anuais exigem períodos equivalentes e atenção aos filtros aplicados.

## Limitações

Todos os dados são fictícios. Os padrões não representam clientes, instituições ou operações reais. Correlações observadas não demonstram causalidade. O projeto PBIP pode exigir ajuste dos caminhos dos CSVs ao ser aberto em outro computador.

## Reprodução

Após baixar o projeto completo, abrir `portfolio.pbip` no Power BI Desktop, configurar as fontes CSV locais se necessário e atualizar os dados.