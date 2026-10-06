# Jornada da Persona 1 — Investidor

> **Persona:** FF-PER-01 — Marcelo Costa
> **Status:** rascunho para validação
> **Tecnologias:** não definidas

## Objetivo

Usar dados de desempenho, probabilidades e projeções como insumos para uma análise relacionada ao futebol, sem tratar estimativas como garantias.

## Jornada ponta a ponta

| Etapa | Ação e necessidade da pessoa | Interface (front-end) | Responsabilidade do sistema (back-end) | Resultado / exceção |
|---|---|---|---|---|
| 1. Definir o que quer entender | Parte de uma questão ou oportunidade relacionada ao futebol. O tipo de investimento e a decisão específica ainda não foram definidos. | Oferece acesso às informações da competição e dos times, sem presumir filtros ou fluxos de análise específicos. | Disponibiliza os dados da competição contemplados no escopo. | A pessoa identifica quais informações estão disponíveis; a decisão que deseja apoiar permanece uma pergunta de pesquisa. |
| 2. Entender o contexto da competição | Consulta classificação e resultados para situar os times. | Apresenta classificação e resultados de forma legível e relacionados à competição. | Fornece dados correspondentes ao mesmo contexto de competição e informa indisponibilidade quando não houver dados para exibir. | A pessoa tem uma visão contextual; dados ausentes não devem ser apresentados como se fossem resultados confirmados. |
| 3. Examinar desempenho | Consulta estatísticas e indicadores para entender a atuação dos times. | Apresenta as métricas com rótulos compreensíveis e contexto suficiente para interpretá-las. | Disponibiliza as estatísticas e os indicadores contemplados no produto. Definições, período e origem dos dados ainda precisam ser definidos. | A pessoa consegue interpretar os indicadores disponíveis; métricas sem definição clara precisam ser esclarecidas antes da validação do requisito. |
| 4. Considerar probabilidades e projeções | Explora estimativas como uma perspectiva adicional. | Distingue claramente estimativas de resultados observados e apresenta suas limitações quando definidas. | Disponibiliza probabilidades, projeções e contexto associado, se houver dados para isso. Método e cadência de atualização não estão definidos. | A pessoa pode considerar estimativas sem que sejam apresentadas como certezas ou recomendações financeiras. |
| 5. Formar sua própria análise | Combina as informações consultadas como subsídio para uma decisão relacionada ao futebol. | Mantém visível o contexto necessário para a leitura dos dados, sem sugerir uma decisão de investimento ou aposta. | Preserva coerência entre classificação, resultados, estatísticas e estimativas referentes à competição. | A pessoa decide se os dados são relevantes para sua análise; o produto não presume nem executa a decisão por ela. |

## Variações e lacunas

- Definir quem é o “investidor” e qual decisão pretende apoiar.
- Confirmar quais métricas, períodos e comparações são necessárias.
- Validar o nível de familiaridade estatística dessa persona.
- Definir se há usos explicitamente fora do escopo, sem presumir recomendação financeira ou apostas.

## Base e rastreabilidade

- [Persona Investidor](./personas/investidor.md)
- [Requisitos funcionais](./jornadas-e-requisitos-funcionais.md): RF-02 a RF-07 e candidatos RF-C03 a RF-C04.

As personas são arquétipos ilustrativos; esta jornada é inicial e deve ser validada com usuários e responsáveis pelo produto.
