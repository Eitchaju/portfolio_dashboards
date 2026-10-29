# Customer Experience Analytics | Power BI

> **Projeto de portfólio — dados inteiramente sintéticos.** Nenhuma informação representa clientes ou empresas reais.

## Visão geral
Análise exploratória de experiência do cliente, satisfação e qualidade de atendimento. O painel ajuda a identificar tendências de reclamações, reincidência, resolução e cumprimento de SLA, além de comparar 2025 e 2026 e segmentar resultados por canal, região e categoria.

**Ferramentas:** Power BI Desktop, Power Query, DAX, modelagem semântica e CSV.

## Perguntas de negócio
- Como evoluíram os atendimentos, reclamações e a satisfação?
- Quais segmentos concentram maior volume de atendimentos e reclamações?
- Como mudaram SLA, CSAT e NPS entre 2025 e 2026?
- Quais sinais merecem investigação e priorização operacional?

## Páginas do relatório
1. **Capa** — apresentação do estudo.
2. **Visão Executiva** — indicadores e tendências gerais.
3. **Reclamações e Qualidade** — reclamações, reincidência, resolução e SLA.
4. **Comparativo 2025 × 2026** — evolução anual e análises por segmento.
5. **Sobre o Projeto | Metodologia** — contexto, definições, abordagem e limitações.

## Indicadores
- **CSAT médio:** média das notas de satisfação (escala 1 a 5).
- **NPS:** percentual de promotores menos percentual de detratores (escala −100 a 100).
- **Taxa de reclamações:** proporção de atendimentos classificados como reclamações.
- **Taxa de reincidência:** proporção definida pelo sinalizador de reincidência em 30 dias.
- **Taxa de resolução:** proporção de atendimentos resolvidos.
- **SLA cumprido:** proporção dentro do prazo acordado.

**Interpretação:** reclamações e reincidência são melhores quando menores; resolução, SLA, CSAT e NPS são melhores quando maiores. As faixas de cores do painel são critérios analíticos do estudo, não padrões universais.

## Base de dados
Os arquivos CSV ficam em `customer_experience_portfolio/`. A base é fictícia, com dados de atendimentos e uma tabela de evolução mensal. Consulte o arquivo `docs/METODOLOGIA.md` para premissas e cuidados de interpretação.

## Como abrir
1. Baixe o repositório em **Code → Download ZIP** e extraia tudo.
2. Instale/abra o **Power BI Desktop**.
3. Abra `portfolio.pbip` a partir da pasta extraída.
4. Se necessário, use **Transformar dados → Configurações da fonte de dados** para apontar os CSVs ao caminho local dentro de `customer_experience_portfolio/` e atualize o modelo.

O PBIP inclui o relatório e o modelo semântico editáveis. A disponibilidade dos dados ao abrir pode depender dos caminhos locais de origem no Power Query.

## Conheça o dashboard

### Capa — Customer Experience Analytics
![Capa do Customer Experience Analytics](imagens/01%20-%20Capa.png)

### Visão Executiva
Panorama de atendimentos, satisfação e indicadores de qualidade.

![Página Visão Executiva](imagens/02%20-%20Visao-executiva.png)

### Reclamações e Qualidade
Acompanhamento de reclamações, reincidência, resolução e SLA.

![Página Reclamações e Qualidade](imagens/03%20-%20Reclamacoes-qualidade.png)

### Comparativo 2025 × 2026
Evolução dos indicadores e comparações entre períodos.

![Página Comparativo 2025 e 2026](imagens/04%20-%20Comparativo-2025-2026.png)

### Sobre o Projeto | Metodologia
Objetivos, definições, abordagem analítica e limitações.

![Página Metodologia](imagens/05%20-%20Metodologia.png)

## Principais insights do cenário simulado

Os indicadores abaixo representam o recorte geral apresentado no dashboard, sem filtros adicionais. Como a base é sintética, os achados ilustram uma abordagem analítica e não descrevem uma operação real.

| Indicador | Resultado exibido |
| --- | ---: |
| Atendimentos | **3.258** |
| Reclamações | **1.298** |
| Taxa de reclamações | **39,84%** |
| CSAT médio | **3,69 / 5** |
| NPS | **−20,7** |
| SLA cumprido | **78,5%** |
| Reincidência em 30 dias | **25,6%** |
| Taxa de resolução | **83,8%** |

### 1. Crescimento de volume com pressão sobre a experiência

O painel indica aumento de atendimentos e reclamações ao longo do período analisado. Na comparação anual apresentada, o volume de atendimentos cresce **133,0%** e o de reclamações, **212,8%**. A diferença entre os ritmos de crescimento sugere a necessidade de investigar os motivos de contato e os segmentos mais afetados.

### 2. Queda acentuada no cumprimento do SLA em 2026

A série mensal mostra uma deterioração expressiva do SLA no segundo semestre de 2026, ao mesmo tempo em que os indicadores de satisfação também enfraquecem. Essa simultaneidade merece investigação, mas **não comprova relação causal**.

### 3. Reincidência e resolução como oportunidades de melhoria

A reincidência de **25,6%** sinaliza oportunidade de avaliar a efetividade das soluções e os motivos de novos contatos. A taxa de resolução de **83,8%** ajuda a acompanhar a capacidade de encerrar atendimentos, mas deve ser analisada em conjunto com reincidência, SLA e satisfação.

### 4. Segmentação para priorizar ações

As visões por **canal, região e categoria** permitem identificar onde se concentram volumes e reclamações. A priorização deve considerar tanto quantidades absolutas quanto taxas proporcionais, para evitar que segmentos maiores pareçam piores apenas pelo volume.

## Recomendações de negócio

1. Investigar a mudança de patamar do SLA em 2026, separando resultados por canal, região e categoria.
2. Analisar os principais motivos de reclamação e sua participação no volume total de atendimentos.
3. Acompanhar a reincidência em 30 dias junto à resolução e ao CSAT, buscando indícios de soluções pouco efetivas.
4. Definir metas e limites de alerta por indicador, respeitando a direção desejada de cada métrica: reclamações e reincidência **menores**; resolução, SLA, CSAT e NPS **maiores**.
5. Validar comparações anuais com períodos equivalentes e o mesmo contexto de filtros.

## Limitações e próximos passos
- Dados sintéticos; não permitem generalizações para uma operação real.
- Relações entre indicadores são descritivas, não evidência de causalidade.
- Antes de comparar períodos, confirme equivalência de meses e filtros aplicados.
- Recomenda-se validar segmentações, medidas e formatação após atualizar a base no Power BI Desktop.

## Autoria
**Julia Nayara Silva** — Portfólio de Business Intelligence e Análise de Dados.
