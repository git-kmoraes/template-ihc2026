# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** {{dd/mm/aaaa}}  
**Status:** ⬜ não iniciada  
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Transformar o conhecimento acumulado sobre usuários, tarefas, plataforma e contexto em princípios e **metas de usabilidade verificáveis**, mantendo o caráter iterativo do projeto.



## Delimitação do sistema interativo

| Camada | O que pertence ao projeto | O que será avaliado em IHC |
|---|---|---|
| Contribuição técnica do TCC | Sistema de gerenciamento de achados e perdidos no campus da FEI, permitindo o registro, a busca, a identificação e a recuperação de objetos. | Eficácia e eficiência do sistema no atendimento às necessidades dos usuários, considerando a taxa de conclusão das tarefas, o tempo de execução e a necessidade de auxílio para localizar, registrar ou solicitar a recuperação de objetos. |
| Camada de interação da disciplina | Interfaces, formulários, filtros de busca, apresentação dos resultados, fluxos de navegação e acompanhamento das solicitações de recuperação. | Facilidade de aprendizagem, clareza das informações, facilidade de navegação, acessibilidade, prevenção de erros e satisfação dos usuários. Serão considerados o número de erros, as dificuldades encontradas e a percepção dos participantes durante os testes de usabilidade. |
| Integrações/dados simulados | Registros de objetos encontrados, fotografias, informações sobre local e data, comprovantes de propriedade e estados das solicitações de recuperação, representados no protótipo. | Capacidade dos usuários de interpretar corretamente as informações apresentadas, identificar objetos, compreender o estado das solicitações e reconhecer os próximos passos necessários para a recuperação, considerando erros de interpretação e dúvidas durante a interação. |


## 1. Características da plataforma

| Característica | Descrição | Consequência para IHC |
|---|---|---|
| Software | Aplicativo móvel de achados e perdidos destinado à comunidade acadêmica da FEI. A solução será representada por um protótipo interativo. | Garantir consistência entre as telas e os fluxos de registro, busca e recuperação de objetos, avaliando a facilidade de aprendizagem e navegação. |
| Hardware/dispositivos | Smartphones com diferentes dimensões de tela, resolução, interação por toque e disponibilidade de câmera. | Garantir legibilidade, facilidade de seleção dos elementos interativos e facilidade de inclusão e visualização de fotografias, observando erros e dificuldades durante a interação. |
| Capacidades | Registro de objetos encontrados, inclusão de fotografias, busca por local e data, comparação de informações, solicitação de recuperação e acompanhamento das solicitações. | Organizar as funcionalidades de acordo com os objetivos dos usuários, avaliando a taxa de sucesso, o tempo de execução e o esforço necessário para concluir as tarefas. |
| Restrições | Espaço reduzido de tela, dependência de conexão com a internet, interrupções e informações incompletas sobre os objetos perdidos. | Reduzir a carga cognitiva por meio de formulários objetivos, priorização das informações e possibilidade de corrigir dados e retomar tarefas interrompidas. |
| Conectividade/latência | A solução proposta depende de conexão com a internet para consultar registros, enviar fotografias e atualizar solicitações, podendo apresentar variações de conectividade durante o uso no campus. | Fornecer feedback durante as operações, comunicar falhas de conexão e orientar a recuperação de erros, avaliando se o usuário compreende a situação e consegue prosseguir. |
| Segurança/privacidade | Manipulação de informações pessoais, fotografias de objetos e informações utilizadas para comprovar sua propriedade. | Apresentar informações claras sobre o compartilhamento de dados, limitar a exposição de informações sensíveis e prevenir erros que possam resultar na devolução de objetos a pessoas indevidas. |
| Volume de dados/histórico | Acúmulo de registros de objetos encontrados e solicitações de recuperação ao longo do tempo. | Disponibilizar mecanismos de busca e filtros por local e data, avaliando o tempo e a facilidade com que o usuário identifica um objeto entre diferentes resultados. |
| Tempo de processamento | Operações de busca, envio de fotografias, registro e atualização das solicitações, além do tempo necessário para a análise da propriedade do objeto. | Apresentar indicadores de processamento, confirmações de conclusão e estados das solicitações, avaliando se o usuário compreende o estado do sistema e evita operações duplicadas. |
| Papéis/permissões | Estudante que perdeu um objeto (P01), estudante que encontrou um objeto (P02) e pessoa que auxilia na análise e devolução dos objetos (P03, papel hipotético). | Adequar as funcionalidades e os fluxos aos objetivos de cada perfil, garantindo clareza sobre as ações disponíveis e prevenindo operações inadequadas ou não autorizadas. |



## 2. Princípios gerais do projeto

| Princípio/norma | Aplicabilidade ao contexto | Decisão/requisito decorrente | Fonte |
|---|---|---|---|
| Contexto de uso | Os usuários possuem diferentes objetivos: localizar um objeto perdido, registrar um objeto encontrado ou auxiliar na sua devolução. | Priorizar o fluxo de busca e recuperação de objetos, considerando as necessidades da persona P01 e diferenciando as ações disponíveis para cada perfil. | Entregas 1/3 |
| LGPD, se aplicável | O processo de recuperação de objetos pode envolver dados pessoais e comprovantes de propriedade. | Solicitar apenas as informações necessárias, esclarecer a finalidade da coleta e restringir a exposição de dados pessoais e comprovantes de propriedade. | [Lei nº 13.709/2018](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709compilado.htm) |
| Acessibilidade | A identificação dos objetos e dos estados das solicitações não deve depender exclusivamente de imagens, cores ou ícones. | Utilizar descrições textuais dos objetos, contraste adequado, textos legíveis e identificação clara dos elementos interativos. | [WCAG 2.2](https://www.w3.org/TR/WCAG22/) |
| Reconhecimento em vez de memorização | O usuário pode não se lembrar de todas as características do objeto perdido, da data ou do local da perda. | Permitir buscas com informações parciais e apresentar fotografias e descrições que auxiliem na identificação dos objetos. | [6ª heurística de Nielsen](https://www.nngroup.com/articles/ten-usability-heuristics/) |
| Visibilidade do estado do sistema | O usuário precisa acompanhar o andamento da sua solicitação de recuperação. | Apresentar confirmações de envio, estados das solicitações e orientações sobre os próximos passos para a recuperação do objeto. | [1ª heurística de Nielsen](https://www.nngroup.com/articles/ten-usability-heuristics/) |


## 3. Metas de usabilidade

Usabilidade deve ser discutida **no contexto de uso**. Metas quantitativas devem dizer o que será medido, em qual tarefa, com qual população e qual limite será considerado aceitável.

### 3.1 Metas qualitativas

| Meta | Para quem/tarefa | Evidência desejada | Justificativa |
|---|---|---|---|
| {{ex.: compreensão clara da diferença entre X e Y}} | {{...}} | {{fala/observação}} | {{...}} |

### 3.2 Metas quantitativas

| ID | Dimensão | Métrica | Tarefa/escopo | Meta | Como medir | Justificativa |
|---|---|---|---|---|---|---|
| MU01 | eficácia | taxa de conclusão sem ajuda | T01 | ≥ {{x}}% | teste observado | {{...}} |
| MU02 | eficiência | tempo mediano | T02 | ≤ {{tempo}} | cronômetro/log | {{...}} |
| MU03 | satisfação | escala pós-tarefa | T01–T03 | ≥ {{valor}} | questionário | {{...}} |

### 3.3 Priorização das metas (se exigida na disciplina)

Se o professor solicitar porcentagens que somem 100%, trate-as como **peso de prioridade**, não como métrica de usabilidade.

| Meta | Peso de prioridade | Justificativa |
|---|---:|---|
| MU01 | {{...}}% | {{...}} |
| **Total** | **100%** | |

## 4. Como o ciclo será iterado

Explique que artefatos serão revisitados após protótipos e avaliações.

## Checklist

- [ ] Capacidades e restrições têm impacto de IHC explicitado.
- [ ] Está claro o limite entre contribuição técnica do TCC e camada interativa da disciplina.
- [ ] Resultados/processamento simulados no protótipo foram explicitados.
- [ ] Metas de usabilidade avaliam a interação, não substituem métricas técnicas do TCC.
- [ ] Normas/princípios estão contextualizados, não apenas copiados.
- [ ] Metas quantitativas são mensuráveis e associadas a tarefas/público.
- [ ] Eficácia, eficiência e satisfação são consideradas quando pertinentes.
- [ ] Metas poderão ser verificadas nas Entregas 12–14.
