# Skill — Product Context Engineering

# 04 — Context

Versão: 1.0

---

# Objetivo

A etapa de Context transforma conhecimento em um ativo permanente do projeto.

Seu objetivo é organizar todas as informações necessárias para que qualquer pessoa ou Inteligência Artificial compreenda o produto sem depender de conhecimento implícito.

Contexto reduz retrabalho.

Contexto preserva decisões.

Contexto acelera evolução.

---

# Princípio Fundamental

> Um produto só pode evoluir de forma consistente quando seu contexto é preservado.

O código representa a implementação.

O contexto representa o conhecimento.

Conhecimento nunca deve depender da memória das pessoas.

---

# Quando utilizar

Esta etapa inicia após a definição da arquitetura.

Neste momento o projeto já possui:

- problema validado;
- visão definida;
- arquitetura organizada.

Agora é necessário construir sua memória permanente.

---

# Resultado Esperado

Ao final desta etapa devemos possuir um projeto completamente compreensível.

Qualquer pessoa deve conseguir responder:

- Por que este produto existe?
- Como ele funciona?
- Quais módulos existem?
- Quais decisões já foram tomadas?
- Como ele deve evoluir?

Sem precisar perguntar ao autor.

---

# Processo

## Etapa 1 — Organizar a Documentação

Toda documentação deve possuir uma responsabilidade única.

Exemplo:

README

Vision

Architecture

Business

Roadmap

Database

API

Modules

Decisions

Glossary

---

## Etapa 2 — Criar um Glossário

Todo projeto deve possuir um vocabulário oficial.

Registrar:

- termos do negócio;
- siglas;
- nomes de módulos;
- entidades;
- conceitos importantes.

Toda IA deverá utilizar este vocabulário.

---

## Etapa 3 — Registrar Regras de Negócio

Documentar todas as regras importantes.

Responder:

O sistema faz o quê?

Quando faz?

Por quê?

Quais exceções existem?

---

## Etapa 4 — Registrar Decisões

Toda decisão relevante deve ser documentada utilizando Architecture Decision Records (ADR).

Nenhuma decisão importante deve permanecer apenas na memória.

---

## Etapa 5 — Definir a Estrutura do Conhecimento

Organizar os documentos para que qualquer pessoa encontre rapidamente a informação necessária.

O conhecimento deve ser previsível.

---

## Etapa 6 — Preparar Contexto para IA

A documentação deve permitir que uma IA compreenda o projeto antes de gerar qualquer código.

Ela deve responder:

Qual é o objetivo?

Como o produto está organizado?

Quais módulos existem?

Quais padrões devem ser respeitados?

Quais decisões não podem ser quebradas?

---

# Estrutura Recomendada

Todo projeto deve possuir uma estrutura semelhante:

```
docs/

README.md

VISION.md

ARCHITECTURE.md

BUSINESS.md

ROADMAP.md

DATABASE.md

MODULES.md

API.md

GLOSSARY.md

DECISIONS/

ADR-0001.md

ADR-0002.md

...
```

Cada documento possui apenas uma responsabilidade.

---

# Perguntas Obrigatórias

## Produto

Por que este produto existe?

---

## Negócio

Qual transformação ele entrega?

---

## Arquitetura

Como ele está organizado?

---

## Módulos

Quais responsabilidades existem?

---

## Regras

Quais comportamentos são obrigatórios?

---

## Evolução

Como novas funcionalidades devem ser adicionadas?

---

# Artefatos Gerados

Ao concluir esta etapa devem existir:

- documentação centralizada;
- glossário oficial;
- regras de negócio;
- histórico de decisões;
- estrutura documental;
- contexto preparado para IA.

---

# O que evitar

Evite:

- documentação duplicada;
- conhecimento espalhado;
- nomes inconsistentes;
- documentos sem propósito;
- documentação desatualizada.

---

# Critérios para Encerramento

Esta etapa termina quando:

- [ ] Toda documentação principal existe.
- [ ] Existe um glossário oficial.
- [ ] As regras de negócio foram registradas.
- [ ] As decisões arquiteturais estão documentadas.
- [ ] A estrutura documental está organizada.
- [ ] Uma IA consegue compreender o projeto apenas lendo a documentação.

---

# Entregáveis

Ao concluir esta etapa devem existir:

- Documentation Structure
- Business Rules
- Glossary
- ADR Repository
- Context Repository

Esses artefatos serão utilizados para geração do backlog e implementação.

---

# Próxima Etapa

Com o contexto consolidado, iniciamos a decomposição do projeto em entregas.

Consulte:

**05_Backlog**

---

# Regra Final

Código envelhece.

Tecnologias mudam.

Ferramentas são substituídas.

O contexto permanece.

Proteja o conhecimento do projeto com o mesmo cuidado dedicado ao seu código.
