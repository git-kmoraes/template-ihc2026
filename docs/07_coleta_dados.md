# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** {{dd/mm/aaaa}}  
**Status:** 🟩 

## Objetivo da atividade

Planejar dados necessários para compreender usuários e requisitos de IHC, escolher técnicas adequadas e documentar instrumentos de modo que a aplicação possa ser reproduzida por pessoas diferentes.

## Para escopos de IHC derivados de TCC técnico

Quando o usuário e a interface foram propostos pela disciplina, uma prioridade da coleta é investigar se esse **cenário de uso realmente faz sentido**. Não trate o exercício de comercialização da Entrega 1 como validação de mercado.

Perguntas úteis incluem:

- esse perfil realmente realiza a atividade imaginada?
- quais ferramentas usa hoje?
- quais informações consulta?
- quais decisões toma?
- que vocabulário utiliza?
- quais parâmetros compreende e quais deveriam ser abstraídos?
- precisa de dashboard, histórico, filtros, relatórios ou comparação? Por quê?
- quais erros são frequentes e quais são críticos?
- existem papéis/permissões diferentes?
- que resultados do algoritmo/modelo seriam úteis ou difíceis de interpretar?

Quando o acesso ao perfil profissional for difícil, discuta com o docente alternativas metodológicas (especialistas próximos, dados secundários, literatura, participantes proxy) e registre as limitações. **Não esconda a limitação da amostra.**

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

Antes de decidir “que dados coletar”, retome os itens `[H]` e `[?]` da Entrega 1 e o registro de hipóteses em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md). A coleta deve responder perguntas reais do projeto, e não apenas produzir um formulário porque a técnica foi solicitada.

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H01 | informações sobre a perda ficam dispersas em mais de um canal | cenário C01 | centralização das informações | alta |
| H02 | quem encontra um item não sabe como encaminhá-lo | cenário C01 | instruções de registro e encaminhamento | alta |
| H03 | categoria, local, peroido e caractersticas ajudam a comparar registros | analise de concorrência | campos e filtros de busca | alta |
| H04 | detalhes não publicos ajudam a confirmar a propriedade | analise de concorrencia | mecanismo de confirmação de propriedade | alta |
| Q01 | existencia de processo oficial de achados e perdidos na FEI | não confirmado | definição do processo de devolução | alta |


## Parte A — necessidades e requisitos de IHC

### A01 — Karen Natally de Moraes

**Autor(a):** Karen Natally de Moraes

#### Que dados coletar?

| Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|
| canais utilizados para buscar itens perdidos | H01 | entender como os usuarios realizam a busca atualmente | organização das informações |
| dificuldades encontradas ao registrar um item | H02 | entender as necessidades de quem encontra um item perdido | formulario de registro |
| informações lembradas sobre o item perdido | H03 | identificar quais informações sao relevantes para a busca | filtros de busca |
| formas de comprovar propriedade | H04 | reduzir o risco de devolução incorreta | formulario de solicitação |
| conhecimento sobre o processo atual da FEI | Q01 | entender o contexto institucional | fluxo de encaminhamento e devolução |


#### De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| alunos | frequentar o campus | P01 e P02 |
| funcionarios da FEI | possuir conhecimento sobre o encaminhamento de itens perdidos | P03, papel ainda hipotetico |


#### Aspectos éticos

Analise voluntariedade, consentimento, minimização de dados, privacidade, riscos, gravação, anonimização, armazenamento e descarte. Não responda apenas “sim, por causa da LGPD”: explique **quais dados e riscos existem neste projeto**.

Não serão coletados nomes ou outras informações sensiveis, que permitam identificar os participantes

## Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

### Instrumento I01 — Questionário

**Autor(a):** Karen Natally de Moraes

**Técnica:** questionário

**Objetivo:** identificar o comportamento e as dificuldades dos usuarios durante a perda ou o encontro de um item no campus.

**Público:** estudantes e funcionarios da FEI.

#### Procedimento padronizado de aplicação

1. Disponibilizar o questionário em formato digital
2. Informar o objetivo da pesquisa e solicitar consentimento
3. Permitir que o participante responda individualmente
4. Agradecer a participação
5. Armazenar as respostas de forma anonima

#### Instrumento

1. Qual sua relação com a FEI?
   - estudante
   - funcionario
   - outro

2. Você já perdeu algum item dentro do campus?
   - sim
   - não

3. Caso tenha perdido um item, como realizou a busca?
   - procurei nos locais que frequentei
   - perguntei a outras pessoas
   - utilizei grupos de mensagens
   - procurei um setor responsável
   - outro

4. Quais dificuldades encontrou durante a busca?

5. Você já encontrou algum item perdido dentro do campus?
   - sim
   - não

6. Caso tenha encontrado, o que fez com o item?

7. Quais informações você normalmente consegue lembrar sobre um item perdido?
   - categoria
   - descrição
   - local
   - data
   - horario aproximado
   - outras características

8. Como você comprovaria que um objeto encontrado pertence a você?

9. Você conhece algum procedimento oficial de achados e perdidos da FEI?
   - sim
   - não

10. Caso conheça, como funciona esse procedimento?

11. O que poderia facilitar a busca e a recuperação de itens perdidos dentro do campus?


#### Como os dados serão analisados

- As respostas das perguntas fechadas serão analisadas atraves da distribuição das respostas
- As respostas abertas serão agrupadas de acordo com as dificuldades e necessidades identificadas

## Síntese

A coleta pretende validar as hipóteses H01, H02, H03 e H04 e investigar a lacuna Q01

## Checklist
- [x] Hipóteses/lacunas prioritárias da Entrega 1 foram revisitadas.
- [ ] Se o escopo de IHC foi derivado de TCC técnico, a coleta investiga a plausibilidade do usuário, tarefa e contexto adotados.
- [x] Perguntas não pressupõem que dashboard, CRUD, filtros ou relatórios sejam necessários; investigam a necessidade.
- [x] Cada dado a coletar responde uma dúvida concreta do projeto ou justifica outra necessidade de informação.
- [x] Parte A identifica dados e perfis de coleta de forma específica.
- [x] Aspectos éticos são contextualizados para o projeto.
- [x] Há uma técnica completa por integrante e técnicas distintas.
- [x] Questionário está incluído entre as técnicas.
- [x] Cada instrumento possui objetivo, público, procedimento e conteúdo integral.
- [x] Perguntas evitam indução e coletam apenas dados necessários.
- [x] Está claro como os dados serão analisados e usados no design.
