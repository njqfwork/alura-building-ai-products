# O agente consulta a base

Cole na ferramenta de construção, com a IA já funcionando e alguns casos registrados: com a base vazia não dá para ver o efeito. No colchete, o nome que o seu produto dá ao que a IA escolhe, como categoria, área ou critério. Depois, acrescente na parte 4 da sua ficha: "Consultar casos parecidos já decididos: use quando o texto for ambíguo, curto demais, ou citar algo que você não reconhece." Para conferir, mande um caso parecido com um que já existe e veja quais itens ele consultou.

```
Quero que o agente olhe o que já foi decidido antes de decidir um caso novo.

Faça o seguinte:
1. Antes de chamar o modelo, busque na tabela até 3 itens já decididos que
   tenham a ver com o texto novo.
2. Mande esses itens junto com a ficha e o caso novo, na mesma chamada.
3. Mostre na tela quais itens foram consultados, junto com a decisão.
4. Mostre também quantos casos daquela mesma [categoria] já existem na base.

Se a base ainda estiver vazia, o agente decide sem consulta, e a tela diz isso.

Antes de construir, liste o que você vai fazer e espere minha confirmação.
```
