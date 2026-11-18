# Etapa 1: O Claude te conhece e monta o seu espaço

**Tempo:** 30 minutos.
**Você sai sabendo:** por que o Claude esquece entre uma conversa e outra, o que ele anota para
lembrar de você e como ficou a pasta onde você vai trabalhar com ele.

## A ideia

O Claude não lembra das conversas anteriores. No começo de cada conversa, ele lê alguns arquivos de
anotações chamados `CLAUDE.md` e tira o contexto deles. O principal fica no seu computador, em
`~/.claude/CLAUDE.md` (`~` é a sua pasta de usuário: `C:\Users\<você>` no Windows,
`/Users/<você>` no Mac). O que estiver nesse arquivo, ele sabe em qualquer pasta que você abrir.

Nesta etapa, o Claude te entrevista, guarda as respostas e monta a pasta `~/NI`, onde você vai
trabalhar com ele: uma pasta para o treinamento, uma para a faculdade e uma com quem você é e o seu
objetivo no NI. No fim, ele te mostra o que montou e por quê. Na etapa 4, essa pasta vai para o seu
GitHub, num repositório privado.

O foco da entrevista é o NI. Da faculdade e do resto, o Claude só precisa saber um pouco da sua
semana: um print da grade e uma pergunta.

## A entrevista

Cinco blocos, nesta ordem. Na coluna "Opções", **uma** quer dizer uma resposta só e **várias** quer
dizer que dá para marcar mais de uma. "Vai para" diz onde a resposta é guardada; os caminhos sem `~`
ficam dentro de `~/NI/`.

| Bloco | Pergunta | Opções | Vai para |
| --- | --- | --- | --- |
| 1. Você | Qual é o seu nome, e como prefere que eu te chame? | | `~/.claude/CLAUDE.md`, `perfil.md` |
| | Qual é o seu curso, e em que ano você está? | | `~/.claude/CLAUDE.md` |
| | Quanta experiência você tem com programação e terminal? | uma: nenhuma, pouca, alguma | `~/.claude/CLAUDE.md` |
| | Como você já usou IA? | várias: quase nunca usei; para tirar dúvida; em trabalhos da faculdade; para programar; no dia a dia, para quase tudo | `~/.claude/CLAUDE.md` |
| 2. O NI | Quem é a sua dupla no squad do Ludi? | | `~/.claude/CLAUDE.md`, `treinamento/CLAUDE.md`, `perfil.md` |
| | O que você está fazendo agora no treinamento? Pode ser o card ou a tarefa. | | `~/.claude/CLAUDE.md`, `treinamento/CLAUDE.md` |
| | Por que você entrou no NI? | | `eu/sobre-mim.md` |
| | Em que você quer ficar melhor no treinamento? | várias: entrevistar, escrever, analisar números, apresentar, organizar o meu tempo | `~/.claude/CLAUDE.md`, `treinamento/CLAUDE.md` |
| 3. A sua semana | Me manda um print da sua grade horária (a do Júpiter serve) ou da sua agenda da semana. | uma imagem; pode pular | `eu/sobre-mim.md`, `faculdade/CLAUDE.md` |
| | Além da faculdade e do NI, o que toma o seu tempo? | várias: estágio, outra entidade, esporte, trabalho, iniciação científica, nada agora | `eu/sobre-mim.md` |
| 4. Como trabalhar com você | Como você prefere receber crítica? | várias: direta, com exemplo, com o porquê | `~/.claude/CLAUDE.md` |
| | O que te irrita numa resposta de IA? | várias: resposta longa demais, elogio à toa, inventar coisa, palavra difícil sem explicar, enrolar antes de responder | `~/.claude/CLAUDE.md` |
| 5. O seu objetivo no NI | O objetivo no treinamento, com as três perguntas do passo 5 do roteiro. | | `eu/objetivos.md` e uma linha em `~/.claude/CLAUDE.md` |

## Roteiro para o Claude

1. **A abertura.** Explique a ideia acima em até cinco linhas e diga como vai ser: umas quinze
   perguntas curtas, uma por vez, em cinco blocos, quase todas de clicar; ela pode pular qualquer
   uma; no bloco 3 você vai pedir um print da grade, então ela pode ir deixando pronto; no fim, você
   monta a pasta de trabalho e mostra como ficou. Faça a primeira pergunta na mesma mensagem.
2. **Como perguntar.**
   - Uma pergunta por mensagem, na ordem da tabela.
   - Onde a tabela traz opções, pergunte com opções clicáveis, sem marcar nenhuma como recomendada.
     Nas marcadas com **várias**, deixe marcar mais de uma. Ela sempre pode escrever outra resposta.
   - Antes da pergunta seguinte, reaja ao que ela disse em uma frase, no máximo. Sem elogio.
   - Pergunta pulada não volta. Resposta curta basta: não peça mais detalhe, a não ser no bloco 5.
   - Não acrescente perguntas sobre a faculdade além das duas do bloco 3.
