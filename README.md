# O seu Jarvis — degrau 2 de "Do chat ao agente" (INEMA Learning v7.2)

Curso completo do degrau 2 da formação [Do chat ao agente](https://inematds.github.io/do-chat-ao-agente-v72/): um assistente pessoal com a memória e a personalidade que você definir, usando o [INTELECTO](https://github.com/inematds/intelecto) como exemplo. Oito aulas: as sete peças de um agente, a identidade em quatro arquivos, o bot no Telegram, construir com o Claude Code ou o Codex e provar com testes, memória, nuvem ou local, ferramentas e cofre, e uma rotina de verdade com o assistente no ar.

**Abrir o curso:** https://inematds.github.io/do-chat-ao-agente-jarvis-v72/

## Como funciona

| Arquivo | O que é |
|---|---|
| `conteudo/pt/curso.json` | nome, vídeos, página inicial e textos da interface |
| `conteudo/pt/aulas/*.json` | uma aula por arquivo (diagrama, passos, código, simulação, prática, vídeo, quiz, resumo, links) |
| `gerar.py` | monta `index.html` e `aulas/<slug>/index.html` |
| `validar.py` | portão de qualidade (`--links` confere os links externos) |
| `assets/` | CSS, JS, imagens e legendas |

```bash
python3 gerar.py && python3 validar.py --links
node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .
```

HTML estático, sem build e sem backend. O progresso fica só no navegador de quem estuda.

Vídeos já publicados: [as 7 peças](https://inematds.github.io/intelecto-estrutura/videos/), [instale o seu Jarvis](https://inematds.github.io/intelecto-instalacao/videos/) e a série [jornada-agentes](https://github.com/inematds/jornada-agentes) (release `video-v2.0.0`). Exercícios originais em `jornada-agentes/exercicios/02-jarvis.md`.

Conteúdo aberto e gratuito · [INEMA.CLUB](https://inema.club)

## Mais no INEMA.CLUB

- [Ficha completa deste curso](https://www.inema.club/cursos/325-do-chat-ao-agente-degrau-2-o-seu-jarvis-com-memoria-no-telegram-intelecto/)
- [Guia: como aprender inteligência artificial](https://www.inema.club/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.inema.club/cursos/)
