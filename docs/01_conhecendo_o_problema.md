# Entrega 1 — Conhecendo o projeto, o usuário e o problema

**Data:** 23/09/2026  
**Status:** 🟩 concluída  
**Responsabilidade:** 1 solução consolidada por equipe

## Objetivo da atividade

Reinterpretar o tema do TCC sob a perspectiva de Interação Humano-Computador e construir um **entendimento comum entre os integrantes da equipe**.

A disciplina utiliza preferencialmente o tema do TCC para os exercícios de IHC. Isso vale tanto para TCCs que já preveem uma interface quanto para trabalhos cujo resultado principal é algoritmo, modelo, API, biblioteca, análise de dados, infraestrutura, estudo experimental ou outro artefato técnico.

> **Importante:** a interface projetada na disciplina é um artefato de aprendizagem de IHC. Ela **não se torna automaticamente uma obrigação do TCC**. Sua incorporação ao trabalho de conclusão depende de decisão da equipe e do orientador.

Antes de preencher, leia [`../GUIA_ESCOPO_IHC.md`](../GUIA_ESCOPO_IHC.md).

Nesta primeira semana a equipe **não deve começar desenhando telas**. Primeiro deverá compreender:

- o que o TCC realmente produz;
- quem poderia obter valor dessa contribuição;
- quais pessoas interagem, administram, configuram, interpretam ou são afetadas;
- o que essas pessoas precisam alcançar;
- como atividades relacionadas acontecem hoje;
- problemas, limitações e contexto;
- alternativas existentes;
- qual recorte de interação fará sentido para a disciplina.

Ao final desta entrega, a equipe deve diferenciar:

- **tema do TCC** × **escopo formal do TCC** × **escopo de IHC da disciplina**;
- **objetivo do projeto** × **objetivo do usuário**;
- **problema do usuário** × **solução tecnológica**;
- **fato conhecido** × **hipótese** × **lacuna de conhecimento**;
- **capacidade técnica** × **forma de uso dessa capacidade**;
- **funcionalidade** × **atividade/resultado que o usuário precisa alcançar**;
- **usuário direto** × **stakeholders**.

---

## Como classificar as respostas

Sempre que a resposta fizer uma afirmação sobre usuários, problemas, atividades, necessidades, contexto ou mercado, use:

- **[F] Fato conhecido** — existe evidência/fonte.
- **[H] Hipótese** — afirmação plausível que ainda precisa ser investigada.
- **[?] Não sabemos ainda** — lacuna relevante.

Quando usar `[F]`, informe a origem. Hipóteses prioritárias devem receber IDs (`H01`, `H02`...) e também ser registradas em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

> **Exemplo:** `[H] H01 — DBAs considerariam útil comparar automaticamente o plano atual de execução com uma recomendação produzida pelo algoritmo.`

Uma hipótese explicitada é melhor do que uma suposição escondida.

---

# 0. Identificação do TCC e da equipe

## 0.1 Membros

| Nome completo | Matrícula | GitHub |
|---|---:|---|
| Karen Natally de Moraes | 221210867 | @git-kmoraes |

## 0.2 Título atual do TCC

Achados e perdidos no campus da FEI.

## 0.3 Orientador(a)

Não se aplica ao recorte adotado.

## 0.4 Qual é o resultado principal atualmente previsto no TCC?

Marque e descreva:

- [x] sistema/aplicação interativa;
- [ ] algoritmo;
- [ ] modelo de IA/ML/LLM;
- [ ] biblioteca/API/framework;
- [ ] análise de dataset;
- [ ] estudo/benchmark/avaliação experimental;
- [ ] infraestrutura/backend;
- [ ] componente embarcado/IoT;
- [ ] outro: projeto acadêmico de IHC.

**Descrição:** sistema interativo para registrar perdas e achados, buscar e comparar possíveis correspondências, confirmar a propriedade e apoiar a devolução de objetos no campus.

## 0.5 O TCC já previa desenvolvimento de interface com usuário?

- [x] Sim, a interface já faz parte do TCC.
- [ ] Parcialmente; existe alguma interação, mas ainda não está bem definida.
- [ ] Não. O TCC é predominantemente técnico e não previa interface.

**Explique o que está formalmente previsto no TCC:** neste preenchimento, considera-se o projeto escolhido para a disciplina. O sistema de achados e perdidos já previa uma interface para registrar, buscar, comparar e acompanhar relatos de perda e achado.

> Esta resposta serve para separar o compromisso do TCC do projeto da disciplina. Mesmo quando a opção for **não**, a equipe irá definir uma interface para exercitar IHC.

---

# 1. Entendendo a contribuição do projeto

## 1.1 Explique o TCC em uma frase, sem citar linguagem de programação, framework ou banco de dados.

O projeto estuda como organizar informações sobre perdas e achados para apoiar a localização, a confirmação de propriedade e a devolução de objetos no campus.

## 1.2 Qual situação, atividade ou problema do mundo real motivou o TCC?

[H] H01 — informações sobre a perda e o achado podem ficar dispersas entre conversas, grupos de mensagens e contatos feitos em locais diferentes. Isso pode levar à repetição da busca e dificultar o encontro entre os relatos.

## 1.3 Qual é a **capacidade/contribuição central** produzida pelo TCC?

Complete, se ajudar:

> “Nosso TCC produz, melhora, analisa ou permite `organizar informações de perda, achado, comparação e devolução de objetos`.”

Exemplos: otimizar consultas; classificar imagens; detectar anomalias; comparar modelos; identificar padrões; prever demanda; analisar desempenho; gerar resumos; recomendar configurações.

Organizar relatos de perda e achado, apoiar a comparação entre informações e manter a continuidade até a devolução do objeto.

## 1.4 O que se espera que esteja diferente **para pessoas, organizações ou processos** se essa contribuição for bem-sucedida?

[H] Se essa organização for adequada, estudantes poderão reduzir buscas repetidas, quem encontra um item terá um encaminhamento mais claro e a devolução poderá ocorrer com menos risco de correspondência incorreta.

## 1.5 O que é mérito técnico/científico do TCC e o que seria uma possível aplicação prática?

| Mérito/contribuição técnica | Possível aplicação/valor em uso |
|---|---|
| Estruturar um recorte coerente de interação entre perda, achado, comparação e devolução | Tornar o processo mais compreensível para quem perdeu, encontrou ou participa da entrega |

---

# 2. Entendendo as pessoas envolvidas

## 2.1 Quem interage diretamente com o produto, se já existe interface prevista?

Se não houver interface prevista no TCC, escreva `NÃO SE APLICA AO ESCOPO ORIGINAL` e prossiga para 2.2.

P01 interage para registrar uma perda, buscar possíveis correspondências e acompanhar o caso. P02 registra um item encontrado e seu encaminhamento. P03 representa, como hipótese, uma pessoa que participa da comparação dos relatos e da devolução.

## 2.2 Quem poderia **usar, configurar, administrar, operar, interpretar ou tomar decisões** a partir da contribuição técnica?

Considere perfis profissionais e stakeholders, não apenas consumidores finais.

| Perfil | Relação com a contribuição | O que faria | Status/evidência |
|---|---|---|---|
| P01 — estudante que perdeu um item | fornece informações e procura possíveis correspondências | localizar, confirmar e recuperar o objeto | H |
| P02 — estudante que encontrou um item | registra o contexto do achado e encaminha o objeto | devolver o item sem assumir uma responsabilidade prolongada | H |
| P03 — pessoa que participa do recebimento ou da devolução | compara relatos, solicita complementos e registra a entrega | evitar devolução incorreta e manter o processo compreensível | H |

## 2.3 Existem pessoas afetadas que não usariam a interface diretamente?

| Stakeholder | Como é afetado | Usa interface? | Status/evidência |
|---|---|---|---|
| comunidade acadêmica | pode se beneficiar de um processo mais previsível | talvez | H — ainda sem pesquisa com participantes |
| instituição | pode precisar definir responsabilidades, guarda e descarte | talvez | ? — não foi confirmado processo oficial |

## 2.4 Que características desses perfis podem influenciar a interação?

