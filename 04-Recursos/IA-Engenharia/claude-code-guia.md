---
tipo: recurso
tags: [ia, claude-code, workflow, mcp, skills]
---

# Claude Code — Guia Operacional

Notas sobre como operar o Claude Code de forma eficiente.

---

## CLAUDE.md

Arquivo na raiz do projeto que resume o contexto para o Claude, reduzindo consumo de tokens em novas sessões.

Comando principal: `/init` — gera um CLAUDE.md com documentação do codebase.

---

## Modo Plan

Use antes de implementar qualquer coisa complexa:
- Definir quais tecnologias usar
- Definir funcionalidades que o sistema deve ter
- Especificar regras de negócio
- Entender por que aquelas tecnologias são indicadas

Ajuda na construção de apps sem surpresas no meio do caminho.

---

## Skills

Instruções específicas que tornam o Claude mais eficiente para uma tarefa determinada.

Ex: "criar uma landing page elegante" com skills define padrões de UI/UX a partir de um `.md` específico.

**Estrutura:**
- Criar pasta `.claude/skills/`
- Colocar o arquivo `.md` da skill dentro
- Referenciar o nome da skill no prompt

Site para buscar skills prontas: https://skillsmp.com/

**Skills vs Plugins:**
- Skills resolve um único problema
- Plugins resolvem uma ou várias skills + hooks + agents em conjunto

---

## Servidores MCP

Funcionalidades prontas para usar em conjunto com o desenvolvimento:

- **context7** — documentação mais atualizada sobre frameworks e libs
- **Playwright MCP** — testa sites automaticamente

---

## Plugins

Agregado de configurações que trazem configs de MCP, Skills, hooks, etc. Mais abrangente que uma skill isolada.

---

## Notas relacionadas

- [[como-iniciar-projeto]]
- [[_MOC-IA-Engenharia]]
