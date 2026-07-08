# Checklist: Antes do Deploy

Execute antes de qualquer deploy em produção.

---

## Código

- [ ] TypeScript sem erros (`tsc --noEmit`)
- [ ] Sem `console.log` de debug expostos
- [ ] Variáveis de ambiente documentadas em `.env.example`
- [ ] Sem credenciais hardcoded

## Banco de Dados

- [ ] Migrations testadas em ambiente de desenvolvimento
- [ ] RLS configurado para todas as tabelas novas
- [ ] Campos sensíveis identificados e protegidos
- [ ] Backup disponível antes de migrations destrutivas

## Funcionalidade

- [ ] Fluxo principal testado manualmente (happy path)
- [ ] Estados de erro testados
- [ ] Estados vazios testados
- [ ] Mobile testado (se aplicável)

## Documentação

- [ ] `status.md` do projeto atualizado
- [ ] Decisões novas registradas em `decisions/`
- [ ] Tasks concluídas marcadas

## Deploy

- [ ] Variáveis de ambiente configuradas no ambiente de destino
- [ ] Sem breaking changes não comunicados
- [ ] Plano de rollback definido para mudanças de schema

**Deploy só ocorre com todos os itens marcados.**
