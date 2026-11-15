---
name: salvar
description: Guardar o espaço de trabalho no GitHub da pessoa (o repositório privado espaco-ni) e, enquanto a trilha estiver em andamento, salvar a trilha também. Use quando a pessoa disser "salvar", "vou parar", "manda pro GitHub", "guarda isso", no fim de uma etapa da trilha e no fim de uma conversa em que algum arquivo mudou.
---

# Salvar

Guarda o espaço `~/NI` no repositório privado `espaco-ni`, no GitHub da pessoa. Rode a partir de
`~/NI`.

## Passos

1. **A trilha primeiro.** Se o `~/NI/CLAUDE.md` ainda tiver a seção "Trilha em andamento", siga
   `trilha-claude/.claude/skills/salvar/SKILL.md`, com o git em `git -C trilha-claude`. Depois,
   volte aqui.
2. **A cópia do computador.** Compare `~/.claude/CLAUDE.md` com `eu/claude-do-computador.md`. Se
   estiverem diferentes, copie o primeiro sobre o segundo e diga isso em uma linha.
3. **O que mudou.** Rode `git status` em `~/NI` e explique em uma linha cada arquivo que mudou. Se
   nada mudou, diga que já está tudo salvo e pare.
4. **Conferência.** Nenhum arquivo pode ter senha, token, `.env`, nem nome, telefone ou e-mail de
   entrevistado, lead ou cliente. Se tiver, pare, mostre onde está e pergunte o que fazer. A pasta
   `trilha-claude/` não pode aparecer no `git status`; se aparecer, pare e confira o `.gitignore`.
5. **A mensagem.** Proponha uma mensagem de commit curta, dizendo o que mudou
   (`treinamento: ata da entrevista com a coordenadora`), e pergunte se pode enviar.
6. **O envio.** Com o ok: `git add -A`, `git commit -m "<mensagem>"` e `git push`.
7. Diga em uma linha que está salvo. `gh repo view --web` abre o repositório no navegador.

## Nunca

- `push --force`, `reset --hard` ou apagar branch.
- Tornar o `espaco-ni` público.
- Copiar arquivo do espaço para a trilha.