Considere conhecimento do domínio, experiência tecnológica, frequência de uso, necessidades de acessibilidade, responsabilidade profissional, familiaridade com métricas, linguagem técnica, urgência etc.

[H] P01 pode estar com pressa, lembrar apenas parte do trajeto e usar o celular durante ou depois das atividades. [H] P02 pode ter pouco tempo e não saber quais dados registrar. [H] P03 pode precisar interpretar relatos contraditórios, preservar a privacidade e consultar um histórico. [?] Necessidades de acessibilidade e frequência de uso ainda não foram investigadas.

---

# 3. Entendendo objetivos e atividades

## 3.1 O que o usuário está tentando conseguir no mundo real?

Não responda “usar o algoritmo”, “clicar no sistema” ou “ver o dashboard”.

[H] P01 tenta recuperar o objeto; P02 tenta encaminhá-lo sem perder tempo; P03 tenta verificar a propriedade e concluir a devolução sem erro.

## 3.2 Quais são as atividades mais importantes?

| ID | Atividade/objetivo | Quem realiza | Frequência/criticidade inicial | Status/evidência |
|---|---|---|---|---|
| A01 | reconstruir onde e quando o objeto foi perdido | P01 | frequência desconhecida; alta importância para a busca | H |
| A02 | registrar características, local e horário do item encontrado | P02 | frequência desconhecida; a informação pode se perder com o tempo | H |
| A03 | comparar relatos, confirmar propriedade e combinar a devolução | P01, P02 e P03 | crítica para evitar correspondência incorreta | H |

## 3.3 Qual atividade parece mais frequente? Por quê?

[?] A frequência real não foi investigada. A01 parece iniciar a maior parte da jornada de P01, mas essa percepção precisa ser validada.

## 3.4 Qual parece mais crítica? Que consequência existe se for mal executada?

[H] A03 parece mais crítica porque uma comparação ou confirmação mal executada pode levar à entrega do objeto para a pessoa errada, à exposição de informações ou à perda definitiva do item.

---

# 4. Entendendo o problema ou processo atual

## 4.1 Como essas atividades são realizadas hoje, antes da interface imaginada na disciplina?

Pode existir software concorrente, linha de comando, planilha, notebook, script, painel técnico, processo manual, consulta a logs, análise visual, troca de mensagens, decisão por especialista etc.

[H] P01 pode refazer o caminho, perguntar a colegas, procurar nos locais visitados e divulgar uma descrição em canais informais. P02 pode perguntar a pessoas próximas, guardar o item temporariamente ou tentar entregá-lo a alguém. Se os relatos chegarem a P03, podem conter níveis diferentes de detalhe.

## 4.2 O que é difícil, demorado, confuso, repetitivo, arriscado ou pouco transparente?

[H] A busca pode ser repetida em vários lugares; relatos podem usar descrições diferentes; local, data e horário podem não ser registrados; a pessoa pode ficar sem retorno; e a confirmação de propriedade pode depender de perguntas improvisadas.

## 4.3 Que informações o profissional precisa interpretar para tomar decisão?

[H] Categoria, descrição, local, período, foto, contato e características que não foram divulgadas publicamente. [?] Ainda não se sabe quais desses dados são realmente usados no campus.

## 4.4 O que acontece quando a atividade falha ou quando o resultado é interpretado incorretamente?

[H] Uma falha pode atrasar a recuperação, manter P02 responsável pelo objeto por mais tempo ou levar P03 a confirmar uma correspondência com dados insuficientes. A interpretação incorreta pode causar entrega indevida ou exposição de informações.

## 4.5 Conte uma situação concreta.

Escreva uma pequena narrativa com pessoa, objetivo, atividade, contexto, dificuldade e consequência. **Não descreva ainda a futura solução.**

[H] Uma estudante percebe que perdeu a mochila depois de passar por mais de um ambiente do campus. Ela pergunta a colegas e retorna aos locais de que se lembra. Outro estudante encontra uma mochila, mas não sabe qual é o melhor encaminhamento. Quando os relatos chegam a uma terceira pessoa, cada um contém informações diferentes. A comparação demora e ainda existe o risco de entregar o objeto à pessoa errada.

