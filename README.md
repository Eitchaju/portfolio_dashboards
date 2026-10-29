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

## Imagens do dashboard
Adicione capturas reais à pasta `imagens/`. Quando estiverem disponíveis, inclua-as aqui no README para que o projeto possa ser visto sem abrir o Power BI.

## Limitações e próximos passos
- Dados sintéticos; não permitem generalizações para uma operação real.
- Relações entre indicadores são descritivas, não evidência de causalidade.
- Antes de comparar períodos, confirme equivalência de meses e filtros aplicados.
- Recomenda-se validar segmentações, medidas e formatação após atualizar a base no Power BI Desktop.

## Autoria
Projeto de portfólio de Business Intelligence. **Personalize esta seção com seu nome profissional e o link do LinkedIn antes de publicar.**
