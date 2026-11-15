# O primeiro prompt

É a primeira mensagem que você manda para o Claude. Ele usa as suas respostas para montar o seu
contexto e os seus objetivos na etapa 1, e daí segue a trilha até o seu espaço guardado no seu
GitHub.

**Como usar:**

1. Copie o bloco abaixo para um arquivo novo do VS Code (`Ctrl+N` no Windows, `Cmd+N` no Mac) ou
   para as notas do celular. Não responda dentro deste arquivo: ele é da trilha.
2. Responda depois de cada dois-pontos, em frases curtas. Não tem resposta certa.
3. Pule o que não quiser contar. O Claude não insiste.
4. Cole tudo no Claude e mande. Se respondeu num arquivo novo do VS Code, feche sem salvar.

Dá para responder antes da sessão, pelo celular.

```text
Oi, Claude. Sou trainee do NI e vou começar a Trilha do Claude. Abaixo estão as minhas respostas
às perguntas de setup. Use para montar o meu contexto e os meus objetivos na etapa 1, e me leve
pela trilha até o meu espaço guardado no meu GitHub. Se faltar alguma coisa, pergunte.

QUEM EU SOU
- Nome completo:
- Como prefiro que me chamem:
- Curso e ano:
- Usuário do GitHub:
- Experiência com programação e terminal (nenhuma, pouca ou alguma):
- Como já usei IA (quase nada, em tarefas da faculdade ou bastante):

NO NI
- Dupla no squad do Ludi:
- O que estou fazendo agora no treinamento (o card ou a tarefa):
- Por que entrei no NI:

FORA DO NI
- Matérias deste semestre, das que mais pesam para as que menos pesam:
- Prova ou entrega grande que já tem data:
- Outras atividades (estágio, outra entidade, esporte, trabalho, iniciação científica):
- A minha semana (horários já tomados, quando estudo, quando trabalho no NI):
- O que eu gosto de fazer ou de estudar por conta própria:

OBJETIVOS (com as minhas palavras; você me ajuda a deixar cada um conferível)
- No treinamento, até o fim de 2026.2:
- Na faculdade, neste semestre:
- Um objetivo de carreira ou pessoal para 2027:

COMO TRABALHAR COMIGO
- Como prefiro receber crítica (direta, com exemplo ou com o porquê):
- Uma coisa em que quero ficar melhor (entrevistar, escrever, analisar número, apresentar, outra):
- O que me irrita numa resposta de IA:
```

## Para onde vão as respostas

| Resposta | Arquivo | Quem vê |
| --- | --- | --- |
| quem você é, os objetivos em uma linha, como trabalhar com você | `~/.claude/CLAUDE.md` | só você, no seu computador |
| fora do NI, a sua semana, o que você gosta | `~/NI/eu/sobre-mim.md` | só você, no seu GitHub (repositório privado) |
| os objetivos com medida, prazo e próximo passo | `~/NI/eu/objetivos.md` | só você, no seu GitHub (repositório privado) |
| nome, dupla, computador, usuário do GitHub e, se você quiser, o objetivo no treinamento | `trainees/<pasta>/perfil.md` | o squad e o Bruno, nesta trilha |
