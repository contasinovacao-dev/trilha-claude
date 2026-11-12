# Etapa 3: O Claude fora do VS Code

**Tempo:** 15 minutos.
**Você sai sabendo:** usar o Claude no navegador e no celular com o contexto do treinamento, e onde
cada um guarda o que sabe de você.

## A ideia

A sua conta do Claude funciona em três lugares, e cada um lembra de um jeito:

| Onde | Bom para | O que ele sabe de você |
| --- | --- | --- |
| VS Code (Claude Code) | trabalhar com arquivos: escrever, organizar, pesquisar e salvar | os `CLAUDE.md` do seu computador |
| claude.ai, no navegador ou no app do computador | conversa rápida, ler um PDF, discutir uma ideia | as preferências do perfil, as instruções do Projeto e a memória que ele gera das conversas |
| app do celular | ensaiar uma entrevista por voz, revisar uma mensagem antes de mandar | o mesmo do claude.ai |

As conversas do VS Code ficam só no seu computador. As do claude.ai ficam na sua conta.

O limite de uso é um só para os três: o que você gasta no celular sai do mesmo saldo do VS Code. Há
um limite por janela de cinco horas e outro por semana. No VS Code, `/usage` mostra quanto já foi.

## Roteiro para o Claude

1. Explique a tabela e o limite em até cinco linhas.
2. **Preferências do perfil.** Monte o texto a partir de `modelos/preferencias-do-perfil.md`, com o
   que está no `~/.claude/CLAUDE.md`. Mostre, ajuste com ela e peça que ela abra claude.ai →
   **Configurações → Perfil** e cole no campo de preferências. Explique que esse texto vale para toda
   conversa no claude.ai.
3. **O Projeto do treinamento.** Ela cria, no claude.ai, um Projeto chamado "Treinamento NI".
   - Monte as instruções a partir de `modelos/projeto-no-claude-ai.md` e mostre.
   - Ela cola em **Instruções do projeto** e anexa o arquivo `contexto/nucleo.md`, que está na pasta
     da trilha.
   - Explique: conversa sobre o treinamento começa dentro do Projeto, e cada Projeto tem uma memória
     separada da do resto da conta.
4. **Memória.** Ela abre as configurações do claude.ai e confere se a memória gerada das conversas
   está ligada. Explique que dá para ver e corrigir o que ele lembra, e desligar a memória numa
   conversa só.
5. **Celular.** Ela instala o app do Claude, entra com a mesma conta e abre o Projeto. Sugira testar
   a conversa por voz com uma pergunta do card dela.
6. **Teste.** Dentro do Projeto, numa conversa nova: "Em que eu estou trabalhando no treinamento e
   como você deve me ajudar?". A resposta tem de bater com as instruções.
7. Marque a etapa 3 em `progresso.md` e rode a skill `salvar`.

Você não enxerga o claude.ai. Nos passos 2 a 6, quem confere é ela: peça que diga o que apareceu.

## Pronto quando

- [ ] As preferências do perfil estão salvas no claude.ai.
- [ ] O Projeto "Treinamento NI" existe, com as instruções e o `nucleo.md`.
- [ ] O app do celular está instalado e abre o Projeto.
- [ ] O teste do passo 6 respondeu certo.
