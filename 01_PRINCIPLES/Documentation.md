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

# Por que documentamos?

Documentamos para:

- reduzir retrabalho;
- preservar conhecimento;
- acelerar o onboarding;
- facilitar manutenção;
- registrar decisões;
- permitir evolução contínua.

A documentação deve sobreviver às pessoas.

---

# O que deve ser documentado?

Todo projeto deve documentar, no mínimo:

## Visão

Por que o projeto existe.

---

## Problema

Qual problema está sendo resolvido.

---

## Público

Para quem o projeto foi criado.

---

## Arquitetura

Como o sistema está organizado.

---

## Regras de Negócio

Como o sistema deve se comportar.

---

## Banco de Dados

Quais entidades existem e como se relacionam.

---

## APIs

Como os módulos se comunicam.

---

## Decisões Arquiteturais

Toda decisão importante deve possuir contexto e justificativa.

---

## Roadmap

Como o projeto pretende evoluir.

---

# O que NÃO documentamos

Não documentamos:

- código linha por linha;
- informações temporárias;
- opiniões pessoais;
- tarefas concluídas que não possuem impacto futuro.

Documentação deve representar conhecimento permanente.

---

# Características de uma boa documentação

Uma boa documentação deve ser:

## Clara

Qualquer pessoa deve conseguir compreender rapidamente.

---

## Atualizada

Documentação desatualizada é pior do que não possuir documentação.

---

## Objetiva

Evitar excesso de texto.

Cada documento deve possuir um propósito claro.

---

## Modular

Cada assunto deve possuir seu próprio documento.

Nunca criar documentos gigantes que tratem de muitos assuntos diferentes.

---

## Atemporal

Evitar referências temporárias.

Documentos devem continuar úteis mesmo após meses ou anos.

---

# Estrutura Recomendada

```
Projeto

README

Visão

Manifesto

Arquitetura

Banco

Negócio

Roadmap

Módulos

Contexto

Decisões

Tarefas
```

Cada documento possui uma única responsabilidade.

---

# Fonte da Verdade

Sempre que existir conflito entre:

Código

e

Documentação

A documentação prevalece.

O código deverá ser ajustado.

---

# Atualização

Toda alteração significativa no projeto exige atualização da documentação correspondente.

Nunca implementar primeiro e documentar depois.

Sempre evoluir ambos juntos.

---

# Relação com Inteligência Artificial

Toda IA utilizada pela empresa deve consultar a documentação antes de:

- escrever código;
- gerar arquitetura;
- criar banco de dados;
- modificar regras de negócio;
- criar novos módulos.

A documentação representa o contexto oficial do projeto.

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
