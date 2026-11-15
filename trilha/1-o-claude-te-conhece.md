# Etapa 1: O Claude te conhece

**Tempo:** 25 minutos.
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

Nesta etapa, o Claude te entrevista, uma pergunta por vez, e guarda as respostas nesses três
arquivos enquanto vocês conversam.

## A entrevista

Seis blocos, nesta ordem. "Vai para" diz onde a resposta é guardada; `eu/` é `~/NI/eu/`.

| Bloco | Pergunta | Opções | Vai para |
| --- | --- | --- | --- |
| 1. Quem é você | Qual é o seu nome completo? | | `~/.claude/CLAUDE.md`, `perfil.md` |
| | Como você prefere que eu te chame? | | `~/.claude/CLAUDE.md` |
| | Qual é o seu curso, e em que ano você está? | | `~/.claude/CLAUDE.md`, `eu/sobre-mim.md` |
| 2. Você e o computador | Quanta experiência você tem com programação e terminal? | nenhuma, pouca, alguma | `~/.claude/CLAUDE.md` |
| | Como você já usou IA? | quase nada, em tarefas da faculdade, bastante | `~/.claude/CLAUDE.md` |
| 3. O NI | Quem é a sua dupla no squad do Ludi? | | `~/.claude/CLAUDE.md`, `eu/sobre-mim.md`, `perfil.md` |
| | O que você está fazendo agora no treinamento? Pode ser o card ou a tarefa. | | `~/.claude/CLAUDE.md` |
| | Por que você entrou no NI? | | `eu/sobre-mim.md` |
| 4. Fora do NI | Quais matérias você faz neste semestre, das que mais pesam para as que menos pesam? | | `eu/sobre-mim.md` |
| | Tem alguma prova ou entrega grande com data marcada? | | `eu/sobre-mim.md` |
| | O que você faz além da faculdade e do NI? | estágio, outra entidade, esporte, trabalho, iniciação científica, nada agora (pode marcar mais de uma) | `eu/sobre-mim.md` |
| | Como é a sua semana: que horários já estão tomados, e quando você estuda e trabalha no NI? | | `eu/sobre-mim.md` |
| | O que você gosta de fazer ou de estudar por conta própria? | | `eu/sobre-mim.md` |
| 5. Como trabalhar com você | Como você prefere receber crítica? | direta, com exemplo, com o porquê | `~/.claude/CLAUDE.md` |
| | Em que você quer ficar melhor no treinamento? | entrevistar, escrever, analisar número, apresentar | `~/.claude/CLAUDE.md` |
| | O que te irrita numa resposta de IA? | | `~/.claude/CLAUDE.md` |
| 6. Objetivos | Três objetivos, um de cada vez: no treinamento, até o fim de 2026.2; na faculdade, neste semestre; de carreira ou pessoal, para 2027. Para cada um, as perguntas do passo 5 do roteiro. | | `eu/objetivos.md` e uma linha em `~/.claude/CLAUDE.md` |

## Roteiro para o Claude

1. **A abertura.** Explique a ideia acima em até cinco linhas e diga como vai ser: umas vinte
   perguntas curtas, uma por vez, em seis blocos; ela pode pular qualquer uma; você guarda as
   respostas no fim de cada bloco e diz o que guardou; ela corrige quando quiser. Faça a primeira
   pergunta na mesma mensagem.
2. **Como perguntar.**
   - Uma pergunta por mensagem, na ordem da tabela.
   - Onde a tabela traz opções, pergunte com opções clicáveis, sem marcar nenhuma como recomendada.
     Ela pode escrever outra resposta.
   - Antes da pergunta seguinte, reaja ao que ela disse em uma frase, no máximo. Sem elogio.
   - Pergunta pulada não volta. Resposta curta basta: não peça mais detalhe, a não ser no bloco 6.
