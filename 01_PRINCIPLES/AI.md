# AI Principle

Versão: 1.0

---

# Objetivo

A Inteligência Artificial é um membro da equipe.

Ela auxilia na execução, na documentação, na geração de código e na análise de problemas.

Nosso objetivo não é substituir decisões humanas por decisões automáticas.

Nosso objetivo é ampliar a capacidade humana através de sistemas de IA bem orientados.

---

# Princípio Fundamental

> A IA executa. O Product Owner decide.

A IA nunca substitui o julgamento estratégico humano.

Ela é tão boa quanto o contexto que recebe.

Contexto ruim gera resultado ruim, independentemente da capacidade do modelo.

---

# Por que existe?

Sem princípios claros, o uso de IA em projetos tende a gerar:

- código que contradiz a arquitetura existente;
- funcionalidades fora do escopo documentado;
- decisões tomadas sem raciocínio registrado;
- perda de consistência entre módulos;
- retrabalho causado por contexto insuficiente.

Este princípio define como a IA deve operar dentro dos projetos ZRO.

---

# Regras

A IA deve consultar a documentação antes de executar qualquer tarefa.

A ordem de leitura obrigatória é:

1. README do projeto.
2. Visão e Manifesto.
3. Arquitetura.
4. Contexto da fase atual.
5. Tarefa específica.

A IA deve executar apenas o que foi solicitado.

Nunca adicionar funcionalidades fora do escopo.

Nunca refatorar código não relacionado à tarefa.

Nunca tomar decisões arquiteturais sem registro.

Quando houver conflito entre código e documentação, a documentação prevalece.

A IA deve sinalizar quando o contexto for insuficiente para executar a tarefa com segurança.

---

# Boas Práticas

**Forneça contexto completo** — quanto mais contexto, mais precisa é a execução.

**Defina o escopo com clareza** — a IA trabalha melhor com objetivos específicos e critérios de aceite mensuráveis.

**Revise sempre** — toda entrega da IA deve ser revisada por um humano antes de ser considerada concluída.

**Use checklists** — oriente a IA a seguir os checklists do Playbook antes de cada execução.

**Registre decisões** — se a IA sugerir uma mudança arquitetural, registre antes de aceitar.

**Itere com documentação** — ao evoluir um projeto com IA, mantenha a documentação atualizada a cada iteração.

---

# O que evitar

- Executar tarefas com IA sem fornecer contexto do projeto.
- Aceitar entregas da IA sem revisão humana.
- Permitir que a IA tome decisões estratégicas ou arquiteturais sem registro.
- Usar a IA para contornar processos do Playbook.
- Assumir que a IA lembra de conversas anteriores sem contexto explícito.
- Tratar a saída da IA como fonte da verdade sem validação.

---

# Checklist

Antes de executar qualquer tarefa com IA, confirme:

- [ ] O contexto do projeto foi fornecido.
- [ ] A documentação relevante foi referenciada.
- [ ] O escopo está claro e fechado.
- [ ] Os critérios de aceite estão definidos.
- [ ] A entrega será revisada por um humano.
- [ ] Decisões geradas pela IA serão registradas antes de serem aceitas.

---

# Regra Final

A IA é tão útil quanto o contexto que recebe e tão confiável quanto a revisão que a valida.

Invista em contexto.

Revise sempre.

Decida você.
