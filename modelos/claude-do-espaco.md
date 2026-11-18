<!--
Modelo do ~/NI/CLAUDE.md, criado pelo Claude no passo 7 da etapa 1, depois da entrevista.
-->

# O espaço de {apelido}

Pasta de trabalho de {nome} com o Claude no treinamento do NI. Montada na etapa 1 da Trilha do
Claude; a partir da etapa 4, guardada no repositório privado `espaco-ni`, no GitHub de {apelido}.
Quem é e como trabalhar junto está em `~/.claude/CLAUDE.md`; a semana e as outras atividades, em
`eu/sobre-mim.md`; o objetivo no NI, em `eu/objetivos.md`.

O foco é o NI. A faculdade e o resto entram como apoio.

## Pastas

| Pasta | O que é |
| --- | --- |
| `treinamento/` | o card de agora, a dupla, as entrevistas e o que sair do treinamento |
| `faculdade/` | as matérias do semestre, tiradas do print da grade (só se ela mandou) |
| `eu/` | sobre mim, o objetivo e a cópia do `~/.claude/CLAUDE.md` |
| `trilha-claude/` | a Trilha do Claude; repositório do time, branch `trilha/{pasta}` |

Pedido que não é de nenhuma pasta: atenda sem criar pasta. Pasta nova: pergunte o nome, crie com um
`CLAUDE.md` a partir de `trilha-claude/modelos/claude-do-projeto.md` e acrescente uma linha nesta
tabela.

## Onde guardar

- Cada coisa na sua pasta. Nada solto na raiz do espaço.
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
- Quando eu disser que algo mudou (card, dupla, grade), atualize o arquivo certo e me diga qual.
- O que está aqui é meu. Nada desta pasta vai para a trilha nem para outro repositório sem eu pedir.
- O `espaco-ni` é privado e continua privado.
- `eu/claude-do-computador.md` é a cópia do `~/.claude/CLAUDE.md`. A skill `/salvar` mantém os dois
  iguais.

## Trilha em andamento

Enquanto esta seção existir, siga a trilha de onde parei:

- Aberto em `~/NI`: leia `trilha-claude/CLAUDE.md` no começo de cada conversa e rode o git da trilha
  com `git -C trilha-claude`. A skill `/salvar` deste espaço salva a trilha também.
- Aberto em `~/NI/trilha-claude` (etapas 1 a 4): siga o `CLAUDE.md` de lá. Dentro da trilha valem
  as regras dela, e não as deste espaço.

Esta seção sai na etapa 7.
