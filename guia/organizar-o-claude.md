# Como organizar o seu Claude

O Claude não lembra das conversas anteriores. Tudo o que ele sabe de você no começo de uma conversa
vem de arquivos que você escreveu. Organizar o Claude é decidir o que vai em cada arquivo. Esse
conjunto de arquivos (instruções, skills e regras) se chama **harness**. O seu fica num
repositório privado no seu GitHub, o `espaco-ni`, que a etapa 4 cria.

## As camadas

| Camada | Arquivo | Quando o Claude lê | O que vai nele | Onde fica guardado |
| --- | --- | --- | --- | --- |
| Computador | `~/.claude/CLAUDE.md` | toda conversa, em qualquer pasta | quem você é, os objetivos em uma linha cada, como trabalhar com você | no computador, com cópia em `espaco-ni/eu/` |
| Espaço | `~/NI/CLAUDE.md` | toda conversa dentro de `~/NI` | os projetos, onde guardar cada coisa, as regras do espaço | `espaco-ni` |
| Você, em detalhe | `~/NI/eu/sobre-mim.md` e `~/NI/eu/objetivos.md` | quando o pedido precisa: estudo, semana, prioridade | matérias, atividades, semana, interesses; objetivos com medida, prazo e próximo passo | `espaco-ni` |
| Projeto | `~/NI/<projeto>/CLAUDE.md` | quando o Claude mexe naquele projeto | o que é, o objetivo que ele move, prazo, com quem, o que já se sabe | `espaco-ni` |
| Skills | `~/NI/.claude/skills/<nome>/SKILL.md` | quando você digita `/<nome>` ou o pedido combina com a descrição | um pedido que você repete, com os passos | `espaco-ni` |
| Regras | `~/NI/.claude/settings.json` | sempre, dentro de `~/NI` | os comandos liberados e os bloqueados | `espaco-ni` |
| Trilha | `~/NI/trilha-claude/` | durante a trilha | as etapas e a sua pasta na turma | repositório do time |
| claude.ai | preferências do perfil e Projeto "Treinamento NI" | no navegador e no celular | um resumo de você e do NI | na sua conta do Claude |

## O que vai onde

- **Vale em qualquer conversa?** `~/.claude/CLAUDE.md`. Mantenha curto: o Claude lê o arquivo
  inteiro em toda conversa, e isso gasta o limite de uso.
- **Só vale dentro de um projeto?** O `CLAUDE.md` do projeto.
- **É detalhe que só às vezes importa?** Um arquivo à parte, com uma linha no `CLAUDE.md` dizendo
  quando ler. É o caso de `sobre-mim.md` e `objetivos.md`.
- **Você pediu a mesma coisa duas vezes?** Vira skill (etapa 6).
- **O Claude fez algo que não devia?** Uma linha em "Como trabalhar comigo". Se foi um comando, uma
  regra no `settings.json`.

## Manter em dia

| Quando | O que fazer |
| --- | --- |
| no fim de uma conversa em que algum arquivo mudou | `/salvar` |
| toda semana | `/objetivos` |
| mudou de card | "mudei de card, atualiza": o Claude mexe no `~/.claude/CLAUDE.md` e no `CLAUDE.md` do treinamento |
| começou um semestre | atualize `eu/sobre-mim.md` e escreva os objetivos novos |
| o Claude errou do mesmo jeito duas vezes | escreva a regra no `CLAUDE.md` certo |

## Sinais de que o harness precisa de ajuste

- Você repete no chat o que já devia estar num arquivo.
- A resposta é genérica, serviria para qualquer pessoa.
- Um `CLAUDE.md` passou de uma página. Separe o detalhe num arquivo à parte.
- Uma skill não sai como você queria. Abra o `SKILL.md` e reescreva o passo que falhou.

## Num computador novo

O `README.md` do seu `espaco-ni` tem os quatro passos. Em resumo: instalar o que a trilha instala,
clonar o `espaco-ni` em `~/NI` e pedir ao Claude para copiar `eu/claude-do-computador.md` para
`~/.claude/CLAUDE.md`.

## Depois da trilha

Com o básico rodando, dá para ir além:

- **hooks:** comandos que rodam sozinhos em certos momentos, como ao fechar uma conversa;
- **conectores:** o Claude lendo o Google Drive, a agenda ou o ValidaNI;
- **um diário por projeto:** o que mudou, o que deu errado e o próximo passo, uma entrada por dia
  de trabalho.

Antes de ligar um conector que lê dado do NI, fale com o Bruno.
