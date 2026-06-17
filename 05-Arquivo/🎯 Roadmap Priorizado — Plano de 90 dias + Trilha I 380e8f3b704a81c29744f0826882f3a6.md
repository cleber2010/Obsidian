# 🎯 Roadmap Priorizado — Plano de 90 dias + Trilha Integrada

> Versão priorizada do roadmap, pensada para gerar **portfólio e oportunidades reais em até 90 dias**, sem abandonar o resto — só reordenando. As duas trilhas (Engenharia de IA e IA Criativa) foram fundidas onde fazia sentido.
> 

---

[Anotações claude](Anota%C3%A7%C3%B5es%20claude%2037be8f3b704a8092934ecda23fe12e46.md)

# 🚀 Fase 0 — Sprint de Portfólio (Dias 1–30)

> Objetivo: ter pelo menos 1 case publicado e 1 agente funcionando rodando antes de qualquer curso novo. Isso é o que recrutador/cliente vê primeiro.
> 
- [ ]  Documentar o projeto de dados eleitorais do Podemos como case (problema → solução → resultado, com números)
- [ ]  Documentar as automações Python da Matrix Energia como case (Salesforce/SharePoint)
- [ ]  Criar repositório GitHub organizado com esses 2 projetos (README bom, sem dados sensíveis)
- [ ]  Construir um agente simples: Claude API + tool use + RAG básico sobre dados eleitorais (TSE/municípios) — vira o 3º case
- [ ]  Publicar 1 post técnico no LinkedIn sobre o case eleitoral ("como usei IA para automatizar X municípios")
- [ ]  Atualizar perfil do Upwork com esses 3 cases

---

# 🧠 Fase 1 — Fundamentos técnicos essenciais (Dias 30–60)

## Claude / API Anthropic (itens que faltam do roadmap original)

- [x]  Praticar artifacts para gerar código, docs e visualizações
- [x]  Criar projeto no [Claude.ai](http://Claude.ai) para Podemos/dados eleitorais
- [x]  Criar projeto no [Claude.ai](http://Claude.ai) para Automação & Freelance
- [x]  Configurar memórias e instruções personalizadas
- [x]  Criar conta na Anthropic + primeira chamada via API
- [x]  Implementar conversa multi-turn + streaming
- [x]  Tratar erros HTTP (429, 529, 400) + variáveis de ambiente

## Infra básica (NOVO — exigido em quase toda vaga de AI Engineer)

- [ ]  Docker: conceitos básicos, criar um Dockerfile simples para uma API Python
- [ ]  FastAPI: criar uma API mínima que chama a Claude API
- [ ]  Deploy simples (Railway ou Render) — ter 1 projeto online com link público

---

# ⚙️ Fase 2 — Orquestração avançada (Dias 60–90)

## Tool use e agentes

- [ ]  Loop completo tool_use → tool_result → resposta final
- [ ]  Agente com acesso a arquivos locais
- [ ]  Agente com acesso a API externa (TSE, IBGE)

## MCP

- [ ]  Entender MCP e configurar Claude Desktop
- [ ]  Conectar MCP ao Google Drive, Gmail, Calendar
- [ ]  Testar integração MCP + n8n

## Multi-agente (ATUALIZADO — priorizar sobre LangChain genérico)

- [ ]  Estudar LangGraph (orquestração de agentes com estado/grafo) — referência de mercado atual
- [ ]  Estudar CrewAI como alternativa mais simples para multi-agentes
- [ ]  Avaliar se faz sentido usar LangChain só para RAG (ele ainda é bom pra isso)

## Avaliação e observabilidade (NOVO — diferencial em entrevista)

- [ ]  Entender o conceito de "LLM eval": como medir se um agente está funcionando bem
- [ ]  Testar LangSmith ou logging próprio para rastrear chamadas e custos
- [ ]  Criar um dataset pequeno de testes ("golden set") pro seu agente eleitoral

## RAG e memória

- [ ]  Embeddings e busca semântica
- [ ]  Pinecone ou Qdrant
- [ ]  RAG aplicado em documentos eleitorais (TSE, relatórios)
- [ ]  Memória de longo prazo para agentes

## n8n

- [ ]  Primeiro workflow (trigger → ação)
- [ ]  n8n + Claude via HTTP Request
- [ ]  Agente de IA dentro do n8n com memória
- [ ]  Automação Google Sheets + Claude
- [ ]  Automação Gmail + Claude
- [ ]  Workflow multi-agente no n8n
- [ ]  RAG básico dentro do n8n

---

# 🎬 Fase 3 — IA Criativa como produto cruzado (paralelo, não trilha separada)

> Em vez de fazer os 12 meses do curso criativo completo, pegue só o que vira **serviço vendável via n8n** — é onde as duas trilhas se cruzam.
> 
- [ ]  Aprender prompt avançado de imagem (Midjourney: `--sref`, `--cref`, parâmetros) — só o essencial
- [ ]  Testar Kling AI / Runway para 2-3 clipes curtos (entender o fluxo, não dominar tudo)
- [ ]  Construir 1 pipeline n8n: briefing de texto → imagem gerada (Ideogram/Leonardo) → copy (Claude) → post formatado
- [ ]  Adicionar ElevenLabs para narração automática em 1 vídeo de teste
- [ ]  Montar 1 case "automação de produção de conteúdo com IA" — isso vira oferta tanto pra Upwork quanto pra agências pequenas

📌 **O resto da trilha criativa (semestres 1-4, TCC, fundamentos de composição/direção)** fica guardado como referência — útil se você decidir migrar 100% pra área criativa depois, mas não é prioridade pra conseguir vaga/freela agora.

---

# 🏢 Fase 4 — Implementação empresarial (depois da Fase 0-2 prontas)

- [ ]  Template de diagnóstico de maturidade de IA
- [ ]  Proposta técnica com estimativa de ROI
- [ ]  Diagnóstico no Podemos (o que pode ser automatizado)
- [ ]  LGPD aplicada a projetos de IA + boas práticas de segurança
- [ ]  One-pager de serviços de consultoria em IA

---

# 🚀 Fase 5 — Autoridade contínua

- [ ]  1 post técnico por semana no LinkedIn
- [ ]  Entrar em comunidades: n8n Brasil, Claude Users, Discord de automação
- [ ]  Fechar primeiro cliente de consultoria
- [ ]  Criar template de agente/workflow como produto digital

---

# ✅ Checkpoints de validação

A cada 30 dias, pergunte:

- Tenho algo *novo* publicado (GitHub, LinkedIn, portfólio)?
- Esse algo prova uma habilidade que uma vaga de AI Engineer pede?
- Estou gastando tempo estudando coisa que ainda não virou nada concreto?

Se a resposta da 3ª for "sim" por mais de 2 semanas — pausa o estudo e vai pro próximo item de portfólio.