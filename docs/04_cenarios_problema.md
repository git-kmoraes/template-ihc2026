# Entrega 4 — Cenários de análise/problema

**Data:** 23/09/2026  
**Status:** 🟩 concluída  
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Descrever situações atuais em que o usuário tenta alcançar um objetivo e encontra dificuldades. O cenário de análise/problema deve tornar visível **o contexto, os atores, as ações e as rupturas**, sem antecipar a interface que será projetada.

> **Regra central:** cenário de problema é a “história do problema”. Se o texto já diz “o sistema mostra”, “o aplicativo resolve” ou descreve botões/telas futuras, provavelmente está misturando problema com solução.

Sempre que possível, o cenário deve aprofundar uma **situação concreta já registrada na Entrega 1**.

### Quando o TCC não possuía interface

O cenário continua sendo uma história de **problema/atividade humana**, não uma história do futuro sistema. Descreva como o profissional realiza hoje uma atividade semelhante ou como lida atualmente com dados, resultados, configurações, logs, decisões e limitações que o tema do TCC pretende apoiar.

Exemplo: em vez de “o DBA abre o novo dashboard e executa o algoritmo”, descreva “o DBA precisa investigar uma consulta lenta, reúne informações em ferramentas distintas, compara planos manualmente e tem dificuldade para estimar o impacto de uma mudança”.

A interface da disciplina aparecerá somente depois, nos cenários de interação.

Se o integrante escolher um novo problema/situação, explique por que ele passou a ser relevante e indique a evidência que motivou sua inclusão.

## Cenário C01 — Informações que não se encontram

**Autor(a):** Karen Natally de Moraes — 221210867  
**Persona(s) relacionada(s):** P01, P02 e P03  
**Necessidade relacionada:** R01, R02, R03 e R04  
**Situação concreta da Entrega 1 relacionada:** seção 4.5  
**Hipóteses ainda presentes:** H01, H02, H03, H04 e Q01

### 1. Cenário inicial

[H] Camila (P01) percebe que perdeu a mochila depois de passar por diferentes ambientes do campus. Ela volta aos lugares de que se lembra, pergunta a colegas e descreve o objeto mais de uma vez. Lucas (P02) encontra uma mochila, mas está a caminho de outra atividade e não sabe onde deve entregá-la. Ele pergunta a pessoas próximas e guarda o objeto temporariamente.

Mais tarde, Marina (P03), que representa uma pessoa hipotética de apoio à devolução, recebe informações sobre a perda e o achado. O relato de Camila destaca a aparência da mochila, enquanto o de Lucas registra apenas o local aproximado. Marina precisa fazer novas perguntas para entender se os relatos tratam do mesmo item. Enquanto isso, Camila não sabe que existe uma possível correspondência, Lucas continua responsável pela mochila e Marina corre o risco de confirmar a entrega com dados insuficientes.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | em que momento Camila percebe a perda e quais locais consegue lembrar? | define o período e a área inicial da busca | entrevista ou questionário com estudantes |
| Q2 | quais canais Camila e Lucas usariam primeiro? | revela onde ocorre a dispersão de informações | entrevista e observação de relatos |
| Q3 | quais dados Lucas consegue registrar sem atrasar sua rotina? | define o mínimo do registro de achado | teste exploratório com estudantes |
| Q4 | quais características podem comprovar que Camila é a dona? | reduz o risco de entrega incorreta | consulta a processos semelhantes e validação institucional |
| Q5 | quem pode assumir o papel de Marina e onde o item fica guardado? | evita inventar setor ou responsabilidade | confirmação com fonte institucional |

### 3. Cenário refinado

Reescreva o cenário incorporando as respostas. Marque o conteúdo novo de forma consistente (por exemplo, `**[NOVO: ...]**`).

[H] Camila (P01) percebe a falta da mochila ao se preparar para sair do campus. **[NOVO — H] Ela lembra de três ambientes visitados, mas não sabe em qual deles estava com a mochila pela última vez.** Primeiro, retorna ao local mais recente. Depois, pergunta a colegas e divulga uma descrição em um canal informal. **[NOVO — H] Cada tentativa gera uma versão um pouco diferente do período e do local da perda.**

Lucas (P02) encontra uma mochila em uma área de circulação enquanto vai para outra atividade. **[NOVO — H] Ele consegue registrar o local aproximado, o horário e uma foto, mas não quer publicar características que poderiam facilitar uma falsa reivindicação.** Como não sabe qual é o encaminhamento correto, pergunta a pessoas próximas e permanece com o objeto.

Marina (P03) representa, apenas como hipótese, a pessoa que participa do recebimento ou da devolução. **[NOVO — H] Ela recebe os dois relatos em momentos diferentes e precisa comparar categoria, local, período e características.** Como alguns dados são incompletos, solicita a Camila um detalhe que não foi divulgado. **[NOVO — H] Até receber a resposta, mantém o caso como possível correspondência, não como item confirmado.**

Camila demora a saber que pode existir um achado, Lucas não sabe quando deixa de ser responsável pela mochila e Marina precisa reconstruir o histórico das conversas. **[NOVO — ?] Continua sem resposta quem assumiria esse papel na FEI e quais regras seriam usadas para guarda e entrega.**

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | P01 perdeu; P02 encontrou; P03 media a comparação e a entrega |
| Objetivo(s) | recuperar, encaminhar e devolver com segurança |
| Contexto | circulação pelo campus, mudança de ambiente, pressa e percepção tardia |
| Recursos/informações | descrição, categoria, local, período, foto, contato e característica não pública |
| Ações | refazer caminho, perguntar, registrar, comparar, complementar e confirmar |
| Problemas/rupturas | relatos dispersos, dados diferentes, responsabilidade incerta e possível correspondência sem confirmação |
| Consequências | demora, retrabalho, risco de entrega incorreta e exposição de detalhes |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

As tarefas prioritárias são T01, buscar e recuperar um item perdido; T02, registrar e encaminhar um item encontrado; e T03, comparar relatos e concluir a devolução. Antes de definir regras institucionais, é necessário investigar Q01. Também será preciso validar campos mínimos, canais usados e critérios de propriedade.

> Repita para C02, C03... com autoria individual.

## Checklist

- [x] Há um cenário completo por integrante.
- [x] Cada cenário tem título, ator, objetivo, contexto e problema.
- [x] O cenário possui origem rastreável na Entrega 1 ou justifica claramente a inclusão de uma nova situação.
- [x] O texto descreve a situação atual, sem antecipar a solução.
- [ ] Para TCC sem interface original, o cenário descreve uma prática humana plausível relacionada à contribuição técnica, e não “a falta de uma tela”.
- [x] Questões de refinamento acrescentam informação nova.
- [x] O refinamento mostra claramente o que foi adicionado/alterado.
- [x] Cenários são diferentes o suficiente para cobrir objetivos/problemas relevantes.
- [x] Cada cenário está ligado a persona/necessidade na matriz de rastreabilidade.