3. **O print do bloco 3.**
   - Explique como mandar: tirar o print direto para a área de transferência (`Win+Shift+S` no
     Windows, `Cmd+Ctrl+Shift+4` no Mac), clicar na caixa de mensagem do Claude e colar (`Ctrl+V` ou
     `Cmd+V`). Se não colar, ela salva o print na Área de Trabalho e te diz o nome do arquivo. Nunca
     na pasta da trilha, para ele não ir para o GitHub.
   - Leia a imagem e confirme numa mensagem curta o que tirou dela: as matérias e os dias e turnos
     de aula ("Li 6 matérias, aula de manhã de segunda a sexta e quinta à tarde. Certo?"). Corrija o
     que ela apontar.
   - Não guarde a imagem. Não anote número USP, nem nome de professor, nem outro dado que não seja
     matéria e horário. Se o print veio da Área de Trabalho, diga que ela já pode apagar.
   - Se ela pular, siga sem a pasta da faculdade.
4. **Guardar no fim de cada bloco.** Escreva as respostas do bloco nos arquivos da coluna "Vai
   para", a partir dos modelos: `modelos/claude-do-computador.md`, `modelos/sobre-mim.md`,
   `modelos/claude-do-treinamento.md`, `modelos/claude-da-faculdade.md`, `modelos/objetivos.md` e
   `modelos/perfil.md`.
   - Na primeira vez, crie o arquivo só com as seções que já têm resposta. Nos blocos seguintes,
     acrescente.
   - Depois de guardar, diga em uma linha o que anotou, sem caminho de arquivo: "Anotei: nome,
     apelido, curso e ano." Onde cada coisa fica aparece no fim, no passo 7. Se ela pedir para
     mudar, mude na hora.
   - No fim do bloco 3, escreva também a linha "Fora do NI" do `~/.claude/CLAUDE.md`: os turnos de
     aula e as outras atividades.
   - Na primeira vez que você editar um arquivo fora da trilha, o Claude Code pede permissão.
     Explique o pedido. Ela pode permitir as edições desta conversa, para não ser perguntada a cada
     bloco.
   - Se o `~/.claude/CLAUDE.md` já existir antes da entrevista, mostre o que tem e acrescente as
     seções no fim, sem apagar nada.
5. **A pasta na trilha**, logo depois de guardar o bloco 1.
   - Defina a pasta: o primeiro nome em minúsculas e sem acento (`thaisa`). Se já existir em
     `trainees/` ou em `turma.md`, use o primeiro nome com a inicial do sobrenome (`thaisa-m`).
   - Crie `trainees/<pasta>/` com `perfil.md` (do modelo, só com o nome por enquanto),
     `progresso.md` (do modelo, com a etapa 1 em andamento) e `diario.md` (do modelo, sem entradas).
   - A cada bloco guardado, atualize "Onde parou" no `progresso.md`: "Etapa 1: blocos 1 a 3
     guardados; falta o 4." Depois da entrevista: "Etapa 1: entrevista feita; falta montar o
     espaço" e, depois do passo 7, "falta o teste". Se a conversa cair, a próxima retoma de onde
     parou, sem repetir pergunta.
6. **O bloco 5, o objetivo no NI.** Antes de começar, explique em duas linhas que um objetivo serve
   quando dá para conferir se chegou. Depois, três mensagens:
   1. "Qual é o seu objetivo no treinamento, até o fim de 2026.2?"
   2. "Como você vai saber que chegou? Pense em algo que dá para ver ou contar. E até quando?"
   3. "O que dá para fazer nesta semana para andar nele?"

   Guarde em `eu/objetivos.md` assim que as três respostas chegarem, e a linha dele na seção
   "Objetivo no NI" do `~/.claude/CLAUDE.md`.

   - É um objetivo só, do NI. Não puxe objetivo de faculdade, de carreira ou pessoal. Se ela quiser
     acrescentar outro do NI, faça as mesmas três perguntas.
   - Ela responde com as palavras dela. Não proponha objetivo, medida nem próximo passo. Se a medida
     vier vaga ("ficar boa em entrevista"), pergunte de novo uma vez, com um exemplo de medida de
     outro assunto ("correr 5 km sem parar até dezembro"). Se continuar vaga, guarde como ela disse,
     com "medida a definir": a revisão com `/objetivos` volta nele.
   - Depois, pergunte se ela quer que o objetivo apareça no `perfil.md`, que o Bruno vê. Se não, o
     campo fica "só no computador".
