# Claude Code 2.0 na prÃ¡tica â€” curso INEMA v7.2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ðŸ‡§ðŸ‡· [Curso em portuguÃªs](https://inematds.github.io/claude-code-2-na-pratica-v72/) Â· ðŸ‡ºðŸ‡¸ [English](https://inematds.github.io/claude-code-2-na-pratica-v72/en/) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](https://inematds.github.io/claude-code-2-na-pratica-v72/es/)**

As novidades do Claude Code para quem nÃ£o programa, em sete aulas curtas, abertas e gratuitas. Cada novidade Ã© testada num trabalho real (o curso de planilhas da Carla), com prompt pronto, prÃ¡tica com "pronto quando" e teste comentado. O curso diz o que Ã© prÃ©via, beta ou sÃ³ nos EUA. "Claude Code 2.0" Ã© o apelido das versÃµes 2.1.x.

**Guia de consulta das 13 novidades (com os prompts):** https://inematds.github.io/claude-code-2/guia/

| # | Aula | PÃ¡gina |
|---|---|---|
| 1 | O mapa: o que mudou e o que jÃ¡ dÃ¡ para usar | `aulas/mapa/` |
| 2 | Organizar: seÃ§Ãµes, side chat e split view | `aulas/organizar/` |
| 3 | Ajudantes: subagentes | `aulas/ajudantes/` |
| 4 | Apps e sites: computer use e navegador embutido | `aulas/apps-e-sites/` |
| 5 | Longe do computador: Remote Control, Projects e Duet | `aulas/longe/` |
| 6 | Entregar: Slides, Design, Dashboards e Docs | `aulas/entregar/` |
| 7 | Personalizar: comandos de barra e mods | `aulas/personalizar/` |

## O processo, do inÃ­cio ao fim

Legenda: ðŸ§  sessÃ£o com o Nei Â· âš™ï¸ script/timer Â· ðŸ¤– `claude -p` / subagente

1. ðŸ§  Pedido do Nei + fatos conferidos na documentaÃ§Ã£o oficial (`longrun/2026-11-01-claude-code-2/FATOS.md` no repo wifi).
2. âš™ï¸ Criar o curso: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/claude-code-2-na-pratica-v72 "Claude Code 2.0 na prÃ¡tica"`.
3. ðŸ¤– Plano das aulas (`longrun/.../PLANO-AULAS.md`) â†’ 3 redatores escrevem `conteudo/pt/aulas/*.json` (brief `longrun/.../BRIEF-AULAS.md`).
4. âš™ï¸ Imagens pelo Codex, uma por vez: `bash longrun/2026-11-01-claude-code-2/tools/imagens_curso.sh` (capa + fotos de abertura); capas EN/ES editando a original.
5. âš™ï¸ PortÃ£o: `python3 gerar.py && python3 validar.py --links && node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`
6. ðŸ¤– Revisor independente (agente novo, persona do pÃºblico) â†’ corrigir â†’ revisar de novo; notas em `~/projetos/wifi/scripts/revisor-nota.py`.
7. âš™ï¸ EN/ES: `python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es` (tradutor central) â†’ `gerar.py --lang en|es` â†’ `validar.py --lang en|es` â†’ conferir rÃ³tulos dos conferidores.
8. âš™ï¸ Publicar: commit (autor inematds) + `gh repo create inematds/claude-code-2-na-pratica-v72 --public --source . --push` + GitHub Pages da raiz.
9. ðŸ§  VÃ­deos (explicavideo 16:9 + 9:16 e rtex 9:16) â†’ lives4, INEMA.CCODE, metritds; portal inema.club (skill `atualiza-portal`).

ConteÃºdo aberto e gratuito Â· [INEMA.CLUB](https://inema.club)

## Mais no INEMA.CLUB

- [Ficha completa deste curso](https://www.inema.club/cursos/389-claude-code-2-0-na-pratica-as-novidades-do-claude-code-para-quem-nao-programa/)
- [Guia: como aprender inteligÃªncia artificial](https://www.inema.club/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.inema.club/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>