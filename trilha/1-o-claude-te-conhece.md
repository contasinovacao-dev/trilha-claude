# Etapa 1: O Claude te conhece

**Tempo:** 15 minutos.
**Você sai sabendo:** por que o Claude esquece entre uma conversa e outra, e onde escrever para ele
lembrar.

## A ideia

O Claude não lembra das conversas anteriores. No começo de cada conversa, ele lê alguns arquivos de
instrução chamados `CLAUDE.md` e tira o contexto deles. O mais importante fica no seu computador, em
`~/.claude/CLAUDE.md` (`~` é a sua pasta de usuário: `C:\Users\<você>` no Windows,
`/Users/<você>` no Mac). O que estiver nesse arquivo, ele sabe em qualquer pasta que você abrir.

Nesta etapa você escreve esse arquivo com a ajuda do Claude, e testa se ele funcionou.

## Roteiro para o Claude

1. Explique a ideia acima em até quatro linhas.
2. Entreviste a pessoa em até três mensagens, com opções onde der:
   - nome completo e como prefere ser chamada;
   - curso e ano;
   - squad, produto e dupla;
   - o que está fazendo agora no treinamento (o card ou a tarefa);
   - experiência com programação e terminal: nenhuma, pouca ou alguma;
   - como já usou IA: quase nada, em tarefas da faculdade ou bastante;
   - como prefere receber crítica: direta, com exemplo ou com o porquê;
   - uma coisa em que quer ficar melhor no treinamento (entrevistar, escrever, analisar número,
     apresentar, outra).
3. Defina a pasta da pessoa no repositório: o primeiro nome em minúsculas e sem acento (`thaisa`).
   Se já existir em `trainees/` ou em `turma.md`, use o primeiro nome com a inicial do sobrenome
   (`thaisa-m`).
4. Monte o `~/.claude/CLAUDE.md` a partir de `modelos/claude-do-computador.md`. Mostre o texto
   inteiro e pergunte o que mudar. Ela é a autora: troque o que ela pedir.
   - Se o arquivo já existir, mostre o que tem e acrescente a seção no fim, sem apagar nada.
5. Salve. Crie `trainees/<pasta>/` com:
   - `perfil.md`, do modelo `modelos/perfil.md`. É curto porque o time vê: nome, squad, dupla e
     computador. O resto fica só no computador dela;
   - `progresso.md`, do modelo `modelos/progresso.md`, com a etapa 1 feita;
   - `diario.md`, do modelo `modelos/diario.md`, ainda sem entradas.
6. **Teste.** Peça que ela abra uma conversa nova (o botão de nova conversa no painel do Claude) e
   escreva: "Quem sou eu e o que estou fazendo no treinamento?". A resposta tem de vir do arquivo,
   sem ela contar de novo. A trilha continua na conversa nova, pela etapa 2.

## Pronto quando

- [ ] `~/.claude/CLAUDE.md` tem a seção "Quem usa este computador", revisada pela pessoa.
- [ ] `trainees/<pasta>/` tem `perfil.md`, `progresso.md` e `diario.md`.
- [ ] Numa conversa nova, o Claude disse quem ela é sem ela contar.
