# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** {{26/11/2026}}  
**Status:** 🟩 concluido  
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Transformar o conhecimento acumulado sobre usuários, tarefas, plataforma e contexto em princípios e **metas de usabilidade verificáveis**, mantendo o caráter iterativo do projeto.



## Delimitação do sistema interativo

| Camada | O que pertence ao projeto | O que será avaliado em IHC |
|---|---|---|
| Contribuição técnica do TCC | Sistema de gerenciamento de achados e perdidos no campus da FEI, incluindo o armazenamento de dados, o processamento das buscas, o gerenciamento dos registros e das solicitações de recuperação de objetos. | Será avaliada a interação do usuário com as funcionalidades disponibilizadas pelo sistema, sem avaliar a implementação técnica, o desempenho computacional ou o funcionamento interno do sistema. |
| Camada de interação da disciplina | Interfaces, formulários, filtros de busca, apresentação dos resultados, fluxos de navegação e acompanhamento das solicitações de recuperação. | Eficácia, eficiência, satisfação, facilidade de aprendizagem, clareza das informações, facilidade de navegação, acessibilidade e prevenção de erros durante a realização das tarefas. |
| Integrações/dados simulados | Registros de objetos encontrados, fotografias, informações sobre local e data, comprovantes de propriedade e estados das solicitações de recuperação. Os dados e as operações de busca, registro e atualização das solicitações serão simulados no protótipo, sem integração com um sistema real. | Capacidade dos usuários de interpretar as informações apresentadas, identificar objetos, compreender o estado das solicitações e reconhecer os próximos passos necessários para a recuperação dos objetos. |


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


### 3.1. Metas qualitativas de usabilidade

| Meta qualitativa | Aplicação ao projeto |
|---|---|
| Facilidade de aprendizagem | Permitir que os usuários compreendam as funcionalidades de busca, registro e recuperação de objetos desde o primeiro contato com a interface. |
| Facilidade de navegação | Permitir que os usuários encontrem as funcionalidades necessárias sem percorrer telas ou etapas desnecessárias. |
| Facilidade de identificação dos objetos | Apresentar fotografias, descrições e filtros por local e data que auxiliem no reconhecimento dos objetos perdidos. |
| Prevenção e recuperação de erros | Permitir que os usuários identifiquem e corrijam informações incorretas durante o registro e a solicitação de recuperação de objetos. |
| Clareza das informações e do estado do sistema | Permitir que os usuários compreendam o andamento das solicitações de recuperação e os próximos passos necessários. |
| Satisfação do usuário | Proporcionar uma experiência de utilização que transmita confiança e segurança durante a busca e a recuperação dos objetos. |


### 3.2 Metas quantitativas
As metas serão avaliadas com estudantes da FEI representativos das personas P01 e P02, priorizando P01. A participação de P03 na tarefa T03 será simulada no protótipo.

| ID | Dimensão | Métrica | Tarefa/escopo | Meta | Como medir | Justificativa |
|---|---|---|---|---|---|---|
| MU01 | eficácia | Taxa de conclusão sem ajuda | T01–T03 | ≥ 80% | Teste observado | Garantir que os usuários consigam concluir corretamente as tarefas propostas sem auxílio. |
| MU02 | eficiência | Tempo mediano de busca e identificação do objeto | T01 | ≤ 3 minutos | Cronômetro | Reduzir o tempo necessário para localizar um objeto entre os registros disponíveis. |
| MU03 | satisfação | Média das avaliações pós-tarefa | T01–T03 | ≥ 3,5 em uma escala de 1 a 5 | Questionário | Avaliar a percepção dos usuários sobre a experiência de utilização do aplicativo. |
| MU04 | taxa de erros | Quantidade média de erros por tarefa | T01–T03 | ≤ 2 erros por tarefa e nenhum erro crítico | Teste observado e registro de erros | Evitar dificuldades durante a interação e erros que possam comprometer a recuperação dos objetos. |
| MU05 | facilidade de aprendizagem | Taxa de conclusão no primeiro contato com a interface, sem treinamento | T01–T03 | ≥ 70% | Observação durante o primeiro uso | Permitir que novos usuários compreendam as funcionalidades sem necessidade de treinamento prévio. |


### 3.3 Priorização das metas
As metas serão utilizadas no planejamento da avaliação (Entrega 12), na identificação de problemas de usabilidade por inspeção heurística (Entrega 13) e na verificação dos resultados obtidos durante a observação dos usuários (Entrega 14).

| Meta | Peso de prioridade | Justificativa |
|---|---:|---|
| MU01 | 30% | A conclusão correta das tarefas é fundamental para que o aplicativo cumpra seu objetivo. |
| MU02 | 20% | Reduzir o tempo e o esforço necessários para localizar objetos perdidos. |
| MU03 | 15% | Proporcionar uma experiência satisfatória e transmitir confiança aos usuários. |
| MU04 | 25% | Prevenir erros que possam comprometer a identificação e a recuperação dos objetos. |
| MU05 | 10% | Facilitar a utilização do aplicativo por novos usuários. |
| **Total** | **100%** | |


## 4. Como o ciclo será iterado

A partir dos resultados coletados, poderão ser revisados os seguintes artefatos:
- Personas e análise de tarefas, caso sejam identificadas necessidades não consideradas inicialmente
- Metas de usabilidade, considerando os resultados das avaliações
- Fluxos de interação e estrutura de navegação do aplicativo
- Prototipos de interface, principalmente nas funcionalidades de busca, registro e recuperação de objetos

As alterações realizadas serão submetidas a novas avaliações, seguindo o caráter iterativo do ciclo de Engenharia de Usabilidade de Mayhew.

## Checklist

- [x] Capacidades e restrições têm impacto de IHC explicitado.
- [x] Está claro o limite entre contribuição técnica do TCC e camada interativa da disciplina.
- [x] Resultados/processamento simulados no protótipo foram explicitados.
- [x] Metas de usabilidade avaliam a interação, não substituem métricas técnicas do TCC.
- [x] Normas/princípios estão contextualizados, não apenas copiados.
- [x] Metas quantitativas são mensuráveis e associadas a tarefas/público.
- [x] Eficácia, eficiência e satisfação são consideradas quando pertinentes.
- [x] Metas poderão ser verificadas nas Entregas 12–14.
