# Prompt: Revisar Código

Use este prompt para pedir à IA uma revisão de código alinhada à metodologia ZRO.

---

```
Revise o código a seguir usando os critérios da Skill Product Context Engineering.

Contexto do projeto:
- [cole o VISION.md ou um resumo de 3 linhas]

Código a revisar:
[cole o código ou indique o arquivo]

Avalie os seguintes critérios:

1. ESCOPO
   - O código faz apenas o que foi pedido?
   - Há funcionalidades não solicitadas?

2. CIRURGIA
   - O código modifica apenas o necessário?
   - Há mudanças colaterais desnecessárias?

3. COERÊNCIA COM O PRODUTO
   - O código contradiz alguma decisão documentada?
   - O código contradiz o MANIFESTO ou a VISION?

4. SEGURANÇA
   - Há dados sensíveis expostos?
   - Há validações ausentes em system boundaries?
   - Há credenciais hardcoded?

5. QUALIDADE
   - O código é compreensível sem comentários?
   - Há abstrações prematuras?
   - Há complexidade desnecessária?

Para cada problema encontrado:
- Identifique o arquivo e a linha
- Explique o problema em 1 frase
- Sugira a correção mínima necessária

Não sugira melhorias fora do escopo do que foi revisado.
```
