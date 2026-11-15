# O primeiro prompt

É a primeira mensagem que você manda para o Claude, depois de abrir a trilha no VS Code. Copie,
cole no Claude e mande:

```text
Oi, Claude. Sou trainee do squad do Ludi e vou começar a Trilha do Claude, que está em
https://github.com/contasinovacao-dev/trilha-claude. Quero sair dela com você sabendo quem eu sou, o que eu faço dentro e fora do NI e quais são os meus objetivos, e com o
meu espaço de trabalho guardado no meu GitHub. Me entrevista aos poucos, uma pergunta por vez, e
vai guardando o que eu responder.
```

## O que acontece depois

O Claude te entrevista em seis blocos, uma pergunta por vez:

1. quem você é;
2. você e o computador;
3. o NI;
4. a sua vida fora do NI;
5. como trabalhar com você;
6. os seus objetivos.

São umas vinte perguntas curtas, e dá para pular qualquer uma. No fim de cada bloco, ele guarda as
respostas no arquivo certo e te diz o que guardou. Se você quiser mudar alguma coisa, é só falar. Se
a conversa cair no meio, ele retoma do bloco seguinte.

## Para onde vai o que você contar

| O que você conta | Arquivo | Quem vê |
| --- | --- | --- |
| quem você é, os objetivos em uma linha, como trabalhar com você | `~/.claude/CLAUDE.md` | só você, no seu computador |
| a vida fora do NI, a sua semana, o que você gosta | `~/NI/eu/sobre-mim.md` | só você, no seu GitHub (repositório privado) |
| os objetivos, com medida, prazo e próximo passo | `~/NI/eu/objetivos.md` | só você, no seu GitHub (repositório privado) |
| nome, dupla, computador, usuário do GitHub e, se você quiser, o objetivo no treinamento | `trainees/<pasta>/perfil.md` | o squad e o Bruno, nesta trilha |
