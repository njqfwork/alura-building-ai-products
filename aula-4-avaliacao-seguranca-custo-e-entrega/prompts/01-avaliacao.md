# A página de avaliação

Cole na ferramenta de construção depois de escrever os três casos no [modelo de gabarito](../modelos/gabarito-em-branco.md). Esta página é o seu laboratório daqui para frente: é nela que moram o gabarito e o histórico das notas. Ela nasce dentro de uma área de administração, que só a sua conta abre. Troque `[seu email]` pelo email com que você entra no app, o mesmo da conta que você criou na Aula 3: sem dizer quem é o dono, a ferramenta não tem como saber. A marca de administradora fica no banco, na linha daquela conta, e não escrita no código. Assim, trocar de administrador depois é mudar uma linha, e se você errar o email agora, o conserto é ali, sem refazer o pedido. E pedir só uma página escondida não basta, porque esconder o link não protege nada, como vimos na Aula 3. A regra de quem entra fica no servidor, e a tela de custo do prompt 03 vai morar na mesma área. A tela usa o mesmo agente que o app já usa: se ela chamasse outro, o placar não diria nada sobre o seu produto. O campo do que mudou, no item 3, é o que transforma o histórico em algo legível meses depois: sem ele, você tem uma lista de números sem causa. O item 8 existe só para poupar clique quando a decisão é uma palavra: a marcação continua sendo sua. Quem dá a nota é você, caso a caso: o agente responde, e quem marca passou ou não é quem escreveu o gabarito. O motivo que você escreve em cada falha é o material da correção seguinte, porque ele vira uma regra na ficha do agente. Os itens 14 e 15 existem por um motivo prático: o plano gratuito tem limite de chamadas, e uma chamada que falha não pode virar falha do agente, senão o placar mente. Para conferir, mude uma linha da ficha do agente e rode de novo: o placar tem que mudar, e a rodada nova tem que aparecer no histórico.

```
Quero uma área de administração no app, e dentro dela uma página de
avaliação do agente. É nessa página que eu testo o agente e guardo o
histórico.

A área de administração
1. A dona dela é a conta do email [seu email]. Marque essa conta como
   administradora no banco, e é essa marca que a regra olha.
2. Só essa conta enxerga a área. Quem não for ela não vê o menu, e se
   digitar o endereço direto recebe uma negativa. Essa regra fica no
   servidor, não só na tela.

Os casos
3. Guarde uma lista de casos. Cada caso tem o texto de entrada, a decisão
   que eu espero, e uma linha dizendo por que ele está na lista.
4. Posso acrescentar casos a qualquer momento, e a lista nunca é apagada.

A rodada
5. Antes de rodar, um campo para eu escrever o que mudei desde a última vez.
6. Um botão Rodar avaliação passa todos os casos pelo mesmo agente que o app
   já usa hoje.
7. Guarde cada rodada: a data, o que eu escrevi que mudei, o placar, e a
   resposta do agente em cada caso.

A marcação
8. Quem marca passou ou não passou sou eu, caso a caso, olhando o esperado
   ao lado da resposta.
9. Em cada caso, um campo para eu escrever em uma linha por que marquei
   assim. Guarde esse motivo junto da rodada.
10. Quando o esperado for uma palavra só, pode já sugerir passou ou não,
    ignorando maiúsculas, acentos e pontuação. A marcação final é sempre
    minha, e eu posso trocar.

A tela
11. No topo, o placar da última rodada: quantos passaram, de quantos.
12. Abaixo, os casos lado a lado: entrada, esperado, resposta do agente,
    a marcação e o motivo.
13. Depois, o histórico das rodadas, da mais nova para a mais antiga, com
    data, placar e o que mudou. Marque a rodada em que um caso que vinha
    passando começou a falhar.

Quando algo falhar
14. Rode um caso por vez, nunca todos ao mesmo tempo.
15. Se a chamada ao modelo falhar, espere alguns segundos e tente mais uma
    vez. Se falhar de novo, mostre erro na chamada naquele caso, e não conte
    como falha do agente: erro de chamada não entra no placar.

O agente nunca julga a própria resposta. Ele só responde os casos.

Antes de construir, liste o que você vai fazer e espere minha confirmação.
```
