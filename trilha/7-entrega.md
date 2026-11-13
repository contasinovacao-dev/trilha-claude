# Etapa 7: Entrega

**Tempo:** 15 minutos. **Prazo:** segunda, 2026-11-16.
**Você sai sabendo:** trazer o trabalho do time para a sua branch e resolver um conflito.

## A ideia

Enquanto você fazia a trilha, os outros trainees também mexeram no `turma.md`, e o PR de alguns pode
já ter entrado na `main`. Antes de pedir a revisão, você traz a `main` para a sua branch. Se duas
pessoas mudaram o mesmo trecho de um arquivo, o Git não sabe qual versão vale e pede para você
decidir. Isso é um conflito, e é normal.

## Roteiro para o Claude

1. Confira o `progresso.md`: etapas 1 a 6 feitas, seis entradas no diário e a skill. O que faltar,
   diga e pergunte se ela quer fazer antes.
2. `git fetch origin` e `git merge origin/main`. Explique: o primeiro baixa o que mudou no GitHub, o
   segundo junta a `main` na branch dela.
3. Se der conflito no `turma.md`, abra o arquivo no VS Code e mostre as marcas `<<<<<<<`, `=======`
   e `>>>>>>>`: em cima fica a versão dela, embaixo a da `main`. Aqui as duas valem, então ficam
   todas as linhas. Ela resolve no VS Code, com **Accept Both Changes**, ou você resolve e mostra.
   Depois, `git add turma.md` e `git commit`.
4. `git push`.
5. Tire do `~/NI/CLAUDE.md` a seção "Trilha em andamento".
6. `gh pr ready` tira o PR do rascunho. Ela manda o link para o Bruno.
7. Explique a conversa de fechamento com o Bruno: ela mostra o diário e conta um uso que mudou o
   trabalho dela e um em que o Claude errou ou não ajudou.
8. Marque a etapa 7 em `progresso.md` e rode a skill `salvar`.

## Pronto quando

- [ ] A branch dela tem a `main` mais recente e nenhum conflito aberto.
- [ ] O PR saiu do rascunho e o Bruno recebeu o link.
- [ ] A seção "Trilha em andamento" saiu do `~/NI/CLAUDE.md`.