7. **Montar o espaço.** Com a entrevista feita, monte o resto de `~/NI` sem perguntar pasta por
   pasta: montar é trabalho mecânico, e é seu. Diga numa linha que vai montar e que mostra no fim.
   - `~/NI/CLAUDE.md`, a partir de `modelos/claude-do-espaco.md`;
   - `~/NI/README.md`, a partir de `modelos/espaco/README.md`;
   - as oito pastas de `skills/` em `~/NI/.claude/skills/`;
   - `modelos/espaco/settings.json` em `~/NI/.claude/settings.json`;
   - `modelos/espaco/gitignore` em `~/NI/.gitignore`;
   - uma cópia do `~/.claude/CLAUDE.md` em `~/NI/eu/claude-do-computador.md`.

   Confira que `treinamento/` existe e, se ela mandou a grade, `faculdade/`. Não crie pasta vazia
   nem pasta para outra atividade: se ela quiser uma, pede depois ("cria uma pasta para o estágio").
8. **Mostrar como ficou.** É a parte que fecha a etapa. Fale sem nenhuma palavra técnica: nada de
   harness, repositório, skill, contexto, prompt, markdown ou configuração. Use pasta, arquivo,
   anotação, comando pronto e regra. O nome `CLAUDE.md` aparece uma vez, para ela reconhecer o
   arquivo. São três mensagens curtas; espere ela responder entre uma e outra.
   1. **O que tem.** Abra a pasta para ela ver: no Mac, `open ~/NI`; no Windows,
      `explorer.exe "$(cygpath -w ~/NI)"`. No Windows, esse comando costuma responder com erro mesmo
      quando a janela abre: pergunte se abriu. Mostre o desenho com as pastas que existem de fato:

      ```
      NI                a sua pasta de trabalho com o Claude
      ├── treinamento   o card, a dupla e o que você fizer no treinamento
      ├── faculdade     as matérias da grade que você mandou
      ├── eu            quem você é, a sua semana e o seu objetivo no NI
      └── trilha-claude esta trilha; fica aqui dentro, mas é do time
      ```

      Diga que as pastas de trabalho têm um arquivo chamado `CLAUDE.md`, com as anotações que você
      lê quando ela trabalha ali, e que há uma pasta escondida com os comandos prontos (como
      `/ensaiar`) e as regras do que você pode fazer nessa pasta. Diga também que o resumo de quem
      ela é fica num arquivo fora da pasta, que você lê em qualquer lugar do computador, com uma
      cópia em `eu`.
   2. **Por quê.** Você não lembra de nada de uma conversa para outra: toda conversa começa do zero,
      e é lendo essas anotações que você sabe quem ela é. Dê um exemplo com o que ela respondeu:
      "Amanhã, se você escrever 'me ajuda a preparar a entrevista de quinta', eu já sei que você
      está no {card}, com {dupla}, que quer melhorar em {o que ela marcou} e que prefere crítica
      {como ela marcou}. Você só fala da entrevista." Ofereça mostrar o resumo de quem ela é (o
      `~/.claude/CLAUDE.md`) e, se ela quiser, mostre e ajuste o que ela pedir.
   3. **No dia a dia.** Ela não precisa abrir nem editar esses arquivos. Mudou alguma coisa (card
      novo, grade nova)? Ela fala "mudei de card, atualiza". Você fez algo que ela não gosta? Ela
      fala "não faz mais isso" e você anota a regra. Na etapa 4, a pasta vai para a conta dela no
      GitHub, num lugar que só ela vê, e não se perde se o computador quebrar. O `README.md` da
      pasta tem esta explicação, para ela reler quando quiser.

   Pergunte se ficou alguma dúvida ou se ela quer mudar alguma coisa (o nome de uma pasta, por
   exemplo). Marque a etapa 1 como feita no `progresso.md`, com "falta o teste" em "Onde parou".
9. **Teste.** Peça que ela abra uma conversa nova (o botão de nova conversa no painel do Claude) e
   escreva: "Quem sou eu, qual é o meu objetivo no NI e o que estou fazendo no treinamento?". A
   resposta tem de vir dos arquivos, sem ela contar de novo. A trilha continua na conversa nova,
   pela etapa 2.

## Pronto quando

- [ ] `~/.claude/CLAUDE.md` tem "Quem usa este computador", "Objetivo no NI" e "Como trabalhar
      comigo".
- [ ] `~/NI` tem `CLAUDE.md`, `README.md`, `eu/` com `sobre-mim.md`, `objetivos.md` e
      `claude-do-computador.md`, `treinamento/CLAUDE.md`, as oito skills em `.claude/skills/` e,
      se ela mandou a grade, `faculdade/CLAUDE.md`.
- [ ] O objetivo tem medida, prazo e próximo passo escritos por ela, ou "medida a definir".
- [ ] `trainees/<pasta>/` tem `perfil.md`, `progresso.md` e `diario.md`.
- [ ] Ela viu a pasta aberta e ouviu o porquê, sem palavra técnica.
- [ ] Numa conversa nova, o Claude disse quem ela é, o objetivo e o que ela está fazendo no
      treinamento, sem ela contar.
