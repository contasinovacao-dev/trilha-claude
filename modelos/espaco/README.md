<!--
Modelo do ~/NI/README.md, criado no passo 7 da etapa 1. É a explicação, sem palavra técnica, do que
o Claude montou e por quê, e o que aparece na página do espaco-ni no GitHub. Escrito na voz dela.
Deixar só as pastas que existem de fato.
-->

# O espaço de {apelido} no NI

Esta é a pasta onde eu trabalho com o Claude no treinamento do NI. O Claude montou a pasta na
Trilha do Claude, a partir de uma conversa comigo. Só eu vejo.

## Por que ela existe

O Claude não lembra de nada de uma conversa para outra. Toda conversa começa do zero, e ele lê as
anotações desta pasta para saber quem eu sou, em que estou trabalhando e como gosto de trabalhar.
Sem elas, eu teria de explicar tudo de novo a cada conversa.

Exemplo: se eu escrever "me ajuda a preparar a entrevista de quinta", ele já sabe qual é o meu
card, quem é a minha dupla e em que eu quero melhorar. Eu só falo da entrevista.

## O que tem aqui

| Pasta | O que guarda |
| --- | --- |
| `treinamento` | o card, a dupla e o que eu fizer no treinamento: entrevistas, atas, análises |
| `faculdade` | as matérias do semestre, tiradas do print da minha grade |
| `eu` | quem eu sou, a minha semana e o meu objetivo no NI |
| `trilha-claude` | a trilha; fica aqui dentro, mas é do time |

As pastas de trabalho têm um arquivo chamado `CLAUDE.md`, com as anotações que o Claude lê quando
eu trabalho ali. Uma pasta escondida, `.claude`, guarda os comandos prontos (como `/ensaiar`) e as
regras do que ele pode fazer aqui.

O resumo de quem eu sou fica num arquivo fora desta pasta, que o Claude lê em qualquer lugar do
computador. A cópia dele está em `eu/claude-do-computador.md`.

## No dia a dia

- Abro esta pasta no VS Code e converso com o Claude. Não preciso abrir nem editar as anotações.
- Mudou alguma coisa (card novo, grade nova)? Falo: "mudei de card, atualiza".
- O Claude fez algo de que eu não gostei? Falo: "não faz mais isso". Ele anota a regra.
- No fim, `/salvar` guarda tudo no meu GitHub.

## Num computador novo

1. Instale o VS Code, o Git, o GitHub CLI (`gh`) e a extensão do Claude Code, como no README da
   trilha.
2. No terminal: `gh auth login --web --git-protocol https`, depois `gh repo clone espaco-ni ~/NI`.
3. Abra `~/NI` no VS Code, abra o Claude e peça: "Copia `eu/claude-do-computador.md` para
   `~/.claude/CLAUDE.md`."
4. Se ainda precisar da trilha: `gh repo clone contasinovacao-dev/trilha-claude ~/NI/trilha-claude`.
