# Entrega 9 — Modelo conceitual e design centrado na comunicação

**Data:** {{dd/mm/aaaa}}  
**Status:** ⬜ não iniciada  
**Responsabilidade:** soluções individuais, com consolidação da equipe para mapa de objetivos e esquema de signos.

## Objetivo da atividade

Passar do cenário de problema para uma concepção da interação, explicitando objetivos, tópicos de conversa, falas e signos que a interface deverá comunicar/manipular.

## Transformando resultados técnicos em conceitos compreensíveis

Em TCCs algorítmicos ou orientados a dados, esta entrega deve evitar que a interface exponha apenas estruturas internas do código. Identifique os **conceitos e signos que fazem sentido para o usuário**.

Exemplos:

- `query plan`, custo estimado, recomendação e impacto para um DBA;
- modelo, dataset, versão, execução e métrica para engenheiro de IA;
- período, indicador, grupo, tendência e filtro para gestor/analista;
- alerta, severidade, evidência, responsável e status para analista de segurança.

Se um termo técnico for necessário, modele como será comunicado, explicado e relacionado à tarefa.

Dashboards, relatórios, filtros e CRUDs devem aparecer no modelo conceitual por meio dos **objetivos, signos e conversas** que justificam sua existência.

## 1. Cenários de interação

Para cada cenário de problema, produza uma versão em que a solução já pode ser descrita. **Destaque claramente o texto alterado** em relação ao cenário original.

### CI01 — Informações que não se encontram

**Autor(a):** Karen Natally de Moraes - 221210867
**Origem:** cenário problema C01

Camila (P01) percebe a falta da mochila ao se preparar para sair do campus. Ela lembra de três ambientes visitados, mas não sabe em qual deles estava com a mochila pela última vez.

Lucas (P02) encontra uma mochila em uma área de circulação enquanto vai para outra atividade. **Ele abre o aplicativo de Achados e Perdidos da FEI, clica no botão "Registrar item encontrado", e preenche as informações do achado: Categoria - prédio K, Descrição - "mochila vermelha da Nike", Local: prédio K. Lucas também clica no botão "Tirar foto", e adiciona uma foto da mochila ao registro. Depois de cadastrar o item, Lucas leva a mochila até o setor de achados e perdidos e entrega a Marina**

 **Camila abre o aplicativo de Achados e Perdidos FEI, clica no botão de "Buscar item perdido". Camila digita o prédio K e data de ontem, pois é o ultimo lugar em que se lembra de estar com a mochila. Ela visualiza todos os itens correspondentes a busca, e identifica um item com uma foto da sua mochila. Camila clica no item, e preenche o formulário de recuperação do item, preenche seu nome, seu telefone e uma foto antiga com a mochila. Após algumas horas, Camila recebe uma notificação do aplicativo "Temos novidade sobre sua solicitação". Camila abre o app, e clica em "Minhas solicitações", visualiza o retorno sobre o item solicitado e se dirige ao setor de achados e perdidos para retirar o item.**
 
 **Marina, funcionária do setor de achados e perdidos, é informada pela Camila sobre sua busca, Marina confere a solicitação e compara o comprovante visualmente com o item encontrado. Marina confirma a correspondência e entrega a mochila para Camila.** 

### Diferenças relevantes

| Alteração | Por que foi necessária | Evidência/artefato que justifica |
|---|---|---|
| Registro do item encontrado pelo aplicativo. | Centralizar as informações e evitar a perda de detalhes sobre o achado. | Entrega 5 — GOMS (T02). |
| Inclusão de uma foto do item encontrado. | Facilitar o reconhecimento do objeto pelo proprietário. | Entrega 5 — GOMS (T02). |
| Busca de itens por local e data. | Reduzir a necessidade de procurar presencialmente nos ambientes visitados. | Entrega 4 — Cenário C01; Entrega 5 — HTA (T01). |
| Formulário de recuperação com nome, telefone e comprovante de propriedade. | Auxiliar na identificação do proprietário e evitar devoluções incorretas. | Entrega 5 — CTT (T03). |
| Notificação e acompanhamento da solicitação pelo aplicativo. | Permitir que o usuário acompanhe o resultado da análise sem precisar se deslocar até o setor. | Entrega 5 — CTT (T03), que prevê o retorno da análise. A notificação específica precisa de evidência complementar. |
| Conferência do comprovante por Marina. | Verificar a correspondência entre o item encontrado e a solicitação de recuperação. | Entrega 5 — CTT (T03). |

