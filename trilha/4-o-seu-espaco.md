# Etapa 4: O seu espaço, no seu GitHub

**Tempo:** 30 minutos.
**Você sai sabendo:** montar uma pasta por projeto, cada uma com o seu `CLAUDE.md`, e guardar o seu
jeito de trabalhar com o Claude num repositório seu. É assim que os PMs do NI trabalham.

## A ideia

O Claude lê o `CLAUDE.md` da pasta que você abriu e os das pastas acima dela, e as skills que estão
em `.claude/skills/` dessa pasta. Então o seu espaço fica assim:

```
~/NI/                     o seu espaço: é esta pasta que você abre no VS Code no dia a dia
├── CLAUDE.md             o mapa: os seus projetos, onde guardar cada coisa e as regras
├── README.md             o que tem aqui e como recuperar num computador novo
├── eu/                   sobre-mim.md, objetivos.md e a cópia do ~/.claude/CLAUDE.md
├── .claude/
│   ├── skills/           as suas skills: as seis de uso, salvar, objetivos e, na etapa 6, a sua
│   └── settings.json     o que o Claude pode e não pode fazer aqui
├── treinamento/
│   └── CLAUDE.md         o que é, objetivo, prazo, dupla, onde estão as coisas
├── estudos/
│   └── CLAUDE.md
└── trilha-claude/        esta trilha: repositório do time, fica de fora do seu
```

Essa pasta vira um repositório privado no seu GitHub, o `espaco-ni`. Só você vê. Se você trocar de
computador, o seu Claude volta inteiro: é clonar o `espaco-ni` e copiar um arquivo. Esse conjunto de
instruções, skills e regras é o seu **harness**.

## Roteiro para o Claude

1. Explique a árvore acima em até cinco linhas. Diga que, a partir de agora, são dois repositórios:
   a trilha, do time, e o espaço, dela.
2. **Projetos.** Pergunte que projetos ela quer ter agora. Sugestão de partida: `treinamento` e
   `estudos`, no máximo três. Os nomes são dela: não recomende nenhum. O `~/NI/eu/sobre-mim.md`
   serve para lembrar do que existe na vida dela (as matérias que mais pesam, uma atividade de
   fora), não para decidir por ela.
3. Para cada projeto, faça uma entrevista curta: o que é, qual objetivo de `eu/objetivos.md` ele
   move, o prazo, com quem, onde estão as coisas (link do card, documentos) e como ela quer ajuda
   ali. Crie a pasta e o `CLAUDE.md` a partir de `modelos/claude-do-projeto.md`. Mostre antes de
   salvar.
4. **O mapa.** Crie `~/NI/CLAUDE.md` a partir de `modelos/claude-do-espaco.md`, com a tabela dos
   projetos, e `~/NI/README.md` a partir de `modelos/espaco/README.md`. Mostre os dois.
5. **Skills e regras.** Explique que uma skill é um pedido pronto, guardado num arquivo, que vira
   comando com `/`. Copie:
   - as oito pastas de `skills/` para `~/NI/.claude/skills/`;
   - `modelos/espaco/settings.json` para `~/NI/.claude/settings.json`;
   - `modelos/espaco/gitignore` para `~/NI/.gitignore`;
   - `~/.claude/CLAUDE.md` para `~/NI/eu/claude-do-computador.md`.

   Explique cada skill em uma linha:
   - `/discutir`: atacar uma ideia sua e achar como testá-la;
   - `/ensaiar`: treinar uma entrevista com o Claude no papel do entrevistado;
   - `/revisar`: apontar os problemas de um texto seu antes de ele sair;
   - `/explicar`: aprender um conceito e ser testado nele;
   - `/pesquisar`: buscar um número ou um fato com fonte;
   - `/ata`: transformar anotação de conversa em ata, sem dado pessoal;
   - `/salvar`: guardar o espaço no GitHub;
   - `/objetivos`: revisar os objetivos e escrever o próximo passo de cada um.

   Explique em duas linhas o `settings.json` (libera os comandos que só leem, bloqueia os que
   apagam histórico ou tornam o repositório público) e o `.gitignore` (deixa a trilha e os segredos
   de fora).
6. **O repositório.** Em `~/NI`, um comando por vez, explicando cada um:
   - `git init -b main`: transforma a pasta num repositório;
   - `git status`: mostre que `trilha-claude/` não aparece. Se aparecer, pare e confira o
     `.gitignore`;
   - `git add -A` e `git commit -m "espaço: primeira versão"`;
   - `gh repo create espaco-ni --private --source . --remote origin --push`: cria o repositório na
     conta dela, privado, e manda o primeiro commit.

   Peça que ela rode `gh repo view espaco-ni --web` e confira que aparece **Private** ao lado do
   nome.
7. Marque a etapa 4 em `progresso.md` e rode a skill `salvar` da trilha
   (`.claude/skills/salvar/SKILL.md`).
8. **Abrir o espaço.** Ela abre `~/NI` numa janela nova do VS Code (**File → Open Folder**). Se o
   VS Code ou o Claude perguntarem se ela confia na pasta, a resposta é sim: a pasta é dela. Ela
   abre o Claude ali. Daqui em diante, ela trabalha por essa janela, e a trilha continua nela: o
   `CLAUDE.md` do espaço manda o Claude seguir a trilha até a etapa 7. O painel **Source Control**
   passa a mostrar dois repositórios, o `NI` e o `trilha-claude`.
9. **Teste**, já na janela de `~/NI`: perguntar "Quais são os meus projetos e qual objetivo cada um
   move?" e digitar `/` para ver as skills na lista.

## Pronto quando

- [ ] `~/NI/CLAUDE.md` existe, com a tabela dos projetos e o objetivo que cada um move.
- [ ] Cada projeto tem a sua pasta e o seu `CLAUDE.md`, revisados por ela.
- [ ] O `espaco-ni` está no GitHub dela, privado, sem a pasta `trilha-claude`.
- [ ] Na janela de `~/NI`, as oito skills aparecem quando ela digita `/`, e o Claude listou os
      projetos dela.
