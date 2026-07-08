# Prompt: Implementar Tarefa

Use este template para instruir a IA a implementar qualquer tarefa.

---

```
🎯 OBJETIVO: [Uma frase clara — o que deve acontecer]

📍 CONTEXTO:
- Projeto: [nome]
- Módulo/arquivo: [localização exata]
- Por quê agora: [razão / prioridade]

✅ SUCESSO DEFINIDO COMO:
- [ ] [Critério 1 — específico, mensurável, testável]
- [ ] [Critério 2]
- [ ] [Critério 3]

⚡ CONSTRAINT:
- Tempo máx: [X minutos]
- Scope: [o que NÃO incluir]
- Dependências: [o que já deve estar pronto]

🚫 NÃO FAZER:
- [ ] Sem refactor de código não relacionado
- [ ] Sem novas abstrações
- [ ] Sem features além do pedido
- [ ] Sem otimizações não solicitadas

🔪 MUDANÇAS CIRÚRGICAS:
- Arquivos tocados: máx 2 [liste]
- Linhas alteradas: máx 10 [estimativa]

🔍 VALIDAÇÃO:
- Como testar: [comando, browser, console]
- Sem regressão em: [features críticas]
```

---

## Exemplo preenchido

```
🎯 OBJETIVO: Adicionar campo de cupom no checkout

📍 CONTEXTO:
- Projeto: marketplace-machine
- Módulo: app/diagnostico/page.tsx (linha 47 — formulário de checkout)
- Por quê agora: beta testers precisam de desconto para validação

✅ SUCESSO DEFINIDO COMO:
- [ ] Campo de texto "Cupom" aparece no formulário
- [ ] POST /api/cupom/validar chamado ao digitar
- [ ] Desconto exibido quando cupom válido
- [ ] Erro exibido quando cupom inválido

⚡ CONSTRAINT:
- Tempo máx: 30 min
- Scope: apenas UI + chamada de API, sem criar novos cupons
- Dependências: /api/cupom/validar já existe

🚫 NÃO FAZER:
- [ ] Sem refactor do formulário existente
- [ ] Sem criar sistema de cupons completo
- [ ] Sem alterar o fluxo de pagamento

🔍 VALIDAÇÃO:
- Testar com cupom BETA29 (deve retornar R$29,90)
- Testar com cupom inválido (deve mostrar erro)
- Sem regressão no formulário principal
```
