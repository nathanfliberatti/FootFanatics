# Jornada da Persona 2 — Torcedor

> **Persona:** FF-PER-02 — Camila Oliveira
> **Status:** rascunho para validação
> **Tecnologias:** não definidas

## Objetivo

Encontrar a situação do clube no Campeonato Brasileiro e compreender resultados e desempenho no contexto da competição.

## Jornada ponta a ponta

| Etapa | Ação e necessidade da pessoa | Interface (front-end) | Responsabilidade do sistema (back-end) | Resultado / exceção |
|---|---|---|---|---|
| 1. Identificar o clube ou a competição | Procura a situação de um clube que acompanha ou consulta a competição como um todo. | Permite chegar às informações de classificação, resultados e times. A forma de seleção, busca ou personalização ainda não está definida. | Disponibiliza o contexto da competição e os times cobertos pelos dados. | A pessoa inicia a consulta; acompanhar um ou vários clubes como preferência é candidato a validação, não requisito assumido. |
| 2. Verificar a classificação | Consulta a posição atual do clube e sua situação na tabela. | Apresenta a classificação e destaca os dados necessários para entender a posição, sem pressupor um critério visual específico. | Fornece os dados da classificação referentes à competição. Critérios de atualização e desempate precisam ser definidos. | A pessoa entende a posição; indisponibilidade ou desatualização dos dados deve ser tratada explicitamente após definição da política de dados. |
| 3. Consultar resultados | Verifica resultados relacionados ao clube e à competição. | Apresenta resultados com identificação suficiente para relacioná-los aos times e ao contexto do campeonato. | Disponibiliza os resultados cobertos pelo produto e o contexto necessário para apresentá-los. | A pessoa encontra o histórico de resultados disponível; quantidade e recorte temporal ainda não foram especificados. |
| 4. Entender o desempenho | Explora estatísticas e indicadores para compreender a campanha. | Apresenta estatísticas em linguagem acessível e conecta os indicadores ao desempenho do time. | Disponibiliza estatísticas e indicadores de desempenho contemplados no escopo, de forma coerente com os resultados. | A pessoa entende o que os indicadores representam; métricas prioritárias e explicações específicas dependem de validação. |
| 5. Retomar o acompanhamento | Volta à plataforma para verificar a situação do clube e da competição. | Torna novamente acessíveis classificação, resultados e desempenho. | Disponibiliza os dados vigentes para uma nova consulta. | A pessoa acompanha a competição ao longo do tempo; histórico de evolução, alertas e notificações não estão incluídos sem validação. |

## Variações e lacunas

- Confirmar se próximos jogos e calendário fazem parte do escopo.
- Validar se a pessoa precisa definir um clube favorito ou acompanhar mais de um.
- Confirmar se é necessária a evolução histórica da tabela ou um resumo do impacto de cada rodada.
- Definir a frequência de atualização necessária para classificação, resultados e desempenho.

## Base e rastreabilidade

- [Persona Torcedor](./personas/torcedor.md)
- [Requisitos funcionais](./jornadas-e-requisitos-funcionais.md): RF-01 a RF-04 e RF-07; candidatos RF-C01 a RF-C03.

As personas são arquétipos ilustrativos; esta jornada é inicial e deve ser validada com usuários e responsáveis pelo produto.
