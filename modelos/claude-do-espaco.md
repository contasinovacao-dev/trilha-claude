<!--
Modelo do ~/NI/CLAUDE.md, preenchido na etapa 4.
-->

# O espaço de {apelido}

Pasta de trabalho de {nome} no treinamento do NI, guardada no repositório privado `espaco-ni`, no
GitHub de {apelido}. Quem é e como trabalhar junto está em `~/.claude/CLAUDE.md`; a vida fora do NI,
em `eu/sobre-mim.md`; os objetivos, em `eu/objetivos.md`.

## Projetos

| Projeto | Pasta | O que é | Objetivo que move |
| --- | --- | --- | --- |
| Trilha do Claude | `trilha-claude/` | a trilha de configuração; repositório do time, branch `trilha/{pasta}` | treinamento |
| {Projeto} | `{pasta-do-projeto}/` | {uma linha} | {1, 2 ou 3 de `eu/objetivos.md`} |
| {Projeto} | `{pasta-do-projeto}/` | {uma linha} | {1, 2 ou 3} |

Pedido que não é de nenhum projeto: atenda sem criar pasta. Projeto novo: pergunte o nome, crie a
pasta com um `CLAUDE.md` a partir de `trilha-claude/modelos/claude-do-projeto.md` e acrescente uma
linha nesta tabela.

## Onde guardar

- Cada coisa na pasta do projeto. Nada solto na raiz do espaço.
- Arquivo que você (Claude) escrever começa com `(C) ` no nome. Assim sei o que escrevi e o que
  você escreveu.
- Rascunho que não vou usar de novo não vira arquivo.
- Ata de entrevista só com o cargo e a organização, nunca com nome, telefone ou e-mail.

## Skills

Ficam em `.claude/skills/` e vão para o GitHub com o resto:

- de uso: `/discutir`, `/ensaiar`, `/revisar`, `/explicar`, `/pesquisar` e `/ata`;
- do espaço: `/salvar` (guarda o espaço no GitHub) e `/objetivos` (revisão da semana);
- as minhas: {a da etapa 6, quando existir}.

Skill nova: uma pasta em `.claude/skills/<nome>/`, a partir de `trilha-claude/modelos/skill.md`.

## Regras do espaço

- No fim de uma conversa em que algum arquivo mudou, ofereça `/salvar`.
- Quando o pedido for de prioridade ou da semana, ou quando eu disser que estou perdido, ofereça
  `/objetivos`.
- O que está aqui é meu. Nada desta pasta vai para a trilha nem para outro repositório sem eu pedir.
- O `espaco-ni` é privado e continua privado.
- `eu/claude-do-computador.md` é a cópia do `~/.claude/CLAUDE.md`. A skill `/salvar` mantém os dois
  iguais.

## Trilha em andamento

No começo de cada conversa, leia `trilha-claude/CLAUDE.md` e siga de onde parei. Os comandos git da
trilha rodam com `git -C trilha-claude`. A skill `/salvar` deste espaço salva a trilha também,
enquanto esta seção existir. Esta seção sai na etapa 7.
