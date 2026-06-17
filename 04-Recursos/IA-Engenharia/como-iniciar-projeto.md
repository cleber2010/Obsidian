---
tipo: recurso
tags: [ia, claude-code, workflow, automacao, projeto]
---

# Como Iniciar um Projeto de Automação

## Fluxo de trabalho

1. **Planejar** — pesquisar tecnologias, definir arquitetura, regras de negócio
2. **Criar** (em fases) — nunca tenta tudo de uma vez
3. **Testar** (em fases) — validar cada fase antes de avançar
4. **Subir / deploy** — colocar online
5. **Monetizar** — cobrar por acesso (licenças, mensalidade)

---

## Antes de abrir o Claude Code

- Tenha algo mais ou menos estruturado na cabeça antes de entrar no modo Plan
- Crie um arquivo `.txt` descrevendo a demanda
- Pesquisar tecnologias custa tokens — use uma conta secundária gratuita ou o GPT para pesquisas exploratórias de tecnologia e ideias

---

## O que descrever no planejamento

- Regras de negócio (não precisa ser todas, mas as principais)
- Alguma tecnologia que você já pesquisou
- Arquitetura de pastas pretendida
- Onde ficará o back end, front end e banco de dados
- Pedir sugestões ao Claude sobre o que falta

---

## Após planejar: solicitar um `plan.md`

Pedir ao Claude que gere um `plan.md` com:
- Etapas de implementação
- A cada etapa concluída: testar com Playwright MCP e pedir feedback antes de avançar
- Plano de deploy (ex: como subir numa VPS $5 da Digital Ocean)
- Sistema de licenças para monetização

---

## Sites para hospedagem e infra

- **Netlify / Vercel** — sites estáticos e serverless
- **Supabase** — banco de dados hospedado (PostgreSQL)
- **Railway / Render** — backend Python/Node
- **Digital Ocean VPS** — controle total, ~$5/mês

---

## Notas relacionadas

- [[claude-code-guia]]
- [[como-vender-automacoes]]
- [[_MOC-IA-Engenharia]]
