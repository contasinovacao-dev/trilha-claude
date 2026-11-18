# Trilha do Claude

Esta trilha deixa o Claude pronto no seu computador e ensina a usá-lo no treinamento do NI. No fim,
você tem:

- o Claude sabendo quem você é, o que você faz no NI, qual é o seu objetivo no treinamento e como
  você gosta de trabalhar, em qualquer pasta que você abrir;
- um objetivo no NI que dá para conferir, com uma revisão por semana;
- uma pasta de trabalho montada pelo Claude, com um lugar para o treinamento e outro para a
  faculdade, guardada num repositório privado no seu GitHub, o `espaco-ni`;
- o Claude também no navegador e no celular, com o mesmo contexto;
- a sua primeira contribuição no GitHub, revisada pelo Bruno;
- seis jeitos de usar o Claude para pensar melhor, testados no seu próprio card.

O Claude conduz a trilha. Você só faz à mão o que vem antes de ele estar no seu computador.

## Antes do Claude (uns 20 minutos, na sessão com o Bruno)

1. **GitHub.** Crie uma conta em <https://github.com> (pode ser com o seu e-mail pessoal) e mande o
   seu usuário para o Bruno. Ele te convida para este repositório. O convite chega por e-mail e
   vence em 7 dias: aceite.
2. **Claude.** Entre na sua conta do Claude em <https://claude.ai>, no navegador.
3. **VS Code.** Instale o editor em <https://code.visualstudio.com>. Ao abrir, ligue o salvamento
   automático: menu **File → Auto Save**.
4. **Git**, o programa que guarda o histórico dos arquivos.
   - Windows: baixe em <https://git-scm.com/download/win> e clique em Next em todas as telas.
   - Mac: abra o app **Terminal**, digite `git --version` e aperte Enter. Se aparecer a janela
     pedindo para instalar as ferramentas de linha de comando, clique em **Instalar**.
5. **Claude Code no VS Code.** No VS Code, abra **Extensions** (`Ctrl+Shift+X` no Windows,
   `Cmd+Shift+X` no Mac), procure **Claude Code**, confira que é da **Anthropic** e clique em
   **Install**.
6. **Baixar esta trilha.** Aperte `Ctrl+Shift+P` (Windows) ou `Cmd+Shift+P` (Mac), digite
   **Git: Clone** e escolha **Clone from GitHub**. O navegador abre para você autorizar o GitHub.
   Escolha `trilha-claude`. Quando ele pedir a pasta, crie uma pasta chamada `NI` dentro da sua
   pasta de usuário (`C:\Users\<você>\NI` ou `/Users/<você>/NI`) e escolha ela. No fim, clique em
   **Open**.
7. **Abrir o Claude.** Clique no ícone do Claude no canto de cima, à direita do editor, ou aperte
   `Ctrl+Shift+P` / `Cmd+Shift+P` e digite **Claude Code**. Entre com a sua conta do Claude.
8. **O primeiro prompt.** Abra `primeiro-prompt.md`, na lista de arquivos à esquerda, copie a
   mensagem e mande para o Claude. Ele te entrevista dali em diante, uma pergunta por vez. Deixe à
   mão um print da sua grade horária do Júpiter ou da sua agenda da semana: ele vai pedir.

Daqui em diante, é com ele.

## A trilha

| Etapa | Você sai sabendo | Tempo |
| --- | --- | --- |
| 1. O Claude te conhece e monta o seu espaço | por que o Claude esquece, o que ele anota para lembrar de você e como ficou a sua pasta de trabalho | 30 min |
| 2. O seu trabalho no GitHub | o ciclo branch, commit, push e pull request | 25 min |
| 3. O Claude fora do VS Code | usar o Claude no navegador e no celular com o contexto do treinamento | 15 min |
| 4. O seu espaço, no seu GitHub | guardar a sua pasta num repositório privado seu e trabalhar nela | 20 min |
| 5. Pensar com o Claude | os seis usos no treinamento, testados no seu card | 20 min na sessão, o resto até segunda, 16/11 |
| 6. A sua skill | transformar um pedido que você repete num comando seu | 15 min, até 16/11 |
| 7. Entrega | trazer o trabalho do time para a sua branch e resolver um conflito | 15 min |

Na sessão com o Bruno, a ideia é chegar até a etapa 4 e fazer dois usos da etapa 5. O resto, até a
etapa 7 com o pull request pronto para revisão, vai até **segunda, 16/11**.

## O que ler

- [`guia/usos.md`](guia/usos.md): os seis usos do Claude no treinamento, com pedidos de exemplo. É o
  guia para depois da trilha.
- [`guia/organizar-o-claude.md`](guia/organizar-o-claude.md): o que vai em cada arquivo do Claude e
  como manter o seu harness em dia.
- [`guia/combinados.md`](guia/combinados.md): as regras. São nove, curtas.

## Se travar

- O Claude errou duas vezes no mesmo passo: ele anota no seu `progresso.md` e você chama o Bruno.
- Fechou o VS Code no meio: abra de novo e escreva "onde eu parei?". O progresso fica salvo.
- Não entendeu uma palavra: pergunte. O glossário está em [`guia/glossario.md`](guia/glossario.md).
