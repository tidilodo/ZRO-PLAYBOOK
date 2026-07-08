# Skill — Product Context Engineering

# 03 — Architecture

Versão: 1.0

---

# Objetivo

A etapa de Architecture transforma a visão do produto em uma estrutura organizada.

Seu objetivo é definir como o sistema será dividido, quais serão seus módulos, como eles se relacionam e quais responsabilidades cada um possuirá.

Arquitetura não define implementação.

Arquitetura define organização.

---

# Princípio Fundamental

> Um bom produto nasce de uma boa arquitetura.

Uma arquitetura clara reduz complexidade, facilita manutenção e permite evolução contínua.

---

# Quando utilizar

Esta etapa inicia apenas após a conclusão da Vision.

Neste momento o produto já possui:

- problema definido;
- público definido;
- proposta de valor;
- missão;
- limites de escopo.

---

# Resultado Esperado

Ao final desta etapa devemos responder:

- Quais módulos existirão?
- Qual responsabilidade cada módulo possui?
- Como os módulos se comunicam?
- Quais dependências são permitidas?
- Como o sistema poderá crescer?

---

# Processo

## Etapa 1 — Identificar os Domínios

Divida o produto em grandes áreas de responsabilidade.

Exemplos:

- Autenticação
- Usuários
- Pagamentos
- Conteúdo
- CRM
- Relatórios
- Inteligência Artificial

Cada domínio representa uma responsabilidade de negócio.

---

## Etapa 2 — Definir os Módulos

Cada domínio pode conter um ou mais módulos.

Um módulo deve possuir:

- responsabilidade única;
- documentação própria;
- evolução independente.

---

## Etapa 3 — Definir Responsabilidades

Responder:

O que este módulo faz?

O que ele não faz?

Quem depende dele?

De quem ele depende?

---

## Etapa 4 — Definir Fluxos

Mapear como as informações percorrem o sistema.

Responder:

Onde os dados entram?

Como são processados?

Quem consome os resultados?

---

## Etapa 5 — Definir Integrações

Listar integrações internas e externas.

Exemplos:

- APIs
- Webhooks
- Bancos de Dados
- Serviços de IA
- Gateways de pagamento

Toda integração deve possuir um responsável.

---

## Etapa 6 — Definir Limites

Registrar claramente:

O que pertence a cada módulo.

O que nunca deve ser responsabilidade daquele módulo.

---

# Perguntas Obrigatórias

## Organização

Como o sistema será dividido?

---

## Responsabilidades

Cada módulo possui apenas uma responsabilidade?

---

## Dependências

Existe baixo acoplamento?

---

## Evolução

Será possível adicionar novos módulos sem reescrever o sistema?

---

## Escalabilidade

O crescimento do produto já foi considerado?

---

# Arquitetura Recomendada

Todo projeto deve buscar a seguinte hierarquia:

```
Produto

↓

Domínios

↓

Módulos

↓

Componentes

↓

Serviços

↓

Implementação
```

Cada nível possui responsabilidades próprias.

---

# Artefatos Gerados

Ao concluir esta etapa devem existir:

- mapa de módulos;
- mapa de domínios;
- diagrama de arquitetura;
- fluxos principais;
- integrações;
- responsabilidades.

---

# O que evitar

Evite:

- escolher frameworks;
- discutir linguagem de programação;
- modelar banco de dados detalhadamente;
- implementar funcionalidades.

Arquitetura vem antes da implementação.

---

# Critérios para Encerramento

Esta etapa termina quando:

- [ ] Todos os módulos foram identificados.
- [ ] Cada módulo possui responsabilidade clara.
- [ ] As dependências estão documentadas.
- [ ] Os fluxos principais foram definidos.
- [ ] As integrações foram registradas.
- [ ] A arquitetura suporta evolução futura.

---

# Entregáveis

Ao concluir esta etapa devem existir:

- Architecture Overview
- Module Map
- Domain Map
- Integration Map
- Responsibility Matrix

Esses documentos servirão como base para a construção do contexto do projeto.

---

# Próxima Etapa

Com a arquitetura definida, inicia-se a criação da memória permanente do projeto.

Consulte:

**04_Context**

---

# Regra Final

Uma arquitetura não deve responder como escrever código.

Ela deve responder como o produto continuará organizado quando tiver dez vezes mais funcionalidades do que possui hoje.