## 4.6 Que evidência existe hoje?

| Evidência/fonte | O que sustenta | Limitação |
|---|---|---|
| [Nuvlost](https://nuvlost.com/university-lost-and-found) | existência de fluxo com registro, comparação, aviso e devolução | descreve um serviço externo, não o processo da FEI |
| [UCLA Lost & Found](https://lostandfound.ucla.edu/) | uso de categoria, local e período no relato de perda | contexto institucional diferente |
| [MissingX](https://www.missingx.com/en/help/quick-tour-of-missingx) | separação entre busca, reivindicação, confirmação e devolução | depende de escritórios cadastrados |

---

# 5. Entendendo o contexto de uso

## 5.1 Onde e em quais situações a interação poderia ocorrer?

[H] A interação pode ocorrer durante a circulação pelo campus, logo após perceber a perda ou mais tarde, quando P01 e P02 já estiverem fora do local.

## 5.2 Em quais dispositivos/equipamentos?

[H] Principalmente em celular para P01 e P02; celular ou computador para P03.

## 5.3 Existem condições físicas relevantes?

Considere iluminação, ruído, mobilidade, conexão, privacidade, uso compartilhado, interrupções, pressão de tempo etc.

[H] Mobilidade, pressa, interrupções, conexão variável e lembrança incompleta do trajeto podem afetar o preenchimento e a busca. A privacidade é relevante na confirmação de propriedade.

## 5.4 Existem fatores sociais ou organizacionais?

Considere papéis, chefias, equipes, permissões, aprovação, responsabilidade profissional, auditoria, turnos e colaboração.

[H] O processo depende da colaboração entre pessoas com objetivos diferentes. [?] Não foi confirmado quem recebe objetos, quais permissões existem nem quais regras de guarda e devolução seriam aplicadas.

## 5.5 Existe necessidade de histórico, rastreabilidade ou auditoria?

[H] Sim. O histórico pode mostrar quando um relato foi criado, quais informações foram complementadas, o estado de uma possível correspondência e se a devolução foi concluída.

## 5.6 Um erro pode produzir consequência relevante? Qual?

[H] Sim. Uma correspondência incorreta pode entregar o objeto à pessoa errada; informações expostas podem facilitar uma falsa reivindicação; e instruções ambíguas podem prolongar a responsabilidade de P02.

---

# 6. Entendendo mercado e alternativas existentes

> Nesta entrega faça apenas um **levantamento inicial**. A análise aprofundada ocorre na Entrega 2.

## 6.1 Como pessoas resolvem problemas semelhantes hoje?

| Alternativa atual | Quem usa | Para quê | Status/evidência |
|---|---|---|---|
| busca em locais visitados e conversa com pessoas próximas | P01 | tentar recuperar rapidamente o objeto | H — cenário inicial, ainda sem coleta |
| divulgação em canais informais | P01 e P02 | comunicar perda ou achado | H — canais reais ainda desconhecidos |
| Nuvlost | universidades e faculdades | registrar, comparar e devolver itens | F — site oficial |
| UCLA Lost & Found | comunidade universitária | relatar perdas e buscar itens encontrados | F — portal oficial |
| MissingX | pessoas e escritórios de achados e perdidos | buscar, reivindicar e confirmar itens | F — site oficial |

## 6.2 Existem produtos que atuam na mesma área, mesmo sem serem equivalentes ao TCC?

[F] Nuvlost, UCLA Lost & Found e MissingX atuam no mesmo domínio ou em processos análogos. A análise detalhada está na Entrega 2.

## 6.3 Quais interfaces profissionais esse público já conhece?

Exemplos possíveis: ferramentas de banco, IDEs, consoles de nuvem, dashboards, plataformas de dados, ferramentas de monitoramento, painéis de IA, sistemas administrativos.

[?] Ainda não houve pesquisa com participantes para afirmar quais interfaces são familiares ao público da FEI.

## 6.4 O que essas soluções parecem fazer bem?

[F] Nas soluções observadas, a separação entre relatar e buscar, a organização por categoria/local/período e a indicação do estado do caso ajudam a tornar as intenções e etapas mais claras.

## 6.5 O que parecem fazer mal, dificultar ou não atender?

[F] Formulários longos aumentam o esforço móvel; estados sem próxima ação podem gerar incerteza; e dados públicos em excesso podem prejudicar a confirmação segura da propriedade.

## 6.6 Que padrões de interface ou vocabulário parecem familiares a esse público?

[F] Busca inicial simples, categorias de item, filtros por local e período, marcação de campos obrigatórios, divisão do fluxo em estados e confirmação antes da devolução aparecem nas soluções analisadas.

---

# 7. Derivando o escopo de IHC da disciplina

## 7.1 Escolha o caminho do projeto

### Caminho A — TCC já possui interface

Explique qual parte da interface será usada como recorte da disciplina e por que esse fluxo é relevante.

O sistema de achados e perdidos já previa interface. O recorte da disciplina abrange o registro de perdas e achados, a busca e comparação de relatos, a confirmação da propriedade, o acompanhamento do caso e a devolução. Esse fluxo é relevante porque conecta os objetivos de quem perdeu, de quem encontrou e de quem participa da entrega.

### Caminho B — TCC não possui interface prevista

Faça o exercício de transferência de uso:

> **Imagine que o TCC foi concluído com sucesso e uma empresa, laboratório ou organização quer transformar a contribuição em algo utilizável. Quem precisaria interagir com ela e para quê?**

Não se aplica, pois a interface já fazia parte do projeto escolhido.

## 7.2 Qual perfil será priorizado no projeto de IHC?

P01 — estudante que perdeu um item.

**Por que esse perfil foi escolhido?** Porque recuperar o objeto é o resultado principal do recorte e depende da coordenação com P02 e P03.

## 7.3 Qual objetivo desse usuário será priorizado?

Localizar, confirmar e recuperar o objeto com o menor número possível de tentativas e com informações suficientes para evitar uma correspondência incorreta.

## 7.4 Que interface será explorada na disciplina?

Complete:

> **Para fins da disciplina de IHC, será projetada uma interface que permita ao `estudante que perdeu um item` utilizar `registros de perda, achado e possíveis correspondências` para `localizar, confirmar e recuperar o objeto`, no contexto da `rotina no campus`.**

A interface explorará o registro de perdas e achados, a busca e comparação entre relatos, o acompanhamento do estado do caso, a confirmação de propriedade e a devolução.

## 7.5 Qual é a relação dessa interface com o TCC?

- [x] Já fazia parte do TCC.
- [ ] É um aprofundamento de algo parcialmente previsto.
- [ ] É uma extensão conceitual criada para a disciplina.
- [ ] É um protótipo demonstrativo de aplicação potencial.
- [ ] Outra: não se aplica ao recorte adotado.

> **Declaração:** a interface já fazia parte do projeto escolhido. Na disciplina, será estudado e detalhado o recorte de registro, busca, comparação, confirmação de propriedade e devolução.

---

# 8. Levantando possibilidades de interação — sem desenhar ainda

A equipe pode registrar possibilidades para investigação. **Não significa que todas serão implementadas.**

Marque apenas as que parecem plausíveis e explique o objetivo correspondente.

| Possibilidade | Pode fazer sentido? | Objetivo/tarefa que justificaria | Evidência atual |
|---|---|---|---|
| Dashboard/visão geral | talvez | permitir a P03 acompanhar casos e pendências | P03 e o volume real ainda são hipóteses |
| Configuração/parametrização | não | não existe tarefa identificada nesta etapa | nenhuma |
| Entrada/upload/seleção de dados | sim | registrar descrição, local, período e foto | C01, C02 e C03 da análise de concorrência |
| Acompanhamento de processamento | não | não existe processamento técnico a acompanhar | nenhuma |
| Relatório/resultados | não | não existe tarefa de relatório identificada | nenhuma |
| Histórico com busca/filtros | sim | localizar registros e acompanhar o caso | H01, H03 e RC03 |
| Comparação de resultados | sim | comparar relatos de perda e achado | H03 e C01 |
| Explicabilidade/detalhamento | sim | explicar por que existe uma possível correspondência | H03 e H04 |
| Administração/configurações globais | talvez | organizar locais e estados se P03 for confirmado | Q01 pendente |
| Usuários/perfis/permissões | talvez | proteger contato e ações de confirmação | H04; papéis ainda pendentes |
| CRUD de entidade do domínio | sim | criar e atualizar registros de perda e achado | A01, A02 e A03 |
| Auditoria/logs | talvez | registrar alterações e devolução | H04; necessidade a validar |
| Alertas/ocorrências | sim | avisar sobre possível correspondência e próxima ação | RC03 |
| Ajuda/documentação | sim | orientar dados mínimos e encaminhamento | H02 e RC05 |

> **Atenção:** “login + dashboard + CRUD” não é uma solução universal. Cada padrão deve surgir de uma tarefa real.

---

# 9. Benefícios e ações iniciais

## 9.1 Qual benefício concreto o projeto de IHC pretende oferecer?

| Benefício esperado | Problema/necessidade | Usuário | Status/evidência |
|---|---|---|---|
| reduzir a dispersão e a repetição da busca | informações de perda e achado podem ficar separadas ou incompletas | P01 | H — precisa ser validada com participantes |
| orientar o encaminhamento do achado | P02 pode não saber o próximo passo | P02 | H — precisa ser validada com participantes |
| apoiar a confirmação e a devolução | relatos podem ser semelhantes sem comprovar propriedade | P01, P02 e P03 | H — padrões observados nos concorrentes |

## 9.2 Que ações o usuário deverá conseguir realizar?

| ID | O usuário precisa conseguir... | Para alcançar... | Prioridade inicial |
|---|---|---|---|
| F01 | registrar uma perda | ampliar e organizar a busca | alta |
| F02 | registrar um achado | preservar informações e encaminhar o objeto | alta |
| F03 | buscar e comparar possíveis correspondências | localizar um item compatível | alta |
| F04 | fornecer um detalhe reservado | comprovar a propriedade | alta |
| F05 | acompanhar e concluir o caso | entender a próxima ação e registrar a devolução | média |

## 9.3 Tecnologias/restrições já definidas no TCC

A tecnologia aparece **agora**, depois do entendimento do uso.

| Tecnologia/restrição | Por que existe | Possível impacto na interação |
|---|---|---|
| uso prioritário em celular | P01 e P02 podem agir em deslocamento | exige preenchimento curto, leitura clara e tolerância a interrupções |
| privacidade dos dados | a confirmação não deve expor todas as características do item | separar informação pública de informação de verificação |
| processo institucional não confirmado | não há fonte sobre setor, permissões ou guarda | manter P03 e regras administrativas como hipóteses |

---

# 10. Hipóteses e dúvidas prioritárias

| ID | Hipótese/dúvida | Por que importa | Como poderá ser investigada |
|---|---|---|---|
| H01 | informações sobre a perda ficam dispersas em mais de um canal | justifica centralização e acompanhamento | Entregas 3 e 7 |
| H02 | quem encontra não sabe o encaminhamento ou os dados necessários | influencia a tarefa de P02 | Entregas 3 e 7 |
| H03 | categoria, local, período e características ajudam a comparar registros | define dados comuns de perda e achado | Entregas 2 e 7 |
| H04 | detalhes não públicos ajudam a confirmar a propriedade | reduz entrega incorreta e orienta privacidade | Entregas 2 e 7 |
| Q01 | existe processo ou responsável oficial na FEI? | evita inventar setor, guarda ou responsabilidade | fonte institucional apropriada |

Registre em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

---

# 11. Síntese da equipe

| Pergunta | Síntese atual |
|---|---|
| Qual é a contribuição central do TCC? | O projeto escolhido organiza informações sobre perda, achado, comparação, confirmação de propriedade e devolução |
| O TCC já previa interface? | Sim. A interface já fazia parte do sistema de achados e perdidos escolhido para o projeto |
| Quem é o usuário prioritário de IHC? | P01 — estudante que perdeu um item |
| O que ele precisa alcançar? | localizar, confirmar e recuperar o objeto |
| Qual problema/atividade será estudado? | busca, comparação de relatos, confirmação de propriedade e devolução |
| Como isso acontece hoje? | por procura em locais, conversas e canais que ainda precisam ser investigados |
| Qual é o contexto de uso? | rotina no campus, com mobilidade, pressa e diferentes locais possíveis |
| Que interface/recorte será explorado? | registro, busca, comparação, acompanhamento, confirmação e devolução |
| Como a interface se relaciona ao TCC? | a interface já fazia parte do escopo do projeto escolhido |
| Quais pontos ainda são hipóteses? | H01, H02, H03, H04 e Q01 |

### Delimitação

**Dentro do escopo de IHC:** registrar perdas e achados; buscar e comparar relatos; acompanhar o estado; confirmar propriedade; apoiar a devolução.  
**Fora do escopo de IHC:** definir setor ou regra institucional; substituir segurança ou registro policial; decidir prazos de guarda; implementar o sistema nesta etapa.  
**Dentro do escopo formal do TCC:** o tema do TCC não é utilizado neste trabalho.  
**Interface da disciplina será implementada no TCC?** a interface pertence ao projeto escolhido e será estudada por meio dos artefatos da disciplina.

---

# 12. Como esta entrega alimenta as próximas

- **Entrega 2:** verifica mercado, concorrentes e interfaces profissionais representativas.
- **Entrega 3:** detalha perfis e contexto.
- **Entrega 4:** aprofunda situações problemáticas.
- **Entrega 5:** modela tarefas centrais.
- **Entrega 6:** experimenta alternativas em baixa fidelidade.
- **Entrega 7:** investiga hipóteses com dados.
- **Entrega 8:** define restrições e metas de usabilidade.
- **Entregas 9–11:** transformam o recorte em modelo de interação e protótipo.
- **Entregas 12–14:** avaliam a interface construída na disciplina.

A Entrega 1 é uma **fotografia inicial do conhecimento**. Ela pode e deve ser revisada quando surgirem evidências.

---

# 13. Relação com INOVA e comunicação do projeto

Prepare uma explicação de até três frases:

1. **Problema/atividade humana:** estudantes podem repetir buscas e lidar com relatos dispersos ou incompletos ao perder ou encontrar um objeto.
2. **Contribuição técnica do TCC:** o projeto escolhido organiza perda, achado, comparação, confirmação e devolução por meio de um sistema interativo.
3. **Como uma pessoa poderia utilizar essa contribuição:** registrando informações, consultando possíveis correspondências, comprovando propriedade e acompanhando a devolução.

Essa síntese ajuda a apresentar o projeto para público não especializado sem reduzir seu mérito técnico.

---

# Checklist de qualidade

- [x] Está clara a diferença entre tema do TCC, escopo formal do TCC e escopo de IHC.
- [x] A equipe declarou se o TCC já previa interface.
- [ ] Se não previa, foi derivado um usuário plausível e um objetivo de uso.
- [x] A interface de IHC não foi apresentada como obrigação automática do TCC.
- [x] A contribuição do TCC foi descrita sem começar por tecnologias de implementação.
- [x] Usuários diretos e stakeholders foram diferenciados.
- [x] Foram considerados profissionais que configuram, administram, interpretam ou decidem, quando pertinente.
- [x] Objetivo do usuário não foi confundido com objetivo do projeto.
- [x] Processo/problema atual foi descrito antes da solução.
- [x] Existe situação concreta de uso/problema.
- [x] Contexto físico, social/organizacional, dispositivos e consequências de erro foram considerados.
- [x] Mercado/alternativas existentes foram levantados inicialmente.
- [x] Possibilidades como dashboard, relatório, histórico, filtros e CRUD foram tratadas como hipóteses de solução, não como requisitos automáticos.
- [x] Cada possibilidade de interface tem um objetivo/tarefa que poderia justificá-la.
- [x] Afirmações relevantes estão marcadas `[F]`, `[H]` ou `[?]`.
- [x] Hipóteses prioritárias receberam IDs e foram para a rastreabilidade.
- [x] O recorte de IHC é viável para modelar, prototipar e avaliar no semestre.
- [x] A equipe consegue explicar problema humano → contribuição computacional → forma de uso.
