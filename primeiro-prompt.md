# O primeiro prompt

É a primeira mensagem que você manda para o Claude, depois de abrir a trilha no VS Code. Copie,
cole no Claude e mande:

```text
Oi, Claude. Sou trainee do squad do Ludi e vou começar a Trilha do Claude, que está em
https://github.com/contasinovacao-dev/trilha-claude. Quero sair dela com você sabendo quem eu sou,
o que eu faço no NI e qual é o meu objetivo no treinamento, e com o meu espaço de trabalho montado.
Me entrevista aos poucos, uma pergunta por vez, e vai guardando o que eu responder.
```

## O que acontece depois

O Claude te entrevista em cinco blocos, uma pergunta por vez:

1. você;
2. o NI;
3. a sua semana, com um print da sua grade horária (a do Júpiter serve) ou da sua agenda;
4. como trabalhar com você;
5. o seu objetivo no NI.

São umas quinze perguntas curtas, quase todas de clicar, e dá para pular qualquer uma. O foco é o
NI: da faculdade, ele só precisa do print. Se a conversa cair no meio, ele retoma de onde parou.

Depois, ele monta a pasta onde você vai trabalhar com ele, abre a pasta para você ver e explica, sem
palavra técnica, o que montou e por quê.

## Para onde vai o que você contar

| O que você conta | Arquivo | Quem vê |
| --- | --- | --- |
| quem você é, o objetivo em uma linha, como trabalhar com você | `~/.claude/CLAUDE.md` | só você, no seu computador |
| o card, a dupla e em que você quer melhorar | `~/NI/treinamento/CLAUDE.md` | só você; da etapa 4 em diante, também no seu GitHub (repositório privado) |
| por que entrou no NI, a sua semana, as outras atividades | `~/NI/eu/sobre-mim.md` | idem |
| as matérias, tiradas do print (a imagem não fica guardada) | `~/NI/faculdade/CLAUDE.md` | idem |
| o objetivo, com medida, prazo e próximo passo | `~/NI/eu/objetivos.md` | idem |
| nome, dupla, computador, usuário do GitHub e, se você quiser, o objetivo | `trainees/<pasta>/perfil.md` | o squad e o Bruno, nesta trilha |
