# Etapa 4: O seu espaço, no seu GitHub

**Tempo:** 20 minutos.
**Você sai sabendo:** guardar a pasta que o Claude montou num repositório privado seu, passar a
trabalhar nela e usar os comandos prontos que vieram com ela. É assim que os PMs do NI trabalham.

## A ideia

Na etapa 1, o Claude montou a pasta `~/NI`. Agora, com os nomes técnicos:

```
~/NI/                     o seu espaço: é esta pasta que você abre no VS Code no dia a dia
├── CLAUDE.md             o mapa: as suas pastas, onde guardar cada coisa e as regras
├── README.md             o que tem aqui e por quê, sem palavra técnica
├── eu/                   sobre-mim.md, objetivos.md e a cópia do ~/.claude/CLAUDE.md
├── .claude/
│   ├── skills/           os comandos prontos: os seis de uso, salvar, objetivos e, na etapa 6, o seu
│   └── settings.json     o que o Claude pode e não pode fazer aqui
├── treinamento/
│   └── CLAUDE.md         o card, a dupla e como o Claude ajuda
├── faculdade/
│   └── CLAUDE.md         as matérias, tiradas do print da grade
└── trilha-claude/        esta trilha: repositório do time, fica de fora do seu
```

O Claude lê o `CLAUDE.md` da pasta que você abriu e os das pastas acima dela, e as skills que estão
em `.claude/skills/` dessa pasta. Esse conjunto de instruções, skills e regras é o seu **harness**.

Agora a pasta vira um repositório privado no seu GitHub, o `espaco-ni`. Só você vê. Se você trocar
de computador, o seu Claude volta inteiro: é clonar o `espaco-ni` e copiar um arquivo.

## Roteiro para o Claude

1. Explique a árvore acima em até cinco linhas, ligando ao que você mostrou na etapa 1: as
   anotações são os `CLAUDE.md`, os comandos prontos são as skills. Diga que, a partir de agora, são
   dois repositórios: a trilha, do time, e o espaço, dela.
2. **Conferir o espaço.** Veja se `~/NI` tem tudo o que o passo 7 da etapa 1 monta. Quem fez a
   etapa 1 antes de 2026-11-18 tem só `~/.claude/CLAUDE.md` e `~/NI/eu/`: complete agora.
   - Monte o que falta a partir dos modelos, com o que já está em `~/.claude/CLAUDE.md` e em
     `~/NI/eu/`. Não refaça a entrevista. Se faltar algo para a pasta `treinamento/` (o card de
     agora, por exemplo), pergunte só isso, uma pergunta por vez.
   - Se ela tinha objetivos de faculdade ou pessoais, não apague: pergunte se ela quer manter ou
     ficar só com o do NI.
   - A pasta `faculdade/` só se ela quiser: aí, peça o print da grade como no passo 3 da etapa 1.
   - Depois, mostre como ficou com o passo 8 da etapa 1, sem palavra técnica.
3. **Skills e regras.** Explique que uma skill é um pedido pronto, guardado num arquivo, que vira
   comando com `/`. Explique cada uma em uma linha:
   - `/discutir`: atacar uma ideia sua e achar como testá-la;
   - `/ensaiar`: treinar uma entrevista com o Claude no papel do entrevistado;
   - `/revisar`: apontar os problemas de um texto seu antes de ele sair;
   - `/explicar`: aprender um conceito e ser testado nele;
   - `/pesquisar`: buscar um número ou um fato com fonte;
   - `/ata`: transformar anotação de conversa em ata, sem dado pessoal;
   - `/salvar`: guardar o espaço no GitHub;
   - `/objetivos`: revisar o objetivo e escrever o próximo passo.

   Explique em duas linhas o `settings.json` (libera os comandos que só leem, bloqueia os que
   apagam histórico ou tornam o repositório público) e o `.gitignore` (deixa a trilha e os segredos
   de fora).
4. **O repositório.** Em `~/NI`, um comando por vez, explicando cada um:
   - `git init -b main`: transforma a pasta num repositório;
   - `git status`: mostre que `trilha-claude/` não aparece. Se aparecer, pare e confira o
     `.gitignore`;
   - `git add -A` e `git commit -m "espaço: primeira versão"`;
   - `gh repo create espaco-ni --private --source . --remote origin --push`: cria o repositório na
     conta dela, privado, e manda o primeiro commit.

   Peça que ela rode `gh repo view espaco-ni --web` e confira que aparece **Private** ao lado do
   nome.
5. Marque a etapa 4 em `progresso.md` e rode a skill `salvar` da trilha
   (`.claude/skills/salvar/SKILL.md`).
6. **Abrir o espaço.** Ela abre `~/NI` numa janela nova do VS Code (**File → Open Folder**). Se o
   VS Code ou o Claude perguntarem se ela confia na pasta, a resposta é sim: a pasta é dela. Ela
   abre o Claude ali. Daqui em diante, ela trabalha por essa janela, e a trilha continua nela: o
   `CLAUDE.md` do espaço manda o Claude seguir a trilha até a etapa 7. O painel **Source Control**
   passa a mostrar dois repositórios, o `NI` e o `trilha-claude`.
7. **Teste**, já na janela de `~/NI`: perguntar "O que tem no meu espaço e em que eu estou
   trabalhando?" e digitar `/` para ver as skills na lista.

## Pronto quando

- [ ] `~/NI` tem tudo o que o passo 7 da etapa 1 monta.
- [ ] O `espaco-ni` está no GitHub dela, privado, sem a pasta `trilha-claude`.
- [ ] Na janela de `~/NI`, as oito skills aparecem quando ela digita `/`, e o Claude disse o que tem
      no espaço e em que ela está trabalhando.