## 2. Design centrado na comunicação

**Nome do cenário:** CI01 — Informações que não se encontram

| Tópico > subtópico | Falas e signos envolvidos | Intenção/efeito esperado |
|---|---|---|
| Registrar item encontrado | U: Encontrei um objeto e quero registrá-lo. / D: Registrar item encontrado. | Permitir o registro de objetos encontrados no campus. |
| > Preencher informações | D: Categoria, descrição, local, data, contato e observações. / U: Informa os dados do item encontrado. | Centralizar as informações sobre o achado. |
| > Adicionar foto | D: Tirar foto. / U: Fotografa a mochila. | Facilitar a identificação visual do item. |
| Buscar item perdido | U: Quero encontrar minha mochila. / D: Buscar item perdido. | Permitir a localização de objetos perdidos. |
| > Informar local e data | D: Local e data. / U: Informa o prédio K e a data de ontem. | Restringir os resultados da busca. |
| > Visualizar resultados | D: Resultados da busca. / U: Identifica a mochila pela foto. | Facilitar o reconhecimento do item perdido. |
| Solicitar recuperação | U: Quero recuperar este item. / D: Formulário de recuperação do item. | Permitir que o usuário solicite a devolução. |
| > Preencher formulário | D: Nome, telefone e comprovante de propriedade. / U: Preenche os dados e anexa uma foto antiga com a mochila. | Fornecer informações para verificar a propriedade do item. |
| Analisar solicitação | U: Marina confere a solicitação e o comprovante. / D: Informações da solicitação de recuperação. | Verificar a correspondência e evitar devoluções incorretas. |
| Acompanhar solicitação | D: Temos novidade sobre sua solicitação. / U: Acessa Minhas solicitações. | Informar o usuário sobre o andamento da recuperação. |
| > Consultar retorno | D: Resultado da análise da solicitação. / U: Consulta o retorno e dirige-se ao setor de achados e perdidos. | Orientar o usuário para a recuperação do item. |

**Convenção:** `U` = usuário; `D` = preposto do designer/sistema, conforme a abordagem de Engenharia Semiótica adotada na disciplina.

## 3. Mapa de objetivos

Cada integrante apresenta seu mapa e a equipe cria um **mapa consolidado**, eliminando duplicidades e resolvendo conflitos de nomenclatura.

![Mapa consolidado](../assets/09_modelo_conceitual/mapa_objetivos.svg)

### Dicionário de objetivos

| ID | Objetivo | Persona(s) | Cenário(s) | Prioridade |
|---|---|---|---|---|
| O01 | {{...}} | {{P01}} | {{CI01}} | {{...}} |

## 4. Esquema conceitual de signos

Consolide as informações em **uma tabela única**.

