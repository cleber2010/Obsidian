# Segundo Cérebro — Sistema PARA

Vault pra substituir o Notion e organizar trabalho (Podemos), estudos (SPTech + roadmap de IA) e vida pessoal (treino, projetos, interesses) em um lugar só, em markdown puro.

## Método: PARA

- **Projetos** (`02-Projetos`): tem objetivo e prazo. Ex: Totem de Autoatendimento, Roadmap de IA.
- **Áreas** (`03-Areas`): responsabilidade contínua, sem fim definido. Ex: Trabalho na Podemos, Estudos, Saúde.
- **Recursos** (`04-Recursos`): material de referência por tema, organizado como MOC (Map of Content) — cada `_MOC-*.md` é um índice que linka pra notas atômicas que você cria conforme estuda (uma nota = uma ideia, usando o template `Nota-Atomica`).
- **Arquivo** (`05-Arquivo`): o que terminou ou ficou inativo. Não deleta, só move pra cá.

Além disso:
- **00-Inbox**: captura rápida, sem pensar em organização. Processa 1x por semana.
- **01-Diario**: uma nota por dia (`AAAA-MM-DD.md`), criada com o template.
- **Templates**: modelo pra cada tipo de nota.

## Plugins pra instalar (Configurações → Plugins da comunidade)

1. **Dataview** — consulta notas via query, tipo SQL. Já deixei queries prontas em algumas Áreas (ex: listar projetos relacionados automaticamente).
2. **Templater** — templates dinâmicos com data automática. Configura a pasta `Templates` em Templater → Template folder location, e define `Daily-Note.md` como template padrão pra notas novas em `01-Diario`.
3. **Tasks** — tarefas com data, recorrência, prioridade. Combinado com Dataview, dá pra fazer uma query puxando tarefas pendentes de qualquer nota do vault.
4. **Calendar** — navegação visual nas daily notes.
5. **Obsidian Git** (opcional, mas faz sentido pro seu perfil) — commita e sincroniza o vault automaticamente via Git.
6. **Kanban** (opcional) — se sentir falta da visão de board do Notion, cria um board por projeto.

## Sincronização entre dispositivos

Pro dia a dia funcionar, você vai querer isso no celular também. Opções:
- **Obsidian Sync** (pago, oficial, mais simples de configurar)
- **iCloud / Google Drive** (grátis, mas pode dar conflito se editar nos dois ao mesmo tempo sem internet)
- **Syncthing** ou **Obsidian Git** (grátis, mais hands-on, combina com seu perfil técnico)

## Migrando conteúdo do Notion

- Notion exporta em Markdown (Settings → Export → Markdown & CSV). Os arquivos vêm com IDs feios no nome — exporta, abre, e copia o conteúdo relevante pra dentro das notas certas aqui, em vez de importar tudo cru de uma vez.
- **Databases do Notion não migram 1:1.** Cada "view" de banco de dados vira, aqui, uma pasta de notas + uma query de Dataview. Por isso os Recursos já vêm como MOC em vez de tabela.
- Toggle lists viram bullets aninhados — perdem o collapse nativo do Notion, mas o Obsidian tem outline fold (seta ao lado do bullet).
- Ordem de migração sugerida: (1) rotina diária, pra criar o hábito primeiro; (2) projetos ativos agora (Totem, Bounty Hunter, freelance, roadmap de IA); (3) o resto, sem pressa.

## Como começar

1. Instala os plugins acima.
2. Abre essa pasta no Obsidian como vault ("Open folder as vault").
3. Configura o Templater pra usar a pasta `Templates`.
4. Usa só Inbox + Diário por uns dias antes de se preocupar com o resto — o sistema só funciona se a captura for rápida.
5. Vai migrando os projetos ativos do Notion, um por vez.

Já deixei exemplos preenchidos com o que você já tem rodando (Podemos, SPTech, roadmap de IA, projetos de portfólio) — é só ajustar e continuar daí.

---

## Camada de IA (adicionada)

Este vault agora tem duas peças pra rodar com IA:

- **`CLAUDE.md`** (raiz) — instruções que transformam o **Claude Code** no operador do vault. Abra o terminal na pasta do vault, rode `claude`, e mande comandos tipo "processa a inbox", "o que eu sei sobre RAG", "resume meu dia", "nota de vídeo <url>".
- **`Scripts/youtube_to_obsidian.py`** — pega um vídeo do YouTube, transcreve, resume com o Claude e salva nota markdown em `04-Recursos/Videos/`. Veja `Scripts/README.md`.

Plugins de IA recomendados (Configurações → Plugins da comunidade):
- **Copilot** (brevilabs) — chat com o vault + suporte nativo a YouTube e web. Caminho zero-build pra resumir vídeo dentro do Obsidian.
- **Smart Connections** — busca semântica local (sem API key) que sugere notas relacionadas enquanto você escreve.
- **Bases** (core do Obsidian) — views de tabela/database, o mais perto das databases do Notion.
