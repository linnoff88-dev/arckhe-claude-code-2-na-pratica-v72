# Claude Code 2.0 na prêÂ¡tica ê¢â¬â curso ARCKHê v7.2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ê°Å¸â¡Â§ê°Å¸â¡Â· [Curso em portuguêÂªs](https://linnoff88-dev.github.io/ êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](https://linnoff88-dev.github.io/ êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](https://linnoff88-dev.github.io/

As novidades do Claude Code para quem nêÂ£o programa, em sete aulas curtas, abertas e gratuitas. Cada novidade êÂ© testada num trabalho real (o curso de planilhas da Carla), com prompt pronto, prêÂ¡tica com "pronto quando" e teste comentado. O curso diz o que êÂ© prêÂ©via, beta ou sêÂ³ nos EUA. "Claude Code 2.0" êÂ© o apelido das versêÂµes 2.1.x.

**Guia de consulta das 13 novidades (com os prompts):** https://linnoff88-dev.github.io/

| # | Aula | PêÂ¡gina |
|---|---|---|
| 1 | O mapa: o que mudou e o que jêÂ¡ dêÂ¡ para usar | `aulas/mapa/` |
| 2 | Organizar: seêÂ§êÂµes, side chat e split view | `aulas/organizar/` |
| 3 | Ajudantes: subagentes | `aulas/ajudantes/` |
| 4 | Apps e sites: computer use e navegador embutido | `aulas/apps-e-sites/` |
| 5 | Longe do computador: Remote Control, Projects e Duet | `aulas/longe/` |
| 6 | Entregar: Slides, Design, Dashboards e Docs | `aulas/entregar/` |
| 7 | Personalizar: comandos de barra e mods | `aulas/personalizar/` |

## O processo, do inêÂ­cio ao fim

Legenda: ê°Å¸Â§Â  sessêÂ£o com o Nei êÂ· ê¢Å¡â¢ê¯Â¸Â script/timer êÂ· ê°Å¸Â¤â `claude -p` / subagente

1. ê°Å¸Â§Â  Pedido do Nei + fatos conferidos na documentaêÂ§êÂ£o oficial (`longrun/2026-11-01-claude-code-2/FATOS.md` no repo wifi).
2. ê¢Å¡â¢ê¯Â¸Â Criar o curso: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/claude-code-2-na-pratica-v72 "Claude Code 2.0 na prêÂ¡tica"`.
3. ê°Å¸Â¤â Plano das aulas (`longrun/.../PLANO-AULAS.md`) ê¢â â 3 redatores escrevem `conteudo/pt/aulas/*.json` (brief `longrun/.../BRIEF-AULAS.md`).
4. ê¢Å¡â¢ê¯Â¸Â Imagens pelo Codex, uma por vez: `bash longrun/2026-11-01-claude-code-2/tools/imagens_curso.sh` (capa + fotos de abertura); capas EN/ES editando a original.
5. ê¢Å¡â¢ê¯Â¸Â PortêÂ£o: `python3 gerar.py && python3 validar.py --links && node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`
6. ê°Å¸Â¤â Revisor independente (agente novo, persona do pêÂºblico) ê¢â â corrigir ê¢â â revisar de novo; notas em `~/projetos/wifi/scripts/revisor-nota.py`.
7. ê¢Å¡â¢ê¯Â¸Â EN/ES: `python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es` (tradutor central) ê¢â â `gerar.py --lang en|es` ê¢â â `validar.py --lang en|es` ê¢â â conferir rêÂ³tulos dos conferidores.
8. ê¢Å¡â¢ê¯Â¸Â Publicar: commit (autor linnoff88-dev) + `gh repo create linnoff88-dev/claude-code-2-na-pratica-v72 --public --source . --push` + GitHub Pages da raiz.
9. ê°Å¸Â§Â  VêÂ­deos (explicavideo 16:9 + 9:16 e rtex 9:16) ê¢â â lives4, ARCKHê.CCODE, metritds; portal ARCKHê AI (skill `atualiza-portal`).

ConteêÂºdo aberto e gratuito êÂ· [ARCKHê AI](https://ARCKHê AI)

## Mais no ARCKHê AI

- [Ficha completa deste curso](https://www.ARCKHê AI/cursos/389-claude-code-2-0-na-pratica-as-novidades-do-claude-code-para-quem-nao-programa/)
- [Guia: como aprender inteligêÂªncia artificial](https://www.ARCKHê AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHê AI/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>