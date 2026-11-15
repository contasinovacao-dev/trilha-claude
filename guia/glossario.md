# Glossário

## Computador e Git

- **Terminal:** a janela onde se escreve comandos em vez de clicar. No VS Code: **Terminal → New
  Terminal**.
- **Pasta de usuário (`~`):** a sua pasta principal no computador. `C:\Users\<você>` no Windows,
  `/Users/<você>` no Mac.
- **Repositório:** uma pasta que guarda o histórico de cada mudança nos arquivos.
- **Clonar:** baixar um repositório do GitHub para o seu computador, com o histórico.
- **Commit:** um ponto salvo no histórico, com uma mensagem dizendo o que mudou.
- **Branch:** uma linha de trabalho separada. A principal se chama `main`.
- **Push:** mandar os seus commits para o GitHub.
- **Pull:** trazer para o seu computador o que os outros mandaram.
- **Pull request (PR):** o pedido para alguém revisar a sua branch e juntá-la na `main`.
- **Conflito:** quando duas pessoas mudaram o mesmo trecho e o Git pede para você decidir qual
  versão vale.
- **GitHub CLI (`gh`):** o programa que conversa com o GitHub pelo terminal.
- **Repositório privado:** só quem o dono convida vê. O seu `espaco-ni` é privado, e só você está
  nele.
- **`.gitignore`:** a lista do que o Git deixa de fora do repositório.

## Claude

- **Claude Code:** o Claude que trabalha com os arquivos do seu computador. Você usa pelo painel no
  VS Code.
- **`CLAUDE.md`:** arquivo de instruções que o Claude lê no começo de toda conversa. O de
  `~/.claude/` vale em qualquer pasta; o de uma pasta vale quando você abre aquela pasta.
- **Contexto:** tudo o que o Claude tem diante dele numa conversa: os `CLAUDE.md`, o que você
  escreveu e os arquivos que ele leu. Fora disso, ele não sabe.
- **Skill:** um pedido pronto, guardado num arquivo, que vira comando com `/`.
- **Harness:** o conjunto de arquivos que faz o Claude trabalhar do seu jeito: os `CLAUDE.md`, as
  skills e as regras do `settings.json`. O seu fica no `espaco-ni`. Ver `guia/organizar-o-claude.md`.
- **Espaço (`~/NI`):** a pasta onde você trabalha com o Claude no dia a dia, guardada no
  repositório privado `espaco-ni`.
- **Projeto (claude.ai):** uma pasta de conversas no claude.ai, com instruções e arquivos próprios e
  uma memória separada.
- **Limite de uso:** quanto a sua conta pode usar por janela de cinco horas e por semana, somando
  VS Code, navegador e celular. `/usage` mostra quanto já foi.

## Treinamento

- **Discovery:** conversar com quem tem o problema para entender o que acontece hoje, antes de
  construir ou vender.
- **Matriz CSD:** certezas, suposições e dúvidas sobre um produto. Cada suposição e cada dúvida têm
  um "como testar".
- **Card:** uma tarefa do quadro do treinamento, com dupla, prazo e critério de aceite.
