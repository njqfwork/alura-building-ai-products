# Aula 1 · Da ideia ao primeiro produto com IA

**Você sai com:** uma especificação de uma página, em sete campos, e o app publicado, com link próprio. A decisão da IA ainda é simulada: o app mostra um resultado de exemplo, com aviso na tela.

## O caminho

1. **Escreva a especificação** no [modelo em branco](modelos/especificacao-em-branco.md), campo por campo: problema e público, proposta de valor, escopo (o que fica dentro e o que fica fora), fluxo principal, componentes, papel da IA e critério de pronto. Sem ideia? Use um dos [exemplos](exemplos/).
2. **Traduza a especificação num prompt de construção**, no chat de IA, com o [prompt 01](prompts/01-traducao.md). Leia o último bloco da resposta, que lista o que a IA decidiu sozinha, corrija o que não quiser e apague ele.
3. **Construa a primeira versão** num Replit App novo, com o [prompt 02](prompts/02-construcao.md). Leia o plano antes de confirmar. Se aparecer tarefa que você não pediu, use o [prompt 03](prompts/03-cortar-o-plano.md).
4. **Corrija** com o [molde de correção](prompts/04-correcao.md), uma correção por mensagem. Para testar, use [textos de exemplo](exemplos/vertice-textos-para-testar.md) ou textos do seu produto.
5. **Publique** pelo Replit. Abra o link numa janela anônima, faça o fluxo inteiro e confira o seu critério de pronto.

## Prompts

| Arquivo | Quando | Onde colar |
|---|---|---|
| [01-traducao.md](prompts/01-traducao.md) | Com os sete campos preenchidos | Chat de IA |
| [02-construcao.md](prompts/02-construcao.md) | Para construir a primeira versão | Ferramenta de construção |
| [03-cortar-o-plano.md](prompts/03-cortar-o-plano.md) | Se o plano trouxer algo que você não pediu | Ferramenta de construção |
| [04-correcao.md](prompts/04-correcao.md) | A cada correção, nesta aula e nas próximas | Ferramenta de construção |
| [05-base-sintetica.md](prompts/05-base-sintetica.md) | Tarefa para a Aula 2 | Chat de IA |

## Outros arquivos

| Arquivo | O que é |
|---|---|
| [modelos/especificacao-em-branco.md](modelos/especificacao-em-branco.md) | Os sete campos, para preencher |
| [exemplos/ideia-feedback.md](exemplos/ideia-feedback.md) | Especificação pronta: análise de feedback de clientes |
| [exemplos/ideia-planejamento.md](exemplos/ideia-planejamento.md) | Especificação pronta: planejamento para pequenos negócios |
| [exemplos/ideia-validacao.md](exemplos/ideia-validacao.md) | Especificação pronta: validação de ideias de produto |
| [exemplos/vertice-especificacao.md](exemplos/vertice-especificacao.md) | A especificação do Vértice, usada na aula |
| [exemplos/vertice-textos-para-testar.md](exemplos/vertice-textos-para-testar.md) | Textos para testar o app do Vértice |
| [exemplos/vertice-base-sintetica.csv](exemplos/vertice-base-sintetica.csv) | Exemplo de base sintética, com 40 feedbacks |

## Tarefa até a Aula 2

1. Crie uma conta no [Google AI Studio](https://aistudio.google.com). A chave você cria na Aula 2.
2. Gere a sua base sintética com o [prompt 05](prompts/05-base-sintetica.md) e guarde o arquivo CSV.
