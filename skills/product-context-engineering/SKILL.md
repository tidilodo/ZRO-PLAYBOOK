# Product Context Engineering

## A Metodologia ZRO

Versão: 1.0

---

## O Problema que Esta Skill Resolve

A maioria dos projetos de software começa pelo código.

O desenvolvedor recebe uma ideia, abre o editor, e começa a construir.

Sem visão documentada.
Sem escopo definido.
Sem decisões registradas.
Sem contexto para a IA.

O resultado é sempre o mesmo:

- Retrabalho por requisitos mal entendidos.
- Código que contradiz o propósito do produto.
- IA que gera funcionalidades fora do escopo.
- Projeto que cresce sem direção.

Product Context Engineering resolve isso na origem.

---

## O Princípio Central

> A documentação é a fonte da verdade.
> O código manifesta a documentação.
> Nunca o contrário.

Antes de qualquer implementação, o projeto precisa ter:

1. Visão clara do problema e da solução.
2. Manifesto com os valores inegociáveis.
3. Arquitetura definida.
4. Glossário oficial de termos.
5. Modelo de negócio documentado.
6. Roadmap com fases e escopo.
7. Stack técnica decidida.
8. Schema de dados conceitual.
9. Tarefas quebradas em unidades executáveis.

Somente com esses documentos preenchidos, o código começa.

---

## Os 4 Pilares de Execução

### 1. Think Before Coding

Planeje antes de executar.

**Antes de qualquer código:**
- Ler os documentos do projeto.
- Entender o estado atual vs. o que precisa fazer.
- Identificar dependências e bloqueadores.
- Definir o objetivo com precisão.

**Antes de qualquer tarefa:**
- O que exatamente precisa mudar? (1 frase)
- Por que isso resolve o problema? (1 frase)
- Quais arquivos vão mudar? (lista)
- O que pode quebrar? (riscos)
- Como vou testar? (critério claro)

Se não conseguir responder tudo: **pare e planeje antes**.

---

### 2. Simplicity First

Implemente APENAS o pedido. Nada mais.

**Nunca:**
- Adicionar features não mencionadas
- Refatorar código não relacionado
- Criar abstrações para o futuro
- Adicionar error handling extra
- Otimizar o que não foi pedido

**Sempre:**
- Fazer exatamente o pedido
- Confiar no framework e no código existente
- Validar apenas em system boundaries
- Parar quando o objetivo for atingido

> Se não foi pedido, não foi pedido.

---

### 3. Surgical Changes

Cada mudança deve ser um corte cirúrgico.

**Padrão cirúrgico:**
- 1-2 arquivos modificados
- 3-10 linhas alteradas
- Zero reorganização de estrutura
- Zero limpeza de código não relacionado

**Anti-padrão proibido: "Enquanto estou aqui..."**

"Enquanto estou aqui, vou refatorar" → NÃO.
"Já que vou tocar aqui, vou limpar" → NÃO.
"Vou aproveitar para melhorar" → NÃO.

> Toque apenas o necessário. Saia do arquivo. Ponto final.

---

### 4. Goal Driven Execution

Foco laser no objetivo. Ignore tudo mais.

**Durante execução, se encontrar:**
- Code smells → IGNORE
- Débito técnico → IGNORE
- Bugs relacionados → IGNORE
- Oportunidades de melhoria → IGNORE

**Parar quando o objetivo for atingido.**

"Mas poderia melhorar..." → Não. FIM.

---

## Os 9 Documentos de Contexto

### VISION.md
Define o problema, o público, a transformação e o objetivo.

É o documento mais importante. Sem visão clara, tudo o mais é improviso.

Responde: **Por que este produto existe?**

---

### MANIFESTO.md
Define crenças, valores e princípios inegociáveis.

É o filtro ético e filosófico do produto. Toda decisão que contradiz o manifesto deve ser recusada.

Responde: **O que nunca faremos, independentemente da pressão?**

---

### ARCHITECTURE.md
Define camadas, módulos, responsabilidades, fluxos e dependências.

É o mapa do sistema. Antes de criar qualquer arquivo, a arquitetura deve estar documentada.

Responde: **Como o sistema está organizado?**

---

### GLOSSARY.md
Define os termos oficiais do projeto.

Nenhum termo pode ter duas interpretações. Se houver conflito entre o glossário e outro documento, o glossário prevalece.

Responde: **O que cada palavra significa neste projeto?**

---

### BUSINESS.md
Define modelo de negócio, fontes de receita, custos, métricas e público-alvo.

Responde: **Como este produto gera e sustenta valor?**

---

### ROADMAP.md
Define fases, escopo de cada fase e critérios de conclusão.

Cada fase deve ser pequena o suficiente para validar uma hipótese específica.

Responde: **O que vai ser construído, em que ordem e por quê?**

---

### MODULE.md
Define a especificação de um módulo específico: o que faz, o que não faz, suas interfaces e dependências.

Usado quando o projeto tem múltiplos módulos independentes.

Responde: **O que este módulo faz e onde terminam suas responsabilidades?**

---

### TECH.md
Define a stack técnica, as decisões arquiteturais e as justificativas.

Toda escolha de tecnologia deve ser documentada aqui com justificativa. Mudanças de stack exigem atualização do documento antes da implementação.

Responde: **Por que escolhemos estas tecnologias?**

---

### DATABASE.md
Define o modelo conceitual de dados: entidades, relacionamentos, campos sensíveis, regras de acesso.

Responde: **Quais dados o sistema armazena e como eles se relacionam?**

---

## O Documento de Tarefas

Após os 9 documentos preenchidos, as tarefas são quebradas seguindo estas regras:

- Nenhuma tarefa maior que 1 dia de desenvolvimento.
- Cada tarefa tem: objetivo, requisitos, critérios de aceite, dependências, estimativa.
- Tarefas maiores são quebradas antes de entrar em execução.
- A sequência respeita dependências — nenhuma tarefa começa antes de suas dependências estarem concluídas.

---

## O Fluxo Completo

```
1. Criar VISION        → por que existe?
2. Criar MANIFESTO     → o que nunca faremos?
3. Criar ARCHITECTURE  → como está organizado?
4. Criar GLOSSARY      → o que cada termo significa?
5. Criar BUSINESS      → como gera valor?
6. Criar ROADMAP       → o que será construído?
7. Criar TECH          → qual a stack e por quê?
8. Criar DATABASE      → quais dados e como?
9. Quebrar TAREFAS     → executáveis, com critérios

10. Implementar — apenas agora.
```

---

## Como a IA Usa Este Contexto

Quando o Claude Code recebe uma tarefa, ele deve:

1. Ler VISION — entender o propósito do produto.
2. Ler MANIFESTO — entender os limites inegociáveis.
3. Ler ARCHITECTURE — entender onde a mudança se encaixa.
4. Ler TECH — entender a stack e as decisões tomadas.
5. Ler a tarefa — entender exatamente o que precisa ser feito.
6. Confirmar escopo — nada fora da tarefa será feito.
7. Implementar — cirurgicamente, com foco no objetivo.
8. Atualizar documentação — se algo mudou, documentar antes do próximo passo.

---

## Regras para a IA

### Antes de codar

```
[ ] Li o VISION.md?
[ ] Li o MANIFESTO.md?
[ ] Li o ARCHITECTURE.md?
[ ] Li o TECH.md?
[ ] A tarefa está claramente definida?
[ ] O escopo está fechado?
[ ] Sei exatamente o que NÃO fazer?
```

Se qualquer resposta for não: **pare e leia antes**.

### Durante a implementação

```
A cada linha escrita:
[ ] Esta linha é necessária para o objetivo?
[ ] Esta linha vai afetar outro código?
[ ] Estou melhorando algo que não foi pedido?
[ ] Quantos arquivos estou modificando? (máx 2)
```

### Após a implementação

```
[ ] O objetivo foi atingido?
[ ] Nenhum arquivo desnecessário foi modificado?
[ ] Nenhuma feature extra foi adicionada?
[ ] A documentação foi atualizada?
[ ] O commit reflete exatamente o que foi feito?
```

---

## O Padrão de Instrução para a IA

Use este template para toda instrução ao Claude Code:

```
🎯 OBJETIVO: [Uma frase clara — o que deve acontecer]

📍 CONTEXTO:
- Projeto: [nome]
- Módulo/arquivo: [localização]
- Por quê agora: [razão]

✅ SUCESSO DEFINIDO COMO:
- [ ] Critério 1 (específico, mensurável, testável)
- [ ] Critério 2
- [ ] Critério 3

⚡ CONSTRAINT:
- Tempo máx: [X minutos]
- Scope: [o que NÃO incluir]
- Dependências: [o que já deve estar pronto]

🔍 VALIDAÇÃO:
- Como testar: [comando, browser, console]
- Sem regressão em: [features críticas]
```

---

## Erros Mais Comuns

### Erro 1: Começar pelo código

Sintoma: "Vou codar e documentar depois."
Consequência: Retrabalho, inconsistência, débito técnico acumulado.
Correção: Documentação primeiro, sempre.

### Erro 2: Escopo aberto

Sintoma: "Faça o módulo de autenticação."
Consequência: IA interpreta, adiciona, expande. Resultado imprevisível.
Correção: Escopo fechado com critérios mensuráveis.

### Erro 3: "Enquanto estou aqui"

Sintoma: IA refatora código não relacionado durante uma tarefa.
Consequência: Regressões, código novo não testado, escopo expandido.
Correção: Cada tarefa tem um objetivo. Ponto final.

### Erro 4: Documentação desatualizada

Sintoma: Código contradiz a documentação.
Consequência: IA trabalha com contexto errado nas próximas tarefas.
Correção: Atualizar documentação antes de fechar qualquer tarefa.

### Erro 5: Tarefas grandes demais

Sintoma: "Implemente o módulo completo de pagamento."
Consequência: Impossível de testar, revisar ou fazer rollback.
Correção: Quebrar em tarefas de no máximo 1 dia, com critérios de aceite claros.

---

## Princípio Final

> Código é manifestação.
> Documentação é direção.
> Sem direção, não há implementação.

A velocidade real vem da clareza, não da pressa.

Um projeto bem documentado é executado mais rápido do que um projeto que começa pelo código — porque elimina o retrabalho antes que ele aconteça.
