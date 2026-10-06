# Jornadas e requisitos funcionais — FootFanatics

> **Status:** rascunho para validação
> **Escopo:** jornadas de Investidor, Torcedor e ADMIN; requisitos funcionais derivados das personas existentes.
> **Tecnologias:** não definidas.

## 1. Propósito e base

Este documento reúne requisitos funcionais iniciais para o FootFanatics e serve como índice das jornadas detalhadas por persona. Cada jornada considera a experiência na interface e as responsabilidades do sistema e dos serviços de dados, sem definir tecnologias.

As personas são arquétipos ilustrativos, não resultados de pesquisa com usuários reais. Por isso:

- **Derivado do escopo descrito:** classificação, resultados, estatísticas, desempenho dos times, probabilidades, projeções e análises baseadas em dados relacionados ao Campeonato Brasileiro.
- **Candidato a validar:** capacidades mencionadas como hipóteses ou possibilidades nas personas.
- **Não definido:** decisões sem informação suficiente para especificar comportamento ou critérios mensuráveis. Não devem ser tratadas como requisitos aprovados.

As descrições de interface e de sistema são responsabilidades conceituais, não uma arquitetura técnica. Não se presume uso para apostas nem recomendação financeira.

## 2. Jornadas por persona

- [Persona 1 — Investidor](./jornada-persona-01-investidor.md)
- [Persona 2 — Torcedor](./jornada-persona-02-torcedor.md)
- [Persona 3 — ADMIN](./jornada-persona-03-admin.md)

## 3. Requisitos funcionais iniciais

Os requisitos **RF-01 a RF-07** derivam do escopo e das necessidades descritas nas personas, mas permanecem em rascunho até validação. Os requisitos **RF-C01 a RF-C07** são candidatos condicionais e não devem ser tratados como compromisso de produto.

### 3.1 Derivados do escopo descrito

| ID | Requisito funcional | Origem | Interface | Sistema / serviços | Critério de aceite inicial |
|---|---|---|---|---|---|
| RF-01 | O produto deve apresentar a classificação do Campeonato Brasileiro e permitir que a pessoa compreenda a posição dos times na competição. | Torcedor; contexto do produto | Apresenta a classificação e os dados que a compõem de forma compreensível. | Disponibiliza os dados de classificação para a competição contemplada. | Dado que há dados de classificação disponíveis, quando a pessoa consultar a competição, então deve conseguir identificar a posição de cada time coberto. |
| RF-02 | O produto deve apresentar resultados do Campeonato Brasileiro relacionados aos times e à competição. | Torcedor e Investidor; contexto do produto | Apresenta os resultados com identificação dos times e contexto suficiente para leitura. | Disponibiliza resultados correspondentes à competição. O recorte temporal será definido. | Dado que há resultados disponíveis, quando a pessoa consultar os resultados, então cada resultado exibido deve estar associado aos times e à competição correspondentes. |
| RF-03 | O produto deve apresentar estatísticas e indicadores de desempenho dos times contemplados no escopo. | Torcedor e Investidor; contexto do produto | Identifica as métricas apresentadas e exibe seus valores de forma legível. | Disponibiliza valores e definições das métricas que forem aprovadas. | Dado que uma métrica faz parte do escopo e tem dados disponíveis, quando for exibida, então seu nome e valor devem estar associados ao time e ao contexto definidos para essa métrica. |
| RF-04 | O produto deve contextualizar estatísticas e indicadores para ajudar a pessoa a compreender o desempenho, sem exigir conhecimento estatístico avançado como pressuposto. | Torcedor e Investidor; necessidades das personas | Apresenta explicações ou contexto para as métricas aprovadas. | Fornece as definições necessárias à apresentação. Quais métricas exigem explicação ainda precisa ser validado. | Dada uma métrica exibida, quando a pessoa consultar seu significado, então deve encontrar uma definição compreensível aprovada para essa métrica. |
| RF-05 | O produto deve disponibilizar probabilidades, projeções e análises baseadas em dados que forem incluídas no escopo. | Investidor; contexto do produto | Identifica claramente probabilidades e projeções como estimativas, distintas de resultados observados. | Disponibiliza as estimativas e análises aprovadas com o contexto associado que vier a ser definido. | Dado que uma probabilidade ou projeção está disponível, quando for exibida, então não deve ser apresentada como resultado confirmado ou garantia de desfecho. |
| RF-06 | O produto deve apresentar contexto suficiente para interpretar probabilidades e projeções, incluindo período de referência e limitações relevantes quando definidos. | Investidor; necessidades e critérios de utilidade | Exibe o período e as limitações disponíveis junto à estimativa correspondente. | Associa à estimativa o contexto aprovado; metodologia, fonte e frequência de atualização permanecem decisões em aberto. | Dada uma estimativa exibida com contexto definido, quando a pessoa a consultar, então deve conseguir identificar o período de referência e as limitações registradas para ela. |
| RF-07 | O produto deve manter coerência entre classificação, resultados, estatísticas e desempenho apresentados para o mesmo contexto de competição. | Torcedor e Investidor; critérios de utilidade | Evita apresentar informações conflitantes como se fossem do mesmo contexto. | Fornece dados associados à competição e ao período correspondentes. As regras de atualização e resolução de divergências precisam ser definidas. | Dado que mais de uma dessas informações é exibida para o mesmo contexto, quando forem consultadas, então as relações entre competição, time e período devem ser consistentes segundo as regras de domínio aprovadas. |

