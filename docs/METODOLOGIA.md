# Metodologia e documentação

## Escopo
Projeto demonstrativo de BI para análise de atendimento e experiência do cliente, utilizando base sintética.

## Dados e granularidade
- `base_satisfacao_clientes.csv`: registros de atendimento, um registro por `id_atendimento`.
- `evolucao_mensal_reclamacoes.csv`: evolução agregada mensal de reclamações.

## Etapas analíticas
1. Importação e tratamento dos CSVs no Power Query.
2. Modelagem de tabelas e calendário no modelo semântico.
3. Criação de medidas DAX para volumes, percentuais e evolução temporal.
4. Análise de séries históricas e segmentações por canal, região e categoria.
5. Interpretação dos resultados, ressalvando limitações de uma base fictícia.

## Cuidados com os indicadores
- Taxas de reclamações e reincidência: **menor é melhor**.
- Taxa de resolução e SLA cumprido: **maior é melhor**.
- CSAT e NPS usam escalas diferentes de 0–100; qualquer conversão para pontuação deve ser documentada.
- Faixas vermelho/amarelo/verde dependem de critérios de negócio explicitados no painel.
- Comparações anuais precisam de períodos equivalentes para evitar viés.

## Limitações
Dados sintéticos, padrões criados para fins didáticos, ausência de validação causal e eventual necessidade de remapear caminhos de arquivos ao abrir o PBIP em outro computador.

## Reprodução
Abra `portfolio.pbip` no Power BI Desktop e configure os caminhos dos CSVs se necessário.
