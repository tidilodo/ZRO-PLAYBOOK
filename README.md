# ZRO Engineering Playbook

Manual oficial de desenvolvimento da empresa.

Todo projeto deve seguir as Skills aqui documentadas antes da implementação.

Nunca iniciar um projeto diretamente pelo código.

---

## Estrutura

```
ZRO-PLAYBOOK/
├── README.md                          — este arquivo
└── skills/
    └── product-context-engineering/
        ├── README.md                  — visão geral da skill
        ├── SKILL.md                   — documento completo da metodologia
        ├── templates/                 — modelos vazios para novos projetos
        │   ├── VISION.md
        │   ├── MANIFESTO.md
        │   ├── ARCHITECTURE.md
        │   ├── GLOSSARY.md
        │   ├── BUSINESS.md
        │   ├── ROADMAP.md
        │   ├── MODULE.md
        │   ├── TECH.md
        │   └── DATABASE.md
        ├── checklists/                — listas de verificação por momento
        │   ├── NEW_PROJECT.md
        │   ├── BEFORE_CODING.md
        │   └── BEFORE_DEPLOY.md
        └── prompts/                   — instruções para IA
            ├── START_PROJECT.md
            ├── IMPLEMENT_TASK.md
            └── REVIEW_CODE.md
```

---

## Como usar

### Criar novo produto

1. Crie a pasta do produto: `NOME-DO-PRODUTO/`
2. Copie todos os templates de `skills/product-context-engineering/templates/` para `NOME-DO-PRODUTO/docs/`
3. Peça ao Claude: *"Preencha esses templates usando a Skill Product Context Engineering do ZRO-PLAYBOOK."*
4. Somente após docs preenchidos: inicie a implementação

### Estrutura padrão de produto

```
NOME-DO-PRODUTO/
├── docs/          — templates preenchidos (visão, manifesto, arquitetura...)
├── context/       — contexto vivo (fase ativa, personas, princípios)
├── tasks/         — tarefas quebradas por fase
├── apps/          — aplicações
├── packages/      — pacotes compartilhados
└── database/      — schema e documentação de dados
```

---

## Princípio fundamental

> A documentação é a fonte da verdade.
> O código manifesta a documentação.
> Nunca o contrário.
