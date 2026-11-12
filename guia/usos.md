# Como usar o Claude no treinamento

O Claude é uma ferramenta para você pensar e trabalhar melhor. Ele não faz o treinamento por você:
quem é avaliado, quem entrevista e quem decide é você. Este guia mostra os seis usos que mais ajudam
no treinamento do NI, com pedidos de exemplo para copiar e adaptar.

**A regra que vale para todos:** traga o seu pensamento primeiro. "Escrevi três hipóteses, ataca a
mais fraca" rende mais do que "escreve três hipóteses". No primeiro pedido, você aprende alguma
coisa. No segundo, só o Claude trabalha.

## 1. Discutir uma ideia: `/discutir`

Para testar uma hipótese, uma decisão ou uma dúvida antes de levar para a dupla ou para o PM. O
Claude pergunta de onde vem a ideia, traz o argumento contrário mais forte e termina com um jeito de
testá-la.

- "Acho que escola independente decide a compra mais rápido que escola de rede. Me ataca."
- "Estou em dúvida entre falar primeiro com a coordenadora ou com o diretor. Me ajuda a pensar, mas
  a decisão é minha."
- "Essa suposição da nossa matriz CSD está bem escrita? Como eu testaria numa entrevista?"

**Cuidado:** se ele concordar com tudo, peça "qual é o melhor argumento contra isso?".

## 2. Ensaiar: `/ensaiar`

Para treinar uma entrevista, uma ligação ou um pitch antes de fazer de verdade. O Claude faz o papel
da outra pessoa e, no fim, aponta as perguntas que induziram a resposta e as que você deixou de
aprofundar.

- "Faz o papel de um professor de matemática de uma escola que monta o próprio simulado. Vou testar
  o meu roteiro."
- "Faz uma coordenadora ocupada que atende o telefone sem saber quem eu sou. Tenho 30 segundos."
- No celular, pela conversa por voz: ensaie a abertura da entrevista falando, do jeito que vai ser.

**Cuidado:** o personagem é inventado. Ele mostra como você pergunta, e não o que a escola de verdade
pensa. O que vale como descoberta só sai da entrevista real.

## 3. Revisar: `/revisar`

Para conferir um texto antes de ele sair: mensagem de WhatsApp ou LinkedIn, e-mail, ata, slide,
resposta num card. O Claude aponta até cinco problemas, do mais grave para o menos grave, e você
reescreve.

- "Vou mandar isso no WhatsApp para uma coordenadora que não me conhece. O que está atrapalhando?"
- "Esta é a conclusão do meu card. Um PM entende em 30 segundos o que eu descobri?"
- "Revisa o português e me diz o que mudou. Não muda o conteúdo."

**Cuidado:** peça a reescrita só depois de tentar a sua. Se pedir, compare as duas e veja o que ele
mudou.

## 4. Aprender: `/explicar`

Para entender um conceito de que você precisa agora, com exemplo do seu trabalho, e ser testado
nele.

- "Me explica TRI com um exemplo de simulado e me faz três perguntas."
- "O que é TAM, SAM e SOM? Monta o exemplo com escolas particulares de São Paulo."
- "Não entendi a diferença entre suposição e dúvida na matriz CSD. Me testa."
- "O que é um pull request? Explica com o que eu fiz na trilha."

**Cuidado:** explicar de volta, com as suas palavras, é o que mostra que você entendeu.

## 5. Pesquisar: `/pesquisar`

Para buscar um número, um concorrente ou um fato sobre uma empresa. O Claude responde numa tabela,
com o link e a data de cada afirmação, e separa o que a fonte diz do que é estimativa dele.

- "Quantas escolas particulares com ensino médio existem no estado de São Paulo? Quero a fonte do
  INEP."
- "O que o portal do SAS mostra para o professor depois do simulado? Só fonte pública."
- "Que empresas vendem software para transportadora de carga fracionada no Brasil?"

**Cuidado:** abra pelo menos dois links e confira se a fonte diz mesmo aquilo. O Claude erra número
e cita fonte que não diz o que ele disse.

## 6. Organizar: `/ata` e pedidos livres

Para o trabalho mecânico: anotação em ata, lista em tabela, card em passos.

- "Colei as minhas anotações da entrevista. Faz a ata." (`/ata`)
- "Tenho este card e quatro dias. Quebra em passos e me diz o que depende do quê."
- "Transforma esta lista de escolas numa tabela com cidade, tipo e sistema de ensino."
- "Junta as respostas das três entrevistas sobre preço numa tabela, uma coluna por escola."

**Cuidado:** na ata, a parte "o que isso muda para nós" é sua. O Claude organiza o que foi dito; a
conclusão você escreve.

## Pedidos que funcionam melhor

- **Dê contexto:** para quem é, para quê, até quando, o que você já tentou.
- **Peça para ele te entrevistar antes:** "Antes de responder, me faz as perguntas de que você
  precisa."
- **Diga o formato:** "em cinco linhas", "numa tabela", "uma pergunta por vez".
- **Peça o contrário:** "Qual é o melhor argumento contra isso?"
- **Peça a fonte:** "De onde vem esse número?"
- **Uma conversa por assunto.** Assunto novo, conversa nova: ele se perde menos e gasta menos limite.

## O que não pedir

- **Escrever o que avalia você:** as suas hipóteses, o seu roteiro, a sua análise. Peça crítica.
- **Inventar dado:** sem fonte, não serve para o card.
- **Falar em seu nome:** a mensagem para a escola, o lead ou o colega sai de você, revisada por você.
- **Guardar dado pessoal de entrevistado:** nome, telefone, e-mail. Use o cargo e a organização.

## Quando o Claude erra

Ele erra com a mesma segurança com que acerta. Os erros mais comuns:

- número sem fonte, ou com uma fonte que não diz aquilo;
- informação velha sobre uma empresa ou um produto;
- concordar com você porque você pareceu ter certeza.

Já aconteceu no NI: a afirmação de que um sistema usado por transportadoras "não tem API" foi
repetida sem fonte numa discussão, e as fichas do próprio discovery mostravam o contrário.

O que fazer: abra a fonte, pergunte "como você sabe?" e peça o argumento contrário. Quando pegar um
erro, anote no diário. Pegar o erro é parte do que o treinamento quer ver.

## Onde usar cada um

| Situação | Onde |
| --- | --- |
| Vou escrever, organizar ou salvar arquivos | VS Code, na pasta do projeto |
| Quero discutir uma ideia rápido, longe do computador | app do celular, no Projeto "Treinamento NI" |
| Vou ensaiar uma entrevista falando | app do celular, conversa por voz |
| Tenho um PDF ou um print para entender | claude.ai, no Projeto |
| Quero que fique registrado para a próxima conversa | arquivo no VS Code (`CLAUDE.md` do projeto ou uma nota) |
