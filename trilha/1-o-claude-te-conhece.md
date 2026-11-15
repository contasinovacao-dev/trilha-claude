# Etapa 1: O Claude te conhece

**Tempo:** 20 minutos.
**Você sai sabendo:** por que o Claude esquece entre uma conversa e outra, onde escrever para ele
lembrar e como escrever um objetivo que dá para conferir.

## A ideia

O Claude não lembra das conversas anteriores. No começo de cada conversa, ele lê alguns arquivos de
instrução chamados `CLAUDE.md` e tira o contexto deles. O mais importante fica no seu computador, em
`~/.claude/CLAUDE.md` (`~` é a sua pasta de usuário: `C:\Users\<você>` no Windows,
`/Users/<você>` no Mac). O que estiver nesse arquivo, ele sabe em qualquer pasta que você abrir.

Esse arquivo é curto, porque o Claude lê tudo nele em toda conversa. O detalhe fica em dois arquivos
que ele abre quando precisa, na pasta `~/NI/eu/`: `sobre-mim.md`, a sua vida fora do NI, e
`objetivos.md`. Na etapa 4, a pasta `~/NI` vai para o seu GitHub, num repositório privado. O mapa
das camadas está em `guia/organizar-o-claude.md`.

Nesta etapa você escreve esses três arquivos com o Claude e testa se funcionaram.

## Roteiro para o Claude

1. Explique a ideia acima em até cinco linhas.
2. **As respostas.** A primeira mensagem da pessoa costuma ser o primeiro prompt
   (`primeiro-prompt.md`), já respondido.
   - Se ela veio sem as respostas, mostre o caminho do `primeiro-prompt.md` e ofereça duas opções:
     ela preenche e cola, ou você faz as mesmas perguntas em até quatro mensagens, com opções onde
     der.
   - Depois, numa mensagem só, pergunte o que ficou faltando para os arquivos (nome completo,
     dupla, card) ou vago demais para usar. O que ela pulou de propósito, não pergunte de novo.
3. **Objetivos.** Explique em duas linhas que um objetivo serve quando dá para conferir se chegou.
   Numa mensagem só, faça para cada objetivo que ela escreveu as três perguntas:
   - "Como você vai saber que chegou?" (algo que dá para ver ou contar);
   - "Até quando?";
   - "O que dá para fazer nesta semana?".

   Ela responde com as palavras dela. Não proponha objetivo, medida nem próximo passo. Se a resposta
   ainda estiver vaga ("melhorar em entrevista"), pergunte de novo uma vez, com um exemplo de
   medida de outro assunto ("correr 5 km sem parar até dezembro"). Se continuar vaga, escreva como
   ela disse e marque "medida a definir": a revisão com `/objetivos` volta nele.
4. Defina a pasta da pessoa no repositório: o primeiro nome em minúsculas e sem acento (`thaisa`).
   Se já existir em `trainees/` ou em `turma.md`, use o primeiro nome com a inicial do sobrenome
   (`thaisa-m`).
5. **Os três arquivos dela.** Monte um de cada vez, mostre o texto inteiro e pergunte o que mudar.
   Ela é a autora: troque o que ela pedir.
   - `~/.claude/CLAUDE.md`, de `modelos/claude-do-computador.md`. Se o arquivo já existir, mostre o
     que tem e acrescente as seções no fim, sem apagar nada.
   - `~/NI/eu/sobre-mim.md`, de `modelos/sobre-mim.md`.
   - `~/NI/eu/objetivos.md`, de `modelos/objetivos.md`.

   Diga que `~/NI/eu/` é só dela: vai para o GitHub dela na etapa 4, num repositório privado, e
   nunca para a trilha.
6. **A pasta na trilha.** Crie `trainees/<pasta>/` com:
   - `perfil.md`, do modelo `modelos/perfil.md`. É curto porque o time vê. Pergunte se ela quer que
     o objetivo no treinamento apareça ali para o Bruno; se não, o campo fica "só no computador".
   - `progresso.md`, do modelo `modelos/progresso.md`, com a etapa 1 feita;
   - `diario.md`, do modelo `modelos/diario.md`, ainda sem entradas.
7. **Teste.** Peça que ela abra uma conversa nova (o botão de nova conversa no painel do Claude) e
   escreva: "Quem sou eu, quais são os meus objetivos e o que estou fazendo no treinamento?". A
   resposta tem de vir dos arquivos, sem ela contar de novo. A trilha continua na conversa nova,
   pela etapa 2.

## Pronto quando

- [ ] `~/.claude/CLAUDE.md` tem "Quem usa este computador" e "Objetivos", revisados por ela.
- [ ] `~/NI/eu/sobre-mim.md` e `~/NI/eu/objetivos.md` existem. Cada objetivo tem medida, prazo e
      próximo passo escritos por ela, ou "medida a definir".
- [ ] `trainees/<pasta>/` tem `perfil.md`, `progresso.md` e `diario.md`.
- [ ] Numa conversa nova, o Claude disse quem ela é e quais são os objetivos dela sem ela contar.
