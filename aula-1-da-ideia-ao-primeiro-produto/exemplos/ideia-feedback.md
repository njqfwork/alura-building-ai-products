# Especificação · Análise de feedback de clientes
> Exemplo preenchido, para quem chegou sem ideia. Troque o produto e as categorias pelo seu contexto.

Minha ideia em uma frase: quem cuida de um produto recebe comentários por vários canais e não sabe quais assuntos mais se repetem.

## 1. Problema e público
Nome do produto: Leitor de Feedback.

A pessoa responsável pelo produto recebe comentários de três lugares: pesquisa de satisfação, chamados de suporte e avaliações públicas. São dezenas por semana. Ela lê o que consegue e leva para a reunião a impressão do que viu, não o que os dados dizem. Público: quem cuida do produto, e quem lidera o suporte.

## 2. Proposta de valor
Em vez de chegar à reunião com impressão, chegar com contagem. Em um minuto ela vê qual assunto mais se repete e quantos comentários sustentam isso.

## 3. Escopo do MVP

Dentro desta versão:
- Registrar um comentário colado de qualquer canal, sem identificar o cliente.
- Classificar em cinco categorias fechadas: Performance, Usabilidade, Integrações, Cobrança e Suporte.
- Listar os comentários por categoria, com a contagem de cada uma no topo.

Fora desta versão:
- Puxar os comentários direto das ferramentas de origem.
- Responder ao cliente, por qualquer canal.
- Separar por produto, plano ou segmento.
- Relatório para exportar ou enviar por email.

## 4. Fluxo principal
1. A pessoa abre a tela de registro. A caixa está vazia e o botão Analisar está desligado.
2. Cola o texto de um comentário e clica em Analisar. A tela mostra que está analisando.
3. A tela mostra a categoria escolhida e o motivo em uma frase.
4. A pessoa clica em Ver na lista. A lista abre com o item no topo.
5. A contagem daquela categoria aumenta em um.

## 5. Componentes
Telas: registro e lista.
Dados: o texto do comentário, a categoria, o motivo, a data e o status.
IA: o agente classificador, que decide a categoria e escreve o motivo.

## 6. Papel da IA
A IA decide: a categoria de cada comentário, entre as cinco da lista, e escreve o motivo em uma frase.
A IA não decide: nada fora dessas cinco categorias, não cria categoria nova, não responde ao cliente e não apaga nem edita comentário registrado.
Quando não tem segurança: marca como revisão, escreve por que ficou em dúvida, e o item aparece na lista com esse status.

## 7. Critério de pronto
Um comentário colado aparece na lista com categoria e motivo, e a contagem daquela categoria aumenta em um.
