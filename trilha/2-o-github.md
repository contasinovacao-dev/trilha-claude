# Etapa 2: O seu trabalho no GitHub

**Tempo:** 25 minutos.
**Você sai sabendo:** o ciclo que todo repositório do NI usa: branch, commit, push e pull request.

## A ideia

- **Repositório:** uma pasta que guarda o histórico de cada mudança. Esta trilha é um.
- **Commit:** um ponto salvo nesse histórico, com uma mensagem dizendo o que mudou.
- **Branch:** uma linha de trabalho separada da principal, que se chama `main`. Você mexe na sua sem
  mexer na do time.
- **Push:** manda os seus commits do computador para o GitHub.
- **Pull request (PR):** o pedido para alguém revisar a sua branch e juntá-la na `main`. Aqui, quem
  revisa é o Bruno.

O VS Code mostra tudo isso no ícone **Source Control**, na barra da esquerda. O Claude faz pelo
terminal, e você acompanha por lá.

## Roteiro para o Claude

1. Explique as cinco palavras acima, em até seis linhas.
2. **GitHub CLI** (`gh`, o programa que conversa com o GitHub pelo terminal). Rode `gh --version`.
   - Se faltar, no Windows: `winget install --id GitHub.cli -e --accept-source-agreements
     --accept-package-agreements`. O Windows pode pedir permissão, e ela clica em Sim.
   - No Mac: ela baixa o instalador `.pkg` em <https://cli.github.com> e abre com duplo clique.
   - Depois de instalar, rode a skill `salvar` (só o progresso) e peça para ela fechar o VS Code
     inteiro e abrir de novo, para o terminal achar o programa novo. A conversa recomeça de onde
     parou.
3. **Login no GitHub.** Ela abre o terminal do VS Code (menu **Terminal → New Terminal**) e roda
   `gh auth login --web --git-protocol https`. Explique antes:
   - aparece um código de oito letras;
   - ela aperta Enter, o navegador abre, ela cola o código e autoriza;
   - se aparecer "Authenticate Git with your GitHub credentials?", a resposta é Y.

   Depois, você roda `gh auth status` para conferir.
4. **Quem assina os commits.** Pegue o id e o usuário com `gh api user --jq '.id, .login'` e rode:
   - `git config --global user.name "<Nome Sobrenome>"`
   - `git config --global user.email "<id>+<usuario>@users.noreply.github.com"`

   Explique que esse é um e-mail do próprio GitHub, que assina os commits sem mostrar o e-mail
   pessoal.
5. **A branch.** `git switch -c trilha/<pasta>`. Mostre o nome da branch no canto de baixo, à
   esquerda, do VS Code.
6. **A turma.** Acrescente a linha dela no fim da tabela de `turma.md` e o usuário do GitHub no
   `perfil.md`. Mostre a diferença com `git diff`.
7. **O primeiro commit.** `git add trainees/<pasta> turma.md` e
   `git commit -m "trilha: <Nome> entra na turma"`. Mostre o resultado com `git log --oneline -3` e
   no painel Source Control.
8. **O push.** `git push -u origin trilha/<pasta>`.
9. **O pull request.**
   `gh pr create --draft --base main --title "Trilha de <Nome>" --body-file .github/pull_request_template.md`.
   Explique que ele nasce como rascunho (draft): o Bruno acompanha, e o PR só vira pedido de revisão
   na etapa 7. Peça para ela abrir o link e olhar a aba **Files changed**.
10. Peça para ela explicar, com as palavras dela, a diferença entre commit e push. Corrija se
    precisar.
11. Guarde o link do PR em `progresso.md`, marque a etapa 2 e rode a skill `salvar`.

## Pronto quando

- [ ] `gh auth status` mostra o usuário dela.
- [ ] O PR rascunho "Trilha de <Nome>" existe e mostra o `turma.md` e a pasta dela.
- [ ] Ela explicou commit e push com as palavras dela.
