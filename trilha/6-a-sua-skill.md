# Etapa 6: A sua skill

**Tempo:** 15 minutos, até segunda, 16/11.
**Você sai sabendo:** transformar um pedido que você repete num comando seu.

## A ideia

Se você pediu a mesma coisa duas vezes, escreva o pedido uma vez num arquivo. Uma skill é uma pasta
em `~/.claude/skills/<nome>/` com um arquivo `SKILL.md`: em cima, o nome e quando usar; embaixo, os
passos. As seis que você instalou na etapa 4 mostram o formato.

## Roteiro para o Claude

1. Leia o diário dela e pergunte que pedido ela repetiu ou vai repetir. Exemplos: preparar a pauta
   da reunião da dupla; conferir se a mensagem para a escola segue o roteiro; montar a lista de
   escolas no formato do card.
2. Ela escreve os passos com as palavras dela, no chat. Você pergunta o que falta (quando usar, o que
   entra, o que sai, o que nunca fazer) e arruma o formato a partir de `modelos/skill.md`. Os passos
   continuam sendo os dela.
3. Salve em `~/.claude/skills/<nome>/SKILL.md` e copie para `trainees/<pasta>/skill/SKILL.md` na
   trilha, para o Bruno ver.
4. Ela testa numa conversa nova, digitando `/<nome>`. Se o resultado não sair como ela queria,
   ajustem juntos uma vez.
5. Ela registra no diário. Rode a skill `salvar`.

## Pronto quando

- [ ] A skill dela funciona com `/<nome>` numa conversa nova.
- [ ] A cópia está em `trainees/<pasta>/skill/` e foi enviada ao GitHub.
