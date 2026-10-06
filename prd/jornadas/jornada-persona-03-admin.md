# Jornada da Persona 3 — ADMIN

> **Persona:** FF-PER-03 — Alex Nunes
> **Status:** rascunho para validação
> **Tecnologias:** não definidas

## Objetivo

Compreender suas responsabilidades e limites e executar somente tarefas administrativas autorizadas.

## Limite desta jornada

Esta jornada é deliberadamente genérica. A persona não define se o ADMIN administra dados esportivos, usuários, permissões, conteúdo ou configurações. Nenhuma dessas capacidades é assumida como parte do produto.

## Jornada ponta a ponta

| Etapa | Ação e necessidade da pessoa | Interface (front-end) | Responsabilidade do sistema (back-end) | Resultado / exceção |
|---|---|---|---|---|
| 1. Receber ou identificar uma tarefa | Entende qual necessidade administrativa está tentando atender. | Não se presume uma fila, painel ou mecanismo de atribuição de tarefas. | Não se presume que o produto gerencie tarefas administrativas. | A jornada só pode avançar quando as responsabilidades do papel forem definidas. |
| 2. Confirmar responsabilidade e autorização | Verifica se a tarefa pertence ao seu papel e se está autorizada a executá-la. | Deve tornar compreensíveis as responsabilidades e os limites que forem definidos. A forma de exibição está em aberto. | Se houver ações administrativas no escopo, deve permitir apenas as ações autorizadas para o papel; o modelo de autorização está em aberto. | Tarefa autorizada segue; tarefa não autorizada não deve permitir a ação. O processo de encaminhamento não foi definido. |
| 3. Acessar informações e executar a tarefa | Consulta as informações necessárias e realiza a tarefa, se suportada e autorizada. | Apresenta somente as informações e ações pertinentes às responsabilidades que vierem a ser aprovadas. | Executa apenas as operações administrativas confirmadas para o produto. Domínios de dados e operações ainda não definidos. | A tarefa pode ser concluída dentro do escopo aprovado; sem essa definição, não há critério de aceite específico. |
| 4. Confirmar ou encaminhar | Verifica o resultado ou encaminha um impedimento. | Comunica o resultado ou a restrição de forma compreensível, caso esses fluxos sejam definidos. | Informa o estado da operação, se houver operação administrativa no escopo. Histórico, confirmação e recuperação dependem de validação. | A pessoa sabe se a tarefa foi concluída ou se precisa de outro processo, ainda a definir. |

## Bloqueio de definição

Não derivar funcionalidades concretas de administração até que responsáveis, tarefas, dados acessíveis, operações permitidas e limites de autorização sejam confirmados.

## Perguntas em aberto

- Quem é ADMIN no contexto do produto e quais resultados são de sua responsabilidade?
- Quais tarefas e dados fazem parte do papel? Há consulta, alteração de dados, gestão de usuários, permissões, conteúdo ou configurações?
- Quais limites de acesso se aplicam e como devem ser apresentados?
- Se houver alterações, quais ações exigem confirmação, revisão, histórico ou possibilidade de recuperação?
- Como encaminhar tarefas fora da responsabilidade ou autorização da pessoa?

## Base e rastreabilidade

- [Persona ADMIN](./personas/Admin.md)
- [Requisitos funcionais](./jornadas-e-requisitos-funcionais.md): candidatos RF-C05 a RF-C07.

As personas são arquétipos ilustrativos; esta jornada é inicial e deve ser validada com responsáveis pelo produto antes de especificar funcionalidades administrativas.