| Grupo | Signo | Origem | Observações/semantica | Tipo de conteudo | Restrição | Valor padrão | Prevenção | Recuperação |
|---|---|---|---|---|---|---|---|---|
| Item (I) | Registrar item (I) | dominio | Item encontrado | Entidade | — | — | Conferir informações antes do registro | Permitir edição do registro |
| Item (I) | descrição | dominio | Caracteristicas do item encontrado | Texto | Não nulo | — | Indicar preenchimento obrigatorio | Permitir correção da descrição |
| Item (I) | local | dominio | Local onde o item foi encontrado | Texto | Local valido no campus | — | Disponibilizar lista de locais | Permitir alteração do local |
| Item (I) | data | dominio | Data em que o item foi encontrado | Data | Não pode ser futura | Data atual | Impedir seleção de datas futuras | Permitir alteração da data |
| Item (I) | contato | dominio | Contato de quem encontrou o item | Texto | Formato valido | — | Validar formato do contato | Permitir correção do contato |
| Item (I) | observações | dominio | Informações complementares sobre o item | Texto | Opcional | — | — | Permitir edição |
| Item (I) | foto | dominio | Foto do item encontrado | Imagem | Formato de imagem valido; opcional | — | Exibir previa da foto | Permitir substituir ou remover a foto |
| Item (I) | Usuario (U) U.[nome, contato, telefone] | aplicação | Usuario que encontrou o item | Entidade | Usuario cadastrado | Usuario autenticado | Vincular ao usuario autenticado | Permitir correção dos dados de contato |
| Formulario (F) | Formulario de recuperação (F) | aplicação | Formulario de solicitação de recuperação do item | Entidade | Campos obrigatorios preenchidos | — | Validar campos antes do envio | Permitir correção dos campos |
| Formulario (F) | comprovante de propriedade | aplicação | Foto que o usuario anexa no formulario de recuperação | Imagem | Não nulo | — | Validar arquivo e exibir previa | Permitir substituir o comprovante |
| Formulario (F) | notificação da solicitação | aplicação | Mensagem recebida pelo usuario informando novidades sobre a solicitação | Entidade | Vinculada a uma solicitação | — | Associar a notificação a solicitação correta | Permitir consultar o retorno em Minhas solicitações |
| Formulario (F) | Usuario (U) U.[nome, contato, telefone] | aplicação | Usuario que recupera o item | Entidade | Usuario cadastrado | Usuario autenticado | Identificar o usuario solicitante | Permitir correção dos dados |
| Usuario (U) | Usuario (U) | aplicação | Usuario do aplicativo | Entidade | — | — | Validar dados de identificação | Permitir atualização dos dados |
| Usuario (U) | nome do usuario | dominio | Nome preenchido em F | Texto | Não nulo | — | Indicar preenchimento obrigatorio | Permitir correção do nome |
| Usuario (U) | contato do usuario | dominio | Contato do usuario preenchido em F | Texto | Formato valido | — | Validar formato do contato | Permitir correção do contato |
| Usuario (U) | telefone do usuario | dominio | Telefone adicionado pelo usuario no formulario de recuperação | Texto | Telefone valido e não nulo | — | Utilizar mascara de telefone | Permitir correção do telefone |

### Regras para os signos

- Use o vocabulário do domínio do usuário.
- Evite duplicar o mesmo conceito com nomes diferentes.
- Diferencie informação fornecida pelo usuário, produzida pelo sistema e derivada do domínio.
- Registre prevenção e recuperação apenas quando fizer sentido; explique as siglas usadas.

## Síntese

Quais objetivos/tópicos/signos deverão necessariamente aparecer nos diagramas MoLIC?

## Checklist

- [ ] Cenários de interação mostram alterações em relação aos cenários de problema.
- [ ] Cada solução individual identifica autor e cenário de origem.
- [ ] Tópicos/falas/signos são coerentes com objetivos do usuário.
- [ ] Mapas individuais foram consolidados.
- [ ] O esquema de signos está em uma tabela única e sem duplicações conceituais.
- [ ] Nomes de objetivos/signos serão reutilizados na Entrega 10.
- [ ] Em TCC técnico, signos representam conceitos do domínio compreensíveis ao usuário, não apenas variáveis/estruturas internas.
- [ ] Padrões como dashboard, relatório, filtros, administração e CRUD possuem objetivos e signos correspondentes.
- [ ] A interface comunica não só o resultado técnico, mas também seu significado para a tarefa.
