# Documentation Principle

Versão: 1.0

---

# Objetivo

A documentação é a memória permanente da empresa.

Ela existe para garantir que qualquer pessoa — humana ou Inteligência Artificial — consiga compreender, evoluir e manter um projeto sem depender de conhecimento implícito.

Nosso objetivo não é documentar tudo.

Nosso objetivo é documentar aquilo que influencia decisões futuras.

---

# Princípio Fundamental

> Se uma decisão é importante, ela deve existir na documentação.

Conhecimento que permanece apenas na memória das pessoas torna o projeto mais frágil.

A documentação é a fonte oficial da verdade.

---

# Por que existe?

Documentamos para:

- reduzir retrabalho;
- preservar conhecimento;
- acelerar o onboarding;
- facilitar manutenção;
- registrar decisões;
- permitir evolução contínua.

A documentação deve sobreviver às pessoas.

---

# Regras

Todo projeto deve documentar, no mínimo:

**Visão** — por que o projeto existe.

**Problema** — qual problema está sendo resolvido.

**Público** — para quem o projeto foi criado.

**Arquitetura** — como o sistema está organizado.

**Regras de Negócio** — como o sistema deve se comportar.

**Banco de Dados** — quais entidades existem e como se relacionam.

**APIs** — como os módulos se comunicam.

**Decisões Arquiteturais** — toda decisão importante deve possuir contexto e justificativa.

**Roadmap** — como o projeto pretende evoluir.

Quando existir conflito entre código e documentação, a documentação prevalece. O código deverá ser ajustado.

Toda alteração significativa no projeto exige atualização da documentação correspondente.

Nunca implementar primeiro e documentar depois.

---

# Boas Práticas

**Clara** — qualquer pessoa deve conseguir compreender rapidamente.

**Atualizada** — documentação desatualizada é pior do que não possuir documentação.

**Objetiva** — cada documento deve possuir um propósito claro.

**Modular** — cada assunto deve possuir seu próprio documento. Nunca criar documentos gigantes que tratem de muitos assuntos diferentes.

**Atemporal** — evitar referências temporárias. Documentos devem continuar úteis mesmo após meses ou anos.

Toda IA utilizada pela empresa deve consultar a documentação antes de escrever código, gerar arquitetura, criar banco de dados, modificar regras de negócio ou criar novos módulos.

---

# O que evitar

- Documentar código linha por linha.
- Registrar informações temporárias.
- Incluir opiniões pessoais.
- Criar documentos gigantes com múltiplos assuntos.
- Documentar após implementar.
- Manter documentação desatualizada.
- Confiar na memória como substituto da documentação.

---

# Checklist

Antes de iniciar qualquer implementação, confirme:

- [ ] Existe um documento de visão.
- [ ] Existe arquitetura definida.
- [ ] Existe modelagem do banco.
- [ ] Existem regras de negócio.
- [ ] Existem decisões registradas.
- [ ] Existe roadmap.
- [ ] O contexto está atualizado.

Se qualquer resposta for negativa, interrompa a implementação e complete a documentação primeiro.

---

# Regra Final

Código pode ser reescrito.

Documentação representa conhecimento.

Proteja o conhecimento antes de proteger o código.
