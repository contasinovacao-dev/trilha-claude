<!--
Modelo do ~/NI/README.md, copiado na etapa 4. É o que aparece na página do espaco-ni no GitHub.
-->

# O espaço de {apelido} no NI

O meu espaço de trabalho no treinamento do NI, com o Claude. Repositório privado: só eu vejo.

| Caminho | O que é |
| --- | --- |
| `CLAUDE.md` | o mapa que o Claude lê ao abrir esta pasta: projetos, onde guardar cada coisa e regras |
| `eu/` | `sobre-mim.md`, `objetivos.md` e `claude-do-computador.md`, a cópia do `~/.claude/CLAUDE.md` |
| `.claude/skills/` | as minhas skills: as seis de uso, `salvar`, `objetivos` e as que eu criar |
| `.claude/settings.json` | o que o Claude pode e não pode fazer aqui |
| `<projeto>/` | uma pasta por projeto, cada uma com o seu `CLAUDE.md` |

A trilha (`trilha-claude/`) fica dentro de `~/NI`, mas é outro repositório, do time. O `.gitignore`
a deixa de fora deste.

## Num computador novo

1. Instale o VS Code, o Git, o GitHub CLI (`gh`) e a extensão do Claude Code, como no README da
   trilha.
2. No terminal: `gh auth login --web --git-protocol https`, depois `gh repo clone espaco-ni ~/NI`.
3. Abra `~/NI` no VS Code, abra o Claude e peça: "Copia `eu/claude-do-computador.md` para
   `~/.claude/CLAUDE.md`."
4. Se ainda precisar da trilha: `gh repo clone contasinovacao-dev/trilha-claude ~/NI/trilha-claude`.
