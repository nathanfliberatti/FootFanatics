# Personas do FootFanatics

## Base e limites

Este documento consolida três arquétipos para apoiar o levantamento de requisitos do FootFanatics, descrito como uma plataforma de acompanhamento do Campeonato Brasileiro com classificação, resultados, estatísticas, desempenho dos times, probabilidades de resultados, projeções e análises baseadas em dados.

Os nomes e perfis são ilustrativos, não representam entrevistas ou pesquisa com usuários reais. Capacidades citadas como potenciais, requisitos identificados como “a investigar” e necessidades sem confirmação não devem ser interpretados como funcionalidades existentes ou decisões de escopo. Não se presume uso para apostas.

## Lista das personas

| Persona | Objetivo principal | Documento |
|---|---|---|
| **Investidor (FF-PER-01)** | Usar dados de desempenho, probabilidades e tendências como subsídio para decisões relacionadas ao futebol. O tipo de investimento e a decisão ainda são lacunas. | [investidor.md](investidor.md) |
| **Torcedor (FF-PER-02)** | Acompanhar seu clube e a competição, incluindo classificação, resultados, próximos jogos, desempenho e evolução da temporada. | [torcedor.md](torcedor.md) |
| **ADMIN (FF-PER-03)** | Executar responsabilidades administrativas do FootFanatics dentro de limites autorizados; tarefas e permissões ainda não foram definidas. | [analista-de-futebol.md](analista-de-futebol.md) |

## Necessidades principais

- **Investidor:** contexto para interpretar desempenho, probabilidades e tendências; clareza sobre incertezas e sobre o tipo de decisão que pretende apoiar.
- **Torcedor:** encontrar a situação do clube e da competição, acompanhar resultados e entender a evolução da campanha; verificar próximos jogos se isso estiver no escopo.
- **ADMIN:** conhecer suas responsabilidades, limites de acesso e informações necessárias para tarefas administrativas; quais tarefas existem ainda é uma lacuna.

## Principais diferenças

- **Foco:** o investidor busca insumos para decisões relacionadas ao futebol; o torcedor prioriza acompanhar o clube e a competição; o ADMIN executa tarefas administrativas ainda não identificadas.
- **Profundidade:** o torcedor tende a precisar de informação direta e contextualizada; o investidor pode precisar de contexto para suas decisões; o nível de informação do ADMIN depende das responsabilidades que forem definidas.
- **Acesso:** investidor e torcedor são tratados como consumidores das informações do produto; as permissões e ações do ADMIN são uma lacuna e não devem ser presumidas.
- **Escopo de incerteza:** não se conhece o contexto decisório do investidor, o perfil de acompanhamento do torcedor nem as responsabilidades administrativas do ADMIN.

## Funcionalidades de maior interesse

| Persona | Maior interesse, conforme o escopo e as hipóteses registradas |
|---|---|
| Investidor | Desempenho, estatísticas, probabilidades, projeções e tendências; comparação e explicabilidade precisam ser validadas. |
| Torcedor | Classificação, resultados, desempenho e acompanhamento do clube; próximos jogos, clube favorito e evolução da tabela são itens a confirmar. |
| ADMIN | Tarefas administrativas relacionadas ao FootFanatics; gestão de dados, usuários, permissões ou configurações são possibilidades, não capacidades confirmadas. |

## Possíveis conflitos entre necessidades

- **Consumo versus administração:** interfaces e informações voltadas a torcedores podem não atender tarefas administrativas; a necessidade de áreas ou fluxos distintos depende das responsabilidades do ADMIN.
- **Acesso versus segurança:** tarefas administrativas podem exigir permissões que não devem ser concedidas a usuários comuns; tarefas e limites ainda precisam ser definidos.
- **Alteração versus integridade dos dados:** se o ADMIN puder alterar informações, prevenção de erros e rastreabilidade podem entrar em tensão com rapidez operacional.
- **Simplicidade versus controles:** controles adicionais podem proteger ações administrativas, mas também aumentar o esforço para concluir tarefas legítimas.
- **Expectativa versus escopo confirmado:** próximos jogos, seleção de clube e quaisquer ferramentas administrativas ainda não estão confirmados como capacidades do produto.
- Nenhum conflito de negócio está validado; esses pontos são riscos a discutir durante a definição de requisitos.

## Requisitos que podem ser derivados

Os itens abaixo são perguntas de requisito, não compromissos de produto:

- **REQ-PER-01:** quais dados de classificação, resultados, estatísticas e desempenho são necessários e com que atualização?
- **REQ-PER-02:** como probabilidades e projeções devem ser contextualizadas para evitar que sejam entendidas como certezas?
- **REQ-PER-03:** o produto precisa cobrir próximos jogos e calendário da competição?
- **REQ-PER-04:** que formas de acompanhamento de clube e evolução da temporada são necessárias?
- **REQ-PER-05:** quais responsabilidades, tarefas e limites de acesso pertencem ao papel ADMIN?
- **REQ-PER-06:** quais definições, fontes e limitações precisam ser visíveis para que os dados sejam interpretáveis?
- **REQ-PER-07:** o que significa apoiar uma decisão de investidor e que tipos de recomendação, se houver, estão fora do escopo?
- **REQ-PER-08:** o ADMIN precisa gerir dados, usuários, permissões ou configurações? Quais ações são permitidas?
- **REQ-PER-09:** ações administrativas precisam de confirmação, revisão ou histórico? Em quais situações?

## Lacunas a investigar

- Segmentos reais de usuários, frequência de uso e tarefas prioritárias; as personas ainda não foram validadas com pesquisa.
- Definição operacional de “investidor” e contexto das decisões que deseja apoiar.
- Perfil de familiaridade estatística do torcedor e do investidor.
- Métricas de desempenho e estatísticas prioritárias para cada segmento.
- Cobertura de próximos jogos, temporadas anteriores e limites temporais do produto.
- Necessidade de acompanhar um ou vários clubes.
- Fonte, atualização, definições e limitações dos dados, probabilidades e projeções.
- Responsabilidades administrativas, limites de acesso e necessidades operacionais do ADMIN.
- Necessidade de o ADMIN consultar ou alterar dados, gerir usuários/permissões ou configurar a plataforma.
- Se ações administrativas precisam de confirmação, revisão ou rastreabilidade.
- Critérios observáveis para medir utilidade, confiança e compreensão para cada persona.
- Limites do produto sobre aconselhamento financeiro ou apostas; não assumir nenhuma dessas capacidades.

## Perguntas para a próxima etapa de levantamento de requisitos

1. Quem são os usuários reais do FootFanatics e quais tarefas tentam concluir ao acompanhar o Campeonato Brasileiro?
2. O que “investidor” significa para este produto e que decisão relacionada ao futebol ele espera apoiar com dados?
3. O produto deve manter foco exclusivo no Campeonato Brasileiro? Quais temporadas ou divisões estão incluídas?
4. Quais dados são indispensáveis para cada persona: classificação, resultados, próximos jogos, estatísticas, desempenho, probabilidades ou projeções?
5. Qual frequência de atualização cada tipo de informação exige e o que significa “atualizado” para os usuários?
6. Como os usuários esperam entender as definições, o período e as limitações de estatísticas e probabilidades?
7. Quais informações administrativas o ADMIN precisa consultar ou alterar, se houver, e quais ações devem ser restritas?
8. O torcedor precisa selecionar um clube de preferência? Precisa acompanhar mais de um?
9. Qual profundidade histórica é necessária para as necessidades de acompanhamento e análise já confirmadas?
10. Existem usos explicitamente fora do escopo, como recomendações financeiras ou apostas?
11. Ações administrativas precisam de confirmação, revisão ou registro? Em quais casos?
12. Como será validada a utilidade de cada persona: quais tarefas e resultados observáveis indicariam sucesso?
13. Quais lacunas devem ser respondidas antes de converter estas hipóteses em requisitos aprovados?

## Rastreabilidade inicial

Cada requisito abaixo é uma proposta a investigar, não uma funcionalidade confirmada.

| Persona | Necessidade | Problema | Funcionalidade potencial | Requisito a investigar |
|---|---|---|---|---|
| Investidor | Interpretar desempenho e tendências | Informações dispersas ou sem contexto podem dificultar decisões relacionadas ao futebol. | Visão contextualizada de desempenho e tendências. | **INV-01 / INV-03:** quais indicadores, comparações e períodos apoiam a decisão real do usuário? |
| Investidor | Compreender probabilidades e projeções | Estimativas sem contexto podem ser confundidas com certezas. | Apresentação contextualizada de probabilidades e projeções. | **INV-02:** que período, limitações e explicações são necessários? |
| Investidor | Delimitar o uso pretendido | “Investidor” não identifica o tipo de decisão nem o usuário. | Não derivar funcionalidade específica antes de esclarecer o contexto. | **INV-04:** quem é o investidor e quais usos pertencem ao produto? |
| Torcedor | Acompanhar a situação do clube | Pode precisar reunir classificação, resultados e desempenho em diferentes fontes. | Acesso focado ao clube dentro das informações da competição. | **TOR-01 / TOR-05:** como o clube é escolhido e quais dados devem aparecer primeiro? |
| Torcedor | Saber resultados e próximos jogos | Resultado passado não responde quando o clube joga em seguida; agenda não está confirmada no escopo atual. | Consulta de resultados e, se aprovada, próximos jogos. | **TOR-02:** calendário e próximos jogos fazem parte do escopo? |
| Torcedor | Entender a evolução da campanha | Números isolados podem não mostrar como a situação mudou durante a temporada. | Visão da evolução do clube e da tabela. | **TOR-03 / TOR-04:** qual evolução apresentar e com que nível de explicação? |
| ADMIN | Conhecer responsabilidades e limites | Um papel administrativo ambíguo pode gerar tarefas sem responsável ou permissões inadequadas. | Definição explícita de responsabilidades e ações autorizadas. | **ADM-01 / ADM-03:** quem é o ADMIN e quais tarefas e limites de acesso se aplicam? |
| ADMIN | Consultar ou alterar informações necessárias | Sem identificar tarefas administrativas, não é possível saber quais dados ou controles são necessários. | Consulta ou gestão de dados da competição, somente se essa atribuição for confirmada. | **ADM-02:** quais informações e ações pertencem ao papel? |
| ADMIN | Evitar alterações indevidas | Se puder alterar dados, ações acidentais podem afetar informações da plataforma. | Confirmação, revisão ou histórico de alterações, caso necessário. | **ADM-04:** quais ações precisam desses controles? |
| ADMIN | Encaminhar tarefas fora de sua alçada | A falta de limites e processo pode deixar solicitações sem tratamento adequado. | Orientação ou fluxo de encaminhamento, se necessário. | **ADM-05:** como tarefas sem autorização devem ser tratadas? |