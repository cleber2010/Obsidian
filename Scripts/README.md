# Scripts

## youtube_to_obsidian.py
Pega um vídeo do YouTube, extrai a transcrição, resume com o Claude e salva uma nota markdown em `04-Recursos/Videos/`, já com frontmatter e link pro MOC.

### Setup (uma vez)
```bash
pip install -r requirements.txt
export ANTHROPIC_API_KEY="sk-ant-..."   # põe no teu .zshrc/.bashrc pra não repetir
```

### Uso
```bash
python youtube_to_obsidian.py "https://www.youtube.com/watch?v=XXXX"

# escolhendo idioma e MOC de destino:
python youtube_to_obsidian.py "https://youtu.be/XXXX" --lang pt --lang en --moc "_MOC-Automacao"
```

### Variáveis de ambiente
- `ANTHROPIC_API_KEY` (obrigatória)
- `CLAUDE_MODEL` (opcional, default `claude-sonnet-4-6`; troca pra `claude-haiku-4-5-20251001` se quiser mais barato)
- `OBSIDIAN_VAULT` (opcional, default = pasta-pai de Scripts/)

### Limitações honestas
- Só funciona em vídeos que TÊM legenda/transcrição (manual ou auto-gerada). Vídeo sem legenda nenhuma não dá.
- Legenda auto-gerada vem sem pontuação e com erros — o resumo do Claude limpa bem, mas não é mágica.
- O oEmbed pega título/canal; se o vídeo for privado/removido, cai pra "sem título".

### Atalho via Claude Code
Com o `CLAUDE.md` na raiz do vault, é só dizer no Claude Code:
`nota de vídeo https://youtu.be/XXXX` — ele roda o script e linka a nota no MOC certo.
