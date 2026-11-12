# Git em uma página

No dia a dia, peça ao Claude: "salva e manda para o GitHub". Ele mostra o que vai antes de mandar.
Esta página é para você saber o que ele está fazendo.

| Quero... | Comando | No VS Code |
| --- | --- | --- |
| ver o que mudou | `git status` e `git diff` | ícone **Source Control**, na barra da esquerda |
| salvar um ponto no histórico | `git add <arquivo>` e `git commit -m "mensagem"` | escrever a mensagem e clicar em **Commit** |
| mandar para o GitHub | `git push` | **Sync Changes** |
| trazer o que o time mandou | `git pull` | **Sync Changes** |
| ver o histórico | `git log --oneline` | aba **Timeline**, embaixo do explorador de arquivos |
| criar uma branch | `git switch -c <nome>` | clicar no nome da branch, no canto de baixo à esquerda |
| trocar de branch | `git switch <nome>` | o mesmo canto |
| abrir um pull request | `gh pr create` | no site do GitHub, botão **Compare & pull request** |
| ver o pull request | `gh pr view --web` | no site do GitHub |

## Mensagem de commit

Diga o que mudou, e não o que você fez: `trilha: diário com o ensaio da entrevista`, e não
`atualizações`.

## Nunca

- `git push --force`: apaga o que outra pessoa mandou.
- `git reset --hard`: apaga o que você não salvou.
- Commit direto na `main`.
