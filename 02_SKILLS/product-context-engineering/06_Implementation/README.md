# Skill — Product Context Engineering

# 06 — Implementation

Versão: 1.0

---

# Objetivo

A etapa de Implementation transforma o backlog em software funcional de forma incremental, preservando a arquitetura, a documentação e os princípios definidos anteriormente.

Implementar não significa apenas escrever código.

Implementar significa materializar uma decisão de produto com qualidade, consistência e rastreabilidade.

---

# Princípio Fundamental

> Toda implementação deve preservar o contexto do projeto.

O código nunca deve evoluir mais rápido que a documentação.

Cada entrega deve fortalecer o produto.

Nunca enfraquecer sua arquitetura.

---

# Quando utilizar

Esta etapa inicia apenas quando:

- Discovery foi concluído;
- Vision foi aprovada;
- Architecture está definida;
- Context está atualizado;
- Backlog está priorizado.

Se qualquer uma dessas etapas estiver incompleta, a implementação deve ser adiada.

---

# Resultado Esperado

Ao final desta etapa devemos possuir:

- funcionalidades entregues;
- arquitetura preservada;
- documentação atualizada;
- testes executados;
- backlog revisado.

Cada incremento deve gerar valor real para o produto.

---

# Processo

## Etapa 1 — Selecionar a User Story

Nunca implemente diretamente um Épico.

Nunca implemente diretamente uma Feature.

Toda implementação começa por uma única User Story.

---

## Etapa 2 — Compreender o Contexto

Antes de escrever código consulte:

- Vision
- Architecture
- Business Rules
- Glossary
- ADRs
- Documentação do módulo

Se existir qualquer dúvida, interrompa a implementação.

---

## Etapa 3 — Planejar a Solução

Antes do código responder:

- O que será alterado?
- Quais módulos serão impactados?
- Existe reutilização possível?
- Existe alguma decisão arquitetural relacionada?

---

## Etapa 4 — Implementar

Escreva apenas o necessário.

Priorize:

- simplicidade;
- legibilidade;
- reutilização;
- baixo acoplamento.

Evite soluções temporárias que se tornem permanentes.

---

## Etapa 5 — Validar

Após implementar verificar:

- comportamento esperado;
- regras de negócio;
- impacto em outros módulos;
- compatibilidade com arquitetura.

---

## Etapa 6 — Atualizar Documentação

Toda implementação relevante exige atualização da documentação correspondente.

Pode incluir:

- APIs;
- Banco de Dados;
- Regras de Negócio;
- ADRs;
- Roadmap;
- README do módulo.

Código e documentação evoluem juntos.

---

## Etapa 7 — Encerrar a Entrega

Ao concluir:

- atualizar backlog;
- registrar aprendizados;
- identificar melhorias futuras;
- preparar próxima User Story.

---

# Boas Práticas

Durante toda implementação:

- implementar pequenas entregas;
- realizar commits frequentes;
- preservar padrões;
- evitar duplicação;
- reutilizar componentes;
- escrever código compreensível.

---

# O que evitar

Evite:

- implementar múltiplas funcionalidades ao mesmo tempo;
- alterar arquitetura sem registro;
- criar dependências desnecessárias;
- ignorar documentação;
- adicionar funcionalidades fora do escopo.

---

# Relação com Inteligência Artificial

A IA deve atuar como colaboradora.

Antes de implementar ela deve:

- compreender o contexto;
- analisar impactos;
- seguir os princípios do Playbook.

Durante a implementação ela deve:

- preservar arquitetura;
- reutilizar componentes existentes;
- sugerir melhorias quando apropriado.

Após concluir:

- revisar código;
- verificar documentação;
- atualizar artefatos necessários.

---

# Critérios para Encerramento

Uma implementação somente é considerada concluída quando:

- [ ] A User Story foi atendida.
- [ ] A arquitetura foi preservada.
- [ ] O código segue os padrões definidos.
- [ ] Não existem duplicações desnecessárias.
- [ ] A documentação foi atualizada.
- [ ] Os testes relevantes foram executados.
- [ ] O backlog foi atualizado.

---

# Entregáveis

Ao concluir esta etapa devem existir:

- código implementado;
- documentação atualizada;
- testes executados;
- backlog atualizado;
- mudanças registradas.

---

# Próxima Etapa

Após cada implementação inicia-se o processo contínuo de evolução do produto.

Consulte:

**07_Evolution**

---

# Regra Final

Implementação não é o fim do processo.

É apenas a materialização temporária do conhecimento acumulado até aqui.

Toda linha de código deve preservar a visão, a arquitetura e o contexto do produto.
