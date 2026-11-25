# Entrega 6 — Prototipação em papel

**Data:** {{dd/mm/aaaa}}  
**Status:** não iniciada  
**Responsabilidade:** 1 solução integrada por equipe

## Objetivo da atividade

Externalizar rapidamente ideias de interação em baixa fidelidade para explorar alternativas antes de investir em detalhes visuais. O valor da atividade está no **ciclo construir → simular → observar → revisar**, não na beleza do desenho.

## 1. Escopo do protótipo

**Personas:** P01

**Cenários/tarefas cobertos:** C01/T01

**Objetivos principais:** permitir que o usuario
busque um item perdido, analise os resultados
retornados e solicite a recuperação do item.

## 1.1 Família de interface escolhida

Interface mobile no formato de aplicativo,
com mecanismos de busca, filtros e visualização
dos detalhes dos itens encontrados.

## 2. Fluxos escolhidos

| Fluxo | Tarefa/objetivo | Por que foi priorizado |
|---|---|---|
| PF01 | buscar e recuperar item perdido | representa um dos principais objetivos do aplicativo |

## 3. Telas e estados

- P01: tela inicial do aplicativo, permite ao usuario escolher a funcionalidade desejada
- P02: tela de busca e visualização dos itens retornados
- P03: tela de detalhes do item encontrado, com opção de solicitar sua recuperação

A navegação entre as telas é representada
através de setas que indicam o resultado
das ações realizadas pelo usuario.

## 3. Telas e estados

- Numere as telas/estados (`P01`, `P02`...).
- Indique controles que mudam o estado.
- Mostre pelo menos caminhos principais e estados de erro/retorno relevantes.

![Protótipo](../assets/06_prototipos/prototipo)

## 4. Simulação / walkthrough

| Observação | Tela/ação | Evidência | Consequência para o design |
|---|---|---|---|
| facilidade em identificar a funcionalidade de busca | P01 | botão Buscar item perdido identificado na tela inicial | manter organização da tela inicial |
| dificuldade em retornar para alterar os filtros | P03 | ausência de botão de voltar | adicionar opção de retorno |
| dúvida sobre como proceder após reconhecer o objeto | P03 | ausência de indicação de como solicitar a recuperação | adicionar botão de solicitação |

## 5. Alterações após a simulação

| Antes | Problema | Depois | Justificativa |
|---|---|---|---|
| tela de resultados sem botão de voltar | dificuldade em alterar informações da busca | adicionar botão de voltar | facilitar nova busca |
| informações do item sem opção de recuperação | usuario não sabe como proceder | adicionar botão Solicitar recuperação | orientar usuario sobre a próxima ação |

## Checklist

## Checklist

- [x] O protótipo cobre tarefas relevantes da Entrega 5.
- [x] Cada tela/estado pode ser justificado por uma tarefa, decisão ou informação necessária.
- [x] O projeto não criou dashboard/CRUD/login apenas para parecer “completo”.
- [x] Telas/estados estão numerados e navegáveis na documentação.
- [x] Há pelo menos uma simulação/walkthrough documentado.
- [x] Críticas não foram apenas listadas: geraram decisão de revisão.
- [x] O protótipo continua em baixa fidelidade; detalhes visuais não mascararam problemas de fluxo.
