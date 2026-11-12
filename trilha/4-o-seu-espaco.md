# Etapa 4: O seu espaço de trabalho

**Tempo:** 20 minutos.
**Você sai sabendo:** montar uma pasta por projeto, cada uma com o seu `CLAUDE.md`, para o Claude
entrar em cada projeto sabendo do que se trata. É assim que os PMs do NI trabalham.

## A ideia

O Claude lê o `CLAUDE.md` da pasta que você abriu e os das pastas acima dela. Então o seu espaço
fica assim:

```
~/NI/                     o seu espaço: é esta pasta que você abre no VS Code no dia a dia
├── CLAUDE.md             o mapa: os seus projetos e onde guardar cada coisa
├── trilha-claude/        esta trilha (repositório do time)
├── treinamento/          o seu trabalho no treinamento agora
│   └── CLAUDE.md         o que é, prazo, dupla, onde estão as coisas
└── estudos/              o que você está aprendendo
    └── CLAUDE.md
```

Fora a trilha, o que está em `~/NI` é só seu: fica no seu computador e não vai para o GitHub.

## Roteiro para o Claude

1. Explique a árvore acima em até quatro linhas.
2. Pergunte que projetos ela quer ter agora. Sugestão de partida: `treinamento` e `estudos`, no
   máximo três. Os nomes são dela: não recomende nenhum.
3. Para cada projeto, faça uma entrevista curta: o que é, o objetivo, o prazo, com quem, onde estão
   as coisas (link do card, documentos) e como ela quer ajuda ali. Crie a pasta e o `CLAUDE.md` a
   partir de `modelos/claude-do-projeto.md`. Mostre antes de salvar.
4. Crie `~/NI/CLAUDE.md` a partir de `modelos/claude-do-espaco.md`, com a tabela dos projetos.
5. **Skills.** Explique que uma skill é um pedido pronto, guardado num arquivo, que vira comando com
   `/`. Copie as seis de `skills/` para `~/.claude/skills/` (crie a pasta se não existir). Explique
   cada uma em uma linha:
   - `/discutir`: atacar uma ideia sua e achar como testá-la;
   - `/ensaiar`: treinar uma entrevista com o Claude no papel do entrevistado;
   - `/revisar`: apontar os problemas de um texto seu antes de ele sair;
   - `/explicar`: aprender um conceito e ser testado nele;
   - `/pesquisar`: buscar um número ou um fato com fonte;
   - `/ata`: transformar anotação de conversa em ata, sem dado pessoal.
6. Marque a etapa 4 em `progresso.md` e rode a skill `salvar`.
7. **Abrir o espaço.** Ela abre `~/NI` numa janela nova do VS Code (**File → Open Folder**) e abre o
   Claude ali. Daqui em diante, ela trabalha por essa janela, e a trilha continua nela: o
   `CLAUDE.md` do espaço manda o Claude seguir a trilha até a etapa 7.
8. **Teste**, já na janela de `~/NI`: perguntar "Quais são os meus projetos e o que tem em cada
   um?" e digitar `/` para ver as skills na lista.

## Pronto quando

- [ ] `~/NI/CLAUDE.md` existe, com a tabela dos projetos.
- [ ] Cada projeto tem a sua pasta e o seu `CLAUDE.md`, revisados por ela.
- [ ] As seis skills aparecem quando ela digita `/`.
- [ ] Na janela de `~/NI`, o Claude listou os projetos dela.
