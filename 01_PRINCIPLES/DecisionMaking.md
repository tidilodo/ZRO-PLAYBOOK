# Decision Making Principle

Versão: 1.0

---

# Objetivo

Este documento define como decisões técnicas, arquiteturais e de produto devem ser tomadas, registradas e comunicadas.

Nosso objetivo é garantir que todas as decisões importantes sejam transparentes, rastreáveis e compreensíveis ao longo do tempo.

Nenhuma decisão relevante deve depender exclusivamente da memória de uma pessoa.

---

# Princípio Fundamental

> Toda decisão importante deve possuir contexto, justificativa e consequências documentadas.

A qualidade de um projeto não depende apenas das decisões tomadas, mas da capacidade de compreender por que elas foram tomadas.

---

# Por que registrar decisões?

Registrar decisões permite:

- preservar conhecimento;
- reduzir retrabalho;
- acelerar onboarding;
- evitar discussões repetidas;
- facilitar futuras revisões;
- manter consistência arquitetural.

Decisões documentadas tornam o projeto previsível.

---

# O que é uma decisão?

Uma decisão é qualquer escolha que impacte a arquitetura, o produto ou o processo de desenvolvimento.

Exemplos:

- escolha da stack tecnológica;
- definição da arquitetura;
- adoção de uma biblioteca;
- criação de um novo módulo;
- alteração de um fluxo crítico;
- mudança de regras de negócio;
- integração com serviços externos.

Pequenas implementações locais normalmente não exigem registro.

---

# Regras

Uma decisão deve ser registrada quando:

- altera a arquitetura;
- cria dependências permanentes;
- modifica regras importantes;
- impacta múltiplos módulos;
- influencia futuras implementações;
- possui alternativas relevantes.

Toda decisão deve seguir o padrão ADR (Architecture Decision Record):

```
Número

Título

Status

Data

---

## Contexto

Qual problema motivou esta decisão?

---

## Alternativas

Quais opções foram consideradas?

---

## Decisão

Qual opção foi escolhida?

---

## Justificativa

Por que essa opção foi escolhida?

---

## Consequências

Quais benefícios?

Quais limitações?

Quais riscos?

---

## Próxima revisão

Quando esta decisão deverá ser reavaliada?
```

Todas as decisões devem ser armazenadas em:

```
/decisions

0001-nome-da-decisao.md

0002-outra-decisao.md
```

A numeração nunca deve ser alterada.

Uma decisão nunca deve ser editada para representar outra realidade. Caso seja necessário alterar uma decisão existente, manter o documento original, criar uma nova decisão e referenciar a anterior. O histórico deve ser preservado.

A IA nunca deve alterar decisões arquiteturais sem autorização explícita do Product Owner. Antes de sugerir mudanças, a IA deve consultar decisões anteriores, avaliar impactos, apresentar alternativas e justificar a recomendação.

---

# Boas Práticas

**Clara** — qualquer pessoa deve compreender rapidamente.

**Justificada** — explicar por que foi escolhida, não apenas o que foi escolhido.

**Objetiva** — evitar excesso de detalhes desnecessários.

**Revisável** — nenhuma decisão é definitiva. Toda decisão pode evoluir quando existir uma justificativa melhor.

**Rastreável** — sempre deve ser possível descobrir quando foi tomada, quem aprovou e por que foi tomada.

---

# O que evitar

- Decisões implícitas não documentadas.
- Mudanças arquiteturais sem registro.
- Justificativas vagas ou ausentes.
- Alterações silenciosas em decisões existentes.
- Apagar o histórico de decisões anteriores.
- Permitir que a IA altere decisões sem aprovação humana.

---

# Checklist

Antes de aprovar uma decisão, confirme:

- [ ] O problema está claramente definido.
- [ ] As alternativas foram avaliadas.
- [ ] A decisão está documentada.
- [ ] As consequências foram registradas.
- [ ] Existe uma justificativa clara.
- [ ] A documentação foi atualizada.
- [ ] Os módulos impactados foram identificados.

---

# Regra Final

Decisões documentadas constroem conhecimento.

Conhecimento compartilhado constrói produtos duradouros.

Nunca permita que uma decisão importante exista apenas na memória de uma pessoa.
