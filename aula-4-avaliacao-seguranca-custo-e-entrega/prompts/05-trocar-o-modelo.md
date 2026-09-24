# Trocar o modelo quando der erro 429

Use se aparecer **erro 429** ao rodar a avaliação ou ao usar o app. O 429 não é falha do seu código: é o limite de chamadas do plano gratuito, que existe por minuto e por dia. Primeiro, espere um minuto e tente de novo. Se continuar, troque de modelo: o limite é contado por modelo, então o `gemini-3.5-flash-lite` tem um limite separado, e ele é feito justamente para muitas chamadas seguidas. Os seus limites do momento aparecem no painel do Google AI Studio, em Rate limits. Depois de trocar, rode a avaliação de novo: o placar pode mudar um pouco, porque é outro modelo, e isso é esperado. Anote no campo do que mudou que você trocou o modelo, senão daqui a um mês a queda na nota vira mistério.

```
Troque o modelo usado pelo agente para gemini-3.5-flash-lite, mantendo a
mesma chave e a mesma ficha. Não mude mais nada.
```
