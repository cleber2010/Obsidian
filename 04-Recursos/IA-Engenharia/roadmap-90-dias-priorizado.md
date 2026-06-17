---
tipo: recurso
tags: [ia, roadmap, carreira, portfólio, planejamento]
---

# Roadmap Priorizado — Plano de 90 dias + Trilha Integrada

Versão priorizada do roadmap, pensada para gerar **portfólio e oportunidades reais em até 90 dias**, sem abandonar o resto — só reordenando. As duas trilhas (Engenharia de IA e IA Criativa) foram fundidas onde fazia sentido.

Ver também: [[Roadmap-Especializacao-IA]] (nota de projeto com checklist geral)

---

## Fase 0 — Sprint de Portfólio (Dias 1–30)

Objetivo: ter pelo menos 1 case publicado e 1 agente funcionando antes de qualquer curso novo.

- [ ] Documentar o projeto de dados eleitorais do Podemos como case (problema → solução → resultado, com números)
- [ ] Documentar as automações Python da Matrix Energia como case (Salesforce/SharePoint)
- [ ] Criar repositório GitHub organizado com esses 2 projetos (README bom, sem dados sensíveis)
- [ ] Construir um agente simples: Claude API + tool use + RAG básico sobre dados eleitorais (TSE/municípios) — vira o 3º case
- [ ] Publicar 1 post técnico no LinkedIn sobre o case eleitoral ("como usei IA para automatizar X municípios")
- [ ] Atualizar perfil do Upwork com esses 3 cases

---

## Fase 1 — Fundamentos técnicos essenciais (Dias 30–60)

### Claude / API Anthropic

- [x] Praticar artifacts para gerar código, docs e visualizações
- [x] Criar projeto no Claude.ai para Podemos/dados eleitorais
- [x] Criar projeto no Claude.ai para Automação & Freelance
- [x] Configurar memórias e instruções personalizadas
- [x] Criar conta na Anthropic + primeira chamada via API
- [x] Implementar conversa multi-turn + streaming
- [x] Tratar erros HTTP (429, 529, 400) + variáveis de ambiente

### Infra básica

- [ ] Docker: conceitos básicos, criar um Dockerfile simples para uma API Python
- [ ] FastAPI: criar uma API mínima que chama a Claude API
- [ ] Deploy simples (Railway ou Render) — ter 1 projeto online com link público

---

## Fase 2 — Orquestração avançada (Dias 60–90)

### Tool use e agentes

- [ ] Loop completo tool_use → tool_result → resposta final
- [ ] Agente com acesso a arquivos locais
- [ ] Agente com acesso a API externa (TSE, IBGE)

### MCP

- [ ] Entender MCP e configurar Claude Desktop
- [ ] Conectar MCP ao Google Drive, Gmail, Calendar
- [ ] Testar integração MCP + n8n

### Multi-agente

- [ ] Estudar LangGraph (orquestração de agentes com estado/grafo)
- [ ] Estudar CrewAI como alternativa mais simples
- [ ] Avaliar se faz sentido usar LangChain só para RAG

### Avaliação e observabilidade

- [ ] Entender o conceito de "LLM eval"
- [ ] Testar LangSmith ou logging próprio para rastrear chamadas e custos
- [ ] Criar um dataset pequeno de testes ("golden set") pro agente eleitoral

### RAG e memória

- [ ] Embeddings e busca semântica
- [ ] Pinecone ou Qdrant
- [ ] RAG aplicado em documentos eleitorais (TSE, relatórios)
- [ ] Memória de longo prazo para agentes

### n8n

- [ ] Primeiro workflow (trigger → ação)
- [ ] n8n + Claude via HTTP Request
- [ ] Agente de IA dentro do n8n com memória
- [ ] Automação Google Sheets + Claude
- [ ] Automação Gmail + Claude
- [ ] Workflow multi-agente no n8n
- [ ] RAG básico dentro do n8n

---

## Fase 3 — IA Criativa como produto cruzado (paralelo)

Em vez de fazer os 12 meses do curso criativo completo, só o que vira serviço vendável via n8n:

- [ ] Prompt avançado de imagem (Midjourney: `--sref`, `--cref`)
- [ ] Testar Kling AI / Runway para 2-3 clipes curtos
- [ ] Construir 1 pipeline n8n: briefing → imagem (Ideogram/Leonardo) → copy (Claude) → post formatado
- [ ] Adicionar ElevenLabs para narração automática em 1 vídeo de teste
- [ ] Montar 1 case "automação de produção de conteúdo com IA"

---

## Fase 4 — Implementação empresarial (depois das fases 0-2)

- [ ] Template de diagnóstico de maturidade de IA
- [ ] Proposta técnica com estimativa de ROI
- [ ] Diagnóstico no Podemos (o que pode ser automatizado)
- [ ] LGPD aplicada a projetos de IA + boas práticas de segurança
- [ ] One-pager de serviços de consultoria em IA

---

## Fase 5 — Autoridade contínua

- [ ] 1 post técnico por semana no LinkedIn
- [ ] Entrar em comunidades: n8n Brasil, Claude Users, Discord de automação
- [ ] Fechar primeiro cliente de consultoria
- [ ] Criar template de agente/workflow como produto digital

---

## Checkpoints de validação (a cada 30 dias)

- Tenho algo *novo* publicado (GitHub, LinkedIn, portfólio)?
- Esse algo prova uma habilidade que uma vaga de AI Engineer pede?
- Estou gastando tempo estudando coisa que ainda não virou nada concreto?

> Se a resposta da 3ª for "sim" por mais de 2 semanas — pausa o estudo e vai pro próximo item de portfólio.
