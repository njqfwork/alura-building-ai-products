# O registro de custo

Cole na ferramenta de construção com a IA já funcionando, e depois da página de avaliação, porque a tela de custo entra dentro da mesma área de administração. Os números de tokens vêm da própria resposta da API, não de estimativa. A tabela de preços fica editável porque o preço do modelo muda: confira em [ai.google.dev/gemini-api/docs/pricing](https://ai.google.dev/gemini-api/docs/pricing). No plano gratuito o gasto real é zero, e o número da tela é quanto custaria no plano pago. O último item põe um limite de chamadas por pessoa por dia: sem ele, qualquer pessoa com o link roda o agente o dia inteiro, e cada clique é uma chamada paga. Para conferir, rode a avaliação inteira e veja o contador subir de uma vez.

```
Quero saber quanto custa cada uso do produto.

1. A cada chamada ao modelo, grave uma linha no banco com: data e hora, o
   que foi pedido, tokens de entrada, tokens de saída e tempo de resposta.
   Os números de tokens vêm da própria resposta da API.
2. Uma página de custo dentro da mesma área de administração que já existe,
   com três números: quantas chamadas, o custo estimado e o tempo médio de
   resposta.
3. Para calcular o custo, use uma tabela de preços que eu possa editar, com
   o preço por milhão de tokens de entrada e de saída.
4. Mostre também o custo médio de um uso, e quanto custariam mil usos.
5. Um limite de chamadas ao modelo por pessoa por dia. Ao passar do limite,
   mostre um aviso em vez de chamar o modelo.

Deixe claro na tela que é um custo estimado, com o preço do plano pago.

Antes de construir, liste o que você vai fazer e espere minha confirmação.
```
