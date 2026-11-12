<!--
Modelo do ~/NI/CLAUDE.md, preenchido na etapa 4.
-->

# O espaço de {apelido}

Pasta de trabalho de {nome} no treinamento do NI. Quem ele é e como trabalhar com ele está em
`~/.claude/CLAUDE.md`.

## Projetos

| Projeto | Pasta | O que é |
| --- | --- | --- |
| Trilha do Claude | `trilha-claude/` | a trilha de configuração; repositório do time, branch `trilha/{pasta}` |
| {Projeto} | `{pasta-do-projeto}/` | {uma linha} |
| {Projeto} | `{pasta-do-projeto}/` | {uma linha} |

Pedido que não é de nenhum projeto: atenda sem criar pasta. Projeto novo: pergunte o nome, crie a
pasta com um `CLAUDE.md` a partir de `trilha-claude/modelos/claude-do-projeto.md` e acrescente uma
linha nesta tabela.

## Onde guardar

- Cada coisa na pasta do projeto dela. Nada solto em `~/NI`.
- Arquivo que você (Claude) escrever começa com `(C) ` no nome. Assim eu sei o que escrevi e o que
  você escreveu.
- Rascunho que não vou usar de novo não vira arquivo.

## Trilha em andamento

No começo de cada conversa, leia `trilha-claude/CLAUDE.md` e siga de onde parei. Para salvar a
trilha, siga `trilha-claude/.claude/skills/salvar/SKILL.md`. Os comandos git da trilha rodam com
`git -C trilha-claude`. Esta seção sai na etapa 7.