3. **Guardar no fim de cada bloco.** Escreva as respostas do bloco nos arquivos da coluna "Vai
   para", a partir dos modelos (`modelos/claude-do-computador.md`, `modelos/sobre-mim.md`,
   `modelos/objetivos.md`, `modelos/perfil.md`).
   - Na primeira vez, crie o arquivo só com as seções que já têm resposta. Nos blocos seguintes,
     acrescente.
   - Depois de guardar, diga em uma linha o que guardou e onde: "Guardei no `~/.claude/CLAUDE.md`:
     nome, apelido, curso e ano." Se ela pedir para mudar, mude na hora.
   - No fim do bloco 4, escreva também a linha "Fora do NI" do `~/.claude/CLAUDE.md`: as matérias
     que mais pesam e as outras atividades.
   - Na primeira vez que você editar um arquivo fora da trilha, o Claude Code pede permissão.
     Explique o pedido. Ela pode permitir as edições desta conversa, para não ser perguntada a cada
     bloco.
   - Se o `~/.claude/CLAUDE.md` já existir antes da entrevista, mostre o que tem e acrescente as
     seções no fim, sem apagar nada.
4. **A pasta na trilha**, logo depois de guardar o bloco 1.
   - Defina a pasta: o primeiro nome em minúsculas e sem acento (`thaisa`). Se já existir em
     `trainees/` ou em `turma.md`, use o primeiro nome com a inicial do sobrenome (`thaisa-m`).
   - Crie `trainees/<pasta>/` com `perfil.md` (do modelo, só com o nome por enquanto),
     `progresso.md` (do modelo, com a etapa 1 em andamento) e `diario.md` (do modelo, sem entradas).
   - A cada bloco guardado, atualize "Onde parou" no `progresso.md`: "Etapa 1: blocos 1 a 3
     guardados; falta o 4." Se a conversa cair, a próxima retoma pelo bloco seguinte, sem repetir
     pergunta.
5. **O bloco 6, objetivos.** Antes de começar, explique em duas linhas que um objetivo serve quando
   dá para conferir se chegou. Depois, para cada um dos três objetivos, três mensagens:
   1. "Qual é o seu objetivo {no treinamento, até o fim de 2026.2 | na faculdade, neste semestre |
      de carreira ou pessoal, para 2027}?"
   2. "Como você vai saber que chegou? Pense em algo que dá para ver ou contar. E até quando?"
   3. "O que dá para fazer nesta semana para andar nele?"

   Guarde cada objetivo em `eu/objetivos.md` assim que as três respostas chegarem, e a linha dele
   na seção "Objetivos" do `~/.claude/CLAUDE.md`.

   Ela responde com as palavras dela. Não proponha objetivo, medida nem próximo passo. Se a medida
   vier vaga ("ficar boa em entrevista"), pergunte de novo uma vez, com um exemplo de medida de
   outro assunto ("correr 5 km sem parar até dezembro"). Se continuar vaga, guarde como ela disse,
   com "medida a definir": a revisão com `/objetivos` volta nele.
6. **A revisão.** Mostre o `~/.claude/CLAUDE.md` inteiro e explique que é isso que você vai ler em
   toda conversa. Pergunte o que mudar. Depois, pergunte se ela quer que o objetivo no treinamento
   apareça no `perfil.md`, que o Bruno vê. Se não, o campo fica "só no computador". Marque a etapa 1
   como feita no `progresso.md`.
7. **Teste.** Peça que ela abra uma conversa nova (o botão de nova conversa no painel do Claude) e
   escreva: "Quem sou eu, quais são os meus objetivos e o que estou fazendo no treinamento?". A
   resposta tem de vir dos arquivos, sem ela contar de novo. A trilha continua na conversa nova,
   pela etapa 2.

## Pronto quando

- [ ] `~/.claude/CLAUDE.md` tem "Quem usa este computador", "Objetivos" e "Como trabalhar
      comigo", revisados por ela.
- [ ] `~/NI/eu/sobre-mim.md` e `~/NI/eu/objetivos.md` existem. Cada objetivo tem medida, prazo e
      próximo passo escritos por ela, ou "medida a definir".
- [ ] `trainees/<pasta>/` tem `perfil.md`, `progresso.md` e `diario.md`.
- [ ] Numa conversa nova, o Claude disse quem ela é e quais são os objetivos dela sem ela contar.
