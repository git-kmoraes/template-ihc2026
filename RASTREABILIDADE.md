# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

**Tema adotado no projeto de IHC:** Achados e perdidos no campus da FEI.

**Recorte do projeto:** apoiar o registro de perdas e achados, a comparação entre relatos, a confirmação de propriedade e a devolução do objeto.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | Projeto escolhido: **sistema de achados e perdidos no campus da FEI** | README e Entrega 1 | definido |
| Resultado técnico esperado | Sistema interativo para registrar perdas e achados, comparar relatos, confirmar a propriedade e apoiar a devolução | Entrega 1, seções 0.4, 1.1 e 1.3 | definido |
| O TCC previa interface? | Sim. A interface já fazia parte do escopo do projeto escolhido | README e Entrega 1, seção 0.5 | definido |
| Capacidade/contribuição central | organizar informações de perda, achado, comparação, confirmação e devolução | Entrega 1 | definido |
| Possíveis beneficiários/stakeholders | estudantes, comunidade acadêmica e instituição | hipóteses H01, H02 e Q01 | H / ? |
| Usuário escolhido para IHC | P01 — Camila, estudante que perdeu um item; P02 — Lucas, estudante que encontrou um item; P03 — Marina, pessoa que apoia a devolução | três papéis com objetivos diferentes no mesmo processo; P03 permanece hipotética | H |
| Objetivo principal do usuário | P01: localizar e recuperar o item; P02: registrar e encaminhar o achado; P03: comparar relatos, confirmar a propriedade e concluir a devolução | Entrega 1, seção 3; Entrega 3 | H |
| Contexto de uso adotado | rotina no campus, com mobilidade e diferentes locais possíveis | Entrega 1, seção 5 | H |
| Interface/recorte de IHC | registro, busca, comparação, acompanhamento, confirmação e devolução | atividades A01, A02 e A03 | proposta |
| Relação com o TCC | o tema do TCC não é utilizado; o trabalho parte de um projeto escolhido que já previa uma interface | README e Entrega 1 | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | informações sobre a perda ficam dispersas em mais de um canal | H | justifica centralização e acompanhamento | Entregas 3 e 7 | cenário C01; coleta PENDENTE | aberta | validar canais e repetições |
| H02 | quem encontra não sabe o encaminhamento ou os dados necessários | H | influencia a tarefa de P02 | Entregas 3 e 7 | cenário C01; coleta PENDENTE | aberta | validar instruções e campos mínimos |
| H03 | categoria, local, período e características ajudam a comparar registros | H | define dados comuns de perda e achado | Entregas 2 e 7 | concorrentes C01, C02 e C03 | refinada | usar como base inicial e validar com participantes |
| H04 | detalhes não públicos ajudam a confirmar a propriedade | H | reduz entrega incorreta | Entregas 2 e 7 | concorrentes C01 e C03 | refinada | separar informação pública de confirmação |
| Q01 | existe processo ou responsável oficial na FEI? | ? | evita inventar setor, guarda ou responsabilidade | fonte institucional apropriada | PENDENTE | aberta | P03 permanece papel hipotético |

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | organizar relatos e possíveis correspondências | localizar e recuperar o item com menos repetição | P01 | C01 | T01 | [HTA](assets/05_tarefas/hta_t01.svg) | PENDENTE | PENDENTE | PENDENTE | — | PENDENTE | protótipo e avaliação pendentes |
| R02 | registrar achados com dados comuns | registrar e encaminhar o achado com pouco esforço | P02 | C01 | T02 | [GOMS](assets/05_tarefas/goms_t02.svg) | PENDENTE | PENDENTE | PENDENTE | — | PENDENTE | protótipo e avaliação pendentes |
| R03 | comparar relatos e solicitar complemento | verificar uma possível correspondência | P03 | C01 | T03 | [CTT](assets/05_tarefas/ctt_t03.svg) | PENDENTE | PENDENTE | PENDENTE | — | PENDENTE | confirmar processo institucional |
| R04 | separar correspondência de comprovação | confirmar propriedade e concluir devolução | P01, P02 e P03 | C01 | T01 e T03 | [HTA](assets/05_tarefas/hta_t01.svg) e [CTT](assets/05_tarefas/ctt_t03.svg) | PENDENTE | PENDENTE | PENDENTE | — | PENDENTE | regras e teste pendentes |

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| F01 | formulário de registro de perda | registrar uma perda | descrição, categoria, local e período aproximado | H01 e RC01; necessidade ainda a validar | C01 e T01 |
| F02 | formulário de registro de achado | registrar um achado | descrição, local, data e forma de encaminhamento | H02, RC02 e Q01; processo ainda a validar | C01, T02 e T03 |
| F03 | busca e comparação de relatos | buscar e comparar possíveis correspondências | filtros, resultados compatíveis e detalhes para comparação | H03 e RC03; necessidade ainda a validar | C01, T01 e T03 |

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| 23/09/2026 | adotado o recorte de achados e perdidos no campus | permite estudar objetivos e tarefas de três papéis relacionados | itens 1 a 5 | Karen Natally de Moraes |
| 23/09/2026 | P03 mantida como papel hipotético | não existe confirmação de setor ou processo institucional | P03, C01 e T03 | Karen Natally de Moraes |

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
