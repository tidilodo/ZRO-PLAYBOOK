# Skill — Product Context Engineering

# 05 — Backlog

Versão: 1.0

---

# Objetivo

A etapa de Backlog transforma a arquitetura e o contexto do produto em um plano de execução incremental.

O backlog não é apenas uma lista de tarefas.

Ele representa a estratégia de evolução do produto.

Cada item deve existir porque aproxima o produto da visão definida anteriormente.

---

# Princípio Fundamental

> O backlog é a representação operacional da visão do produto.

Nenhuma tarefa deve existir sem contribuir para um objetivo maior.

Se uma tarefa não pode ser relacionada à visão do produto, ela não pertence ao backlog.

---

# Quando utilizar

Esta etapa inicia após:

- Discovery concluído;
- Vision definida;
- Architecture documentada;
- Context organizado.

Somente então o projeto possui informações suficientes para ser dividido em entregas.

---

# Resultado Esperado

Ao final desta etapa devemos possuir:

- backlog organizado;
- prioridades definidas;
- entregas independentes;
- evolução incremental;
- visão clara das próximas fases do produto.

---

# Processo

## Etapa 1 — Identificar Épicos

Os Épicos representam grandes capacidades do produto.

Exemplos:

- Gestão de Usuários
- CRM
- Pagamentos
- Inteligência Artificial
- Relatórios

Cada épico deve representar uma área significativa do sistema.

---

## Etapa 2 — Criar Features

Cada épico deve ser dividido em funcionalidades.

Exemplo:

Épico:

CRM

Features:

- Cadastro de Clientes
- Histórico
- Pipeline
- Agenda

---

## Etapa 3 — Criar User Stories

Cada feature deve gerar pequenas histórias independentes.

Formato recomendado:

> Como **[tipo de usuário]**, quero **[objetivo]**, para **[benefício]**.

Exemplo:

Como terapeuta,
quero registrar um novo cliente,
para acompanhar sua evolução.

---

## Etapa 4 — Criar Tarefas Técnicas

Somente agora criar tarefas técnicas.

Exemplos:

- criar endpoint
- criar tabela
- implementar autenticação
- integrar API
- criar testes

Tarefas técnicas nunca devem existir diretamente no backlog principal.

Elas pertencem às User Stories.

---

## Etapa 5 — Definir Prioridades

Priorizar utilizando valor entregue.

Perguntar:

Esta entrega gera valor imediato?

Reduz riscos?

Valida hipóteses?

Acelera próximas etapas?

---

## Etapa 6 — Organizar Releases

Agrupar funcionalidades em versões.

Exemplo:

MVP

↓

Versão 1.1

↓

Versão 1.2

↓

Versão 2.0

Cada release deve entregar valor completo.

Nunca apenas funcionalidades isoladas.

---

# Estrutura Recomendada

```
Produto

↓

Épicos

↓

Features

↓

User Stories

↓

Tarefas Técnicas
```

Nunca inverter esta ordem.

---

# Critérios de Priorização

Toda prioridade deve considerar:

Valor para o usuário.

Impacto no negócio.

Dependências.

Complexidade.

Risco.

Aprendizado gerado.

---

# O que evitar

Evite:

- backlog composto apenas por tarefas técnicas;
- funcionalidades sem objetivo;
- tarefas gigantes;
- backlog desorganizado;
- prioridades indefinidas.

---

# Critérios para Encerramento

Esta etapa termina quando:

- [ ] Todos os épicos foram identificados.
- [ ] Cada épico possui features.
- [ ] Todas as features possuem User Stories.
- [ ] As User Stories possuem tarefas técnicas.
- [ ] Existe priorização.
- [ ] Existe planejamento de releases.

---

# Entregáveis

Ao concluir esta etapa devem existir:

- Product Backlog
- Epic Map
- Feature Map
- User Story Map
- Release Plan

Esses documentos servirão como entrada para a implementação.

---

# Relação com Inteligência Artificial

A IA nunca deve implementar diretamente um Épico.

Toda implementação deve partir de uma User Story específica.

Antes de iniciar qualquer tarefa a IA deve compreender:

- a User Story;
- o objetivo da Feature;
- o contexto do Épico;
- a visão do produto.

Implementar sem contexto aumenta o risco de inconsistências.

---

# Próxima Etapa

Com o backlog estruturado, iniciamos a implementação incremental.

Consulte:

**06_Implementation**

---

# Regra Final

Um bom backlog não organiza tarefas.

Ele organiza a evolução do produto.

Cada item deve representar um pequeno passo em direção à visão construída durante as etapas anteriores.
