# Traduzir a especificação em prompt de construção

Cole no seu chat de IA, com a sua especificação de sete campos no lugar do colchete do fim. A resposta vem em nove blocos. Os oito primeiros vão para a ferramenta de construção. O nono lista o que a IA decidiu sozinha, porque a sua especificação não dizia: leia, corrija o que não quiser e apague esse bloco antes de seguir.

```
Você vai traduzir a especificação de produto abaixo em um prompt de construção
para uma ferramenta de desenvolvimento assistido por IA.

Regras:
- Use apenas o que está na especificação. Não acrescente funcionalidade.
- Onde a especificação não disser, escolha a opção mais simples e anote no último bloco.
- Esta versão não tem banco de dados, login nem chamada a serviço de IA.
- Onde a especificação previr uma decisão da IA, ela é simulada: decidida no
  próprio aplicativo, sem serviço externo, e com aviso na tela.
- A simulação não tenta acertar. Ela só produz resultados diferentes conforme
  o texto, incluindo o caso sem segurança quando a especificação previr esse
  caso, para a tela mostrar o fluxo inteiro. O aviso na tela diz que o
  resultado é simulado e não tem relação com o conteúdo.
- Quando a decisão da IA não for escolher entre opções fechadas, a simulação
  varia a parte que a especificação fechou e mostra o restante como texto de
  exemplo, no formato final, com o mesmo aviso na tela.
- Se houver uma área que mostra esse resultado na tela, ela tem o mesmo formato
  que terá com a IA real.
- Toda caixa de texto tem limite de caracteres, com o número escrito no bloco
  de componentes.
- Quando a especificação trouxer uma lista fechada de opções, escreva os nomes
  exatos dela no bloco de componentes. Não troque, não traduza e não acrescente
  opção.
- O aplicativo roda com servidor, não como site estático. Nesta versão o
  servidor só serve a interface e responde a uma rota de saúde. Nenhuma lógica
  do produto fica nele.
- Escreva em português, em frases curtas e diretas.
- Siga exatamente o formato de cada bloco. Não use tabela, negrito nem emoji.

1. CONTEXTO
Um parágrafo de até 4 linhas: o que é o produto, quem usa e o que a pessoa
consegue fazer.

2. PÁGINAS
Uma linha por página, neste formato:
- Nome da página (rota): o que a pessoa faz aqui.

3. JORNADA PRINCIPAL
Passos numerados. Um passo por linha, neste formato:
N. [Página] A pessoa faz X. A tela mostra Y.

4. COMPONENTES POR PÁGINA
Um bloco por página, neste formato:
Nome da página:
- componente: descrição curta, com limites quando houver.

5. ESTADOS DE CADA PÁGINA
Uma linha por estado, neste formato:
Nome da página, vazio: o que aparece.
Nome da página, em espera: o que aparece.
Nome da página, sucesso: o que aparece.
Nome da página, erro: o que aparece e o que é preservado.

6. DADOS NESTA VERSÃO
Duas ou três linhas: o que fica guardado enquanto a página estiver aberta, e o
que acontece ao recarregar. Diga também que o servidor não guarda nada nesta
versão. Termine com: Não criar banco de dados.

7. FORA DESTA VERSÃO
Uma lista separada por vírgula, numa linha só.

8. CRITÉRIO DE ACEITE
No máximo três gerais e dois por página. Uma linha por item, neste formato:
Geral: frase que se confere com sim ou não.
Nome da página: frase que se confere com sim ou não.
O primeiro geral é o critério de pronto da especificação, copiado palavra por
palavra.

9. O QUE VOCÊ DECIDIU SEM ESTAR NA MINHA ESPECIFICAÇÃO
Liste aqui tudo que você escolheu por conta própria porque a especificação não
dizia. Não repita o que já estava escrito nela.
Uma linha por decisão, neste formato:
- Bloco N: o que decidi, e por que escolhi assim.
Se não precisou decidir nada por conta própria, escreva: nada.
Este bloco não vai para a ferramenta de construção. Ele existe para eu conferir
o que aceito e o que quero mudar. Deixe ele no fim da resposta, separado dos
demais, para eu poder apagar de uma vez.

[cole aqui a sua especificação de sete campos]
```
