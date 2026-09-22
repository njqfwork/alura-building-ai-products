# Aula 2 · Construindo agentes inteligentes na prática

**Você sai com:** os dados guardados num banco, a ficha do agente escrita e calibrada, e a IA decidindo de verdade dentro do app, consultando o que já foi decidido antes.

## O caminho

1. **Mude as regras do projeto** com o [prompt 01](prompts/01-regras.md). As regras da Aula 1 proibiam banco e IA. Se ficarem, a ferramenta recusa o que vem a seguir.
2. **Guarde os dados num banco** com o [prompt 03](prompts/03-banco.md). Se não souber o que listar, antes use o [prompt 02](prompts/02-o-que-guardar.md) no chat de IA. Para conferir, registre algo e recarregue a página: o registro tem que continuar lá. Depois, carregue a sua base sintética.
3. **Escreva a ficha do agente** no [modelo em branco](modelos/ficha-do-agente-em-branco.md). São seis partes: identidade, o que ele recebe, como ele decide, o que ele pode fazer, o que faz quando não tem certeza e o que ele devolve. A parte 3 é a mais importante. Veja a [ficha do Vértice](exemplos/vertice-ficha.md) como exemplo. Se travar, use o [prompt 04](prompts/04-escrever-ficha.md).
4. **Calibre a ficha** numa conversa nova do chat de IA, com o [prompt 05](prompts/05-calibrar-ficha.md). Salve a ficha reescrita por cima da sua.
5. **Crie a chave do modelo** seguindo o [passo a passo](modelos/chave-do-modelo.md), e **ligue a ficha ao app** com o [prompt 06](prompts/06-ia-no-app.md).
6. **Teste os limites.** Mande um caso fora do assunto do seu produto, que deve cair na saída de dúvida, e um caso ambíguo. Se algum limite falhar, corrija a ficha, não o código.
7. **Faça o agente consultar a base** com o [prompt 07](prompts/07-consultar-base.md). O modelo passa a responder com os seus dados, e não só com o que aprendeu antes. Isso se chama RAG.
8. **MCP**, só conceito, sem construção: veja [o resumo](conceitos/mcp.md).

## Prompts

| Arquivo | Quando | Onde colar |
|---|---|---|
| [01-regras.md](prompts/01-regras.md) | Antes de tudo | Ferramenta de construção |
| [02-o-que-guardar.md](prompts/02-o-que-guardar.md) | Só se não souber o que o banco guarda | Chat de IA |
| [03-banco.md](prompts/03-banco.md) | Para criar o banco | Ferramenta de construção |
| [04-escrever-ficha.md](prompts/04-escrever-ficha.md) | Só se travar no rascunho da ficha | Chat de IA, conversa nova |
| [05-calibrar-ficha.md](prompts/05-calibrar-ficha.md) | Com a ficha escrita | Chat de IA, conversa nova |
| [06-ia-no-app.md](prompts/06-ia-no-app.md) | Com a chave criada | Ferramenta de construção |
| [07-consultar-base.md](prompts/07-consultar-base.md) | Com a IA funcionando e alguns casos na base | Ferramenta de construção |

## Outros arquivos

| Arquivo | O que é |
|---|---|
| [modelos/ficha-do-agente-em-branco.md](modelos/ficha-do-agente-em-branco.md) | As seis partes da ficha, para preencher |
| [modelos/chave-do-modelo.md](modelos/chave-do-modelo.md) | Como criar a chave gratuita do Gemini |
| [exemplos/vertice-ficha.md](exemplos/vertice-ficha.md) | A ficha do agente do Vértice |
| [conceitos/mcp.md](conceitos/mcp.md) | O que é MCP, e onde ele aparece no curso |

## Tarefa até a Aula 3

1. Use o seu produto mais dez vezes ao longo da semana.
2. Anote cinco erros: o texto e a resposta que você esperava.
3. Traga essa lista para a Aula 3.
