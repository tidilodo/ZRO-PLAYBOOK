# Exemplo — ANKHE / Oráculo OS

Versão: 1.0

---

# O que é

ANKHE é o primeiro produto construído com a metodologia Product Context Engineering da ZRO.

Ele serve como projeto de referência para demonstrar como a metodologia funciona na prática.

---

# Sobre o Produto

**Nome:** Oráculo OS

**Tipo:** SaaS para terapeutas e profissionais de desenvolvimento humano

**Missão:** Ampliar a capacidade de terapeutas sem substituir sua essência.

**Stack:** Next.js + TypeScript + Tailwind + Supabase + AWS Bedrock (Claude Sonnet 4.6)

**URL:** ankhe-rkxuwjz39-tidilodos-projects-638506dd.vercel.app

---

# Como a Metodologia PCE foi Aplicada

## 01 — Discovery

**Problema identificado:** terapeutas possuem profundidade técnica mas dificuldade em comunicar valor e criar conteúdo consistente.

**Público:** terapeutas, mentores, profissionais de autoconhecimento e desenvolvimento humano.

**Hipótese validada:** se a IA aprender a identidade do profissional, pode gerar conteúdo coerente com sua essência.

---

## 02 — Vision

**Missão:** ampliar a capacidade de terapeutas sem substituir sua essência.

**Transformação:** profissional para de improvisar comunicação e passa a ter presença digital coerente com quem é.

**Diferencial:** a IA nunca improvisa — ela consulta a Chave Ankhe antes de qualquer geração.

**Limites definidos:** a IA não diagnostica, não garante resultados, não substitui a presença humana.

---

## 03 — Architecture

**Mapa de Domínios aplicado:**

```
Oráculo OS

├── Domínio Identidade
│   └── Chave Ankhe (8 dimensões do DNA do profissional)
│
├── Domínio Inteligência
│   └── Ankhe Core AI (consulta Chave antes de gerar)
│
├── Domínio Ressonância (Fase 1)
│   └── Oráculo Studio (pilares, ideias, legendas, calendário)
│
├── Domínio Plataforma
│   ├── Autenticação (Supabase Auth)
│   ├── Tenants (multi-tenancy)
│   └── Auditoria
│
└── Módulos Futuros
    ├── Transmutação (Mapas, Journey)
    └── Manifestação (CRM, Launch)
```

---

## 04 — Context

**Context Score calculado antes da implementação:**

| Documento | Peso | Status |
|-----------|------|--------|
| Vision | 20 | ✅ |
| Architecture | 20 | ✅ |
| Business Rules | 15 | ✅ |
| Glossary | 10 | ✅ |
| ADRs | 10 | ✅ |
| Database | 10 | ✅ |
| Roadmap | 10 | ✅ |
| Module Docs | 5 | ✅ |

**Score: 100/100** — desenvolvimento assistido por IA liberado.

**45 tasks documentadas** antes de escrever uma linha de código.

---

## 05 — Backlog

**Épicos da Fase 1:**

- Autenticação e Tenant
- Chave Ankhe (8 dimensões)
- Ankhe Core AI
- Oráculo Studio

**45 tasks quebradas** em unidades de máximo 1 dia, cada uma com objetivo, requisitos e critérios de aceite.

---

## 06 — Implementation

**Stack implementada:**

```
Next.js 16 (App Router) + TypeScript
Tailwind CSS
Supabase (Auth + PostgreSQL + RLS)
AWS Bedrock — us.anthropic.claude-sonnet-4-6
Vercel (deploy)
```

**Conceitos centrais implementados:**

- `runAnkheCoreRaw()` — geração estruturada (pilares, ideias)
- `runAnkheCore()` — geração IAResponse (legendas)
- Service client — bypassa RLS em server actions
- `useRef(chaveId)` + debounce — evita criação de N registros

**Bugs críticos encontrados e resolvidos:**
- chave_ankhe criava 1 registro por keystroke → fix: ID em useRef + debounce 1s
- Pilares não apareciam → fix: runAnkheCoreRaw (sem wrapper IAResponse)
- RLS bloqueava inserts → fix: service client em todos os writes
- middleware deprecado Next.js 16 → fix: proxy.ts export `proxy`

---

## 07 — Evolution

**Fase G (próxima):** validação beta com 5-8 terapeutas reais.

**Métricas de sucesso definidas:**
- 80% conclui a Chave Ankhe na primeira semana
- Média ≥ 4/5 em "o conteúdo parece com você"
- 60% aprova 3 conteúdos

---

# Aprendizados para o Playbook

## O que funcionou bem

- Documentar 45 tasks antes de codar eliminou dúvidas durante implementação
- Context Score deu clareza objetiva de quando estava pronto
- Mapa de Domínios revelou limites entre módulos antes de qualquer conflito de responsabilidade

## O que pode melhorar

- Testar Context Score com outros produtos para calibrar os pesos
- Adicionar checklist específico para Next.js + Supabase em `04_CHECKLISTS/`
- Criar template de `context/` vivo separado dos `docs/` estáticos

---

# Repositório

Código fonte: `C:/Users/Utilizador/ankhe/`

Documentação: `C:/Users/Utilizador/Documents/ANKHE/`