### 3.2 Candidatos condicionais a validação

| ID | Requisito candidato | Origem | Condição para aprovação |
|---|---|---|---|
| RF-C01 | Apresentar próximos jogos e calendário da competição. | Torcedor | Confirmar se agenda futura está dentro do escopo e quais informações devem ser exibidas. |
| RF-C02 | Permitir que a pessoa defina um ou mais clubes para acompanhamento recorrente. | Torcedor | Confirmar necessidade, quantidade de clubes e se a preferência deve persistir entre consultas. |
| RF-C03 | Apresentar a evolução da classificação e do desempenho ao longo da temporada. | Torcedor e Investidor | Confirmar período histórico, granularidade e valor para cada persona. |
| RF-C04 | Permitir comparar times, métricas ou períodos. | Investidor | Confirmar quais comparações apoiam uma tarefa real e quais métricas são comparáveis. |
| RF-C05 | Informar ao ADMIN suas responsabilidades e limites de acesso. | ADMIN | Definir primeiro quem é ADMIN, suas responsabilidades e o modelo de autorização do produto. |
| RF-C06 | Permitir ao ADMIN executar operações administrativas autorizadas e impedir operações não autorizadas. | ADMIN | Definir as operações, dados, permissões e consequências de cada ação. Não implica gestão de usuários, dados esportivos ou configurações. |
| RF-C07 | Apresentar ao ADMIN o resultado de uma operação e, se necessário, permitir confirmar, revisar ou recuperar uma alteração. | ADMIN | Confirmar se operações alteram dados e quais controles de confirmação, rastreabilidade e recuperação são necessários. |

## 4. Itens fora de definição — não assumir

- Gestão de usuários, permissões, dados esportivos, conteúdo ou configurações pelo ADMIN.
- Área, painel, fila ou fluxo de trabalho administrativo.
- Agenda de próximos jogos, favoritos, alertas, notificações ou personalização.
- Cobertura de competições ou divisões além do Campeonato Brasileiro indicado nas personas.
- Recomendação de investimento, recomendação financeira ou funcionalidade de apostas.
- Fonte dos dados, método de cálculo, periodicidade de atualização, métricas específicas e níveis de disponibilidade.
- Tecnologias, arquitetura, APIs, armazenamento ou integrações.

## 5. Perguntas para validação

1. Quais tarefas e quais tipos de dado pertencem realmente ao papel ADMIN? Ele consulta dados, altera dados, administra usuários, permissões, conteúdo ou configurações?
2. O que “Investidor” significa no contexto do produto e que decisão relacionada ao futebol pretende apoiar?
3. Quais métricas, períodos e explicações são prioritários para Torcedor e Investidor?
4. Próximos jogos, seleção de clube preferido, evolução histórica e comparação entre times fazem parte do escopo inicial?
5. Quais são as fontes, definições, períodos de referência e frequências de atualização dos dados e estimativas?
6. Como tratar ausência, atraso ou divergência de dados para cada informação apresentada?
7. Há limites explícitos sobre recomendações financeiras ou apostas além de não presumir essas capacidades?

## 6. Rastreabilidade às personas e jornadas

- [Persona 1 — Investidor](./jornada-persona-01-investidor.md): usa desempenho, probabilidades e projeções como insumos, considerando contexto e incerteza. A decisão específica, comparação e metodologia permanecem em aberto.
- [Persona 2 — Torcedor](./jornada-persona-02-torcedor.md): acompanha clube e competição por classificação, resultados, estatísticas e desempenho. Próximos jogos, preferências e evolução histórica permanecem candidatos.
- [Persona 3 — ADMIN](./jornada-persona-03-admin.md): compreende responsabilidades e executa somente tarefas autorizadas. A jornada e os requisitos administrativos concretos dependem de definição de escopo.
- Personas: [Investidor](./personas/investidor.md), [Torcedor](./personas/torcedor.md) e [ADMIN](./personas/Admin.md).
- [Índice de personas](./personas/README.md): registra limites, hipóteses e perguntas abertas que este documento preserva.
