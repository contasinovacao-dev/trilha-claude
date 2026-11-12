---
name: salvar
description: Salvar o progresso da Trilha do Claude, atualizando o progresso.md, mostrando o que mudou e fazendo commit e push na branch do trainee. Use quando a pessoa disser "salvar", "vou parar", "terminei a etapa", "manda pro GitHub", e sempre no fim de uma etapa.
---

# Salvar

Se você estiver aberto em `~/NI`, rode o git com `git -C trilha-claude` e leia os caminhos abaixo a
partir de `trilha-claude/`.

1. Atualize `trainees/<pasta>/progresso.md`: o status e a data da etapa, e "Onde parou" em uma ou
   duas frases.
2. Se o GitHub ainda não estiver configurado (antes do passo 8 da etapa 2), pare aqui e diga que o
   envio começa na etapa 2.
3. Rode `git status` e explique em uma linha cada arquivo que mudou.
4. Confira que a branch é `trilha/<pasta>`. Se for a `main`, pare e explique antes de qualquer
   commit.
5. Confira que nenhum arquivo de outro trainee mudou e que nenhum arquivo tem nome, telefone ou
   e-mail de entrevistado.
6. Proponha a mensagem do commit no formato `trilha: <o que mudou>` e pergunte se pode enviar.
7. Com o ok: `git add` só da pasta dela e do `turma.md`, `git commit` e `git push`.
8. Diga que o pull request já mostra a mudança (`gh pr view --web` abre no navegador) e qual é o
   próximo passo da trilha.
