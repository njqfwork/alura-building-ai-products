# Especificação · Vértice
> Exemplo hipotético. O produto não existe e os dados são inventados.

Minha ideia em uma frase: a pessoa de produto de um SaaS de gestão de tarefas recebe feedback por três canais e não sabe quais assuntos mais se repetem.

## 1. Problema e público
Nome do produto: Leitor de Feedback do Vértice.

A pessoa de produto do Vértice recebe feedback de três lugares: a pesquisa de NPS trimestral, os chamados abertos no suporte e as avaliações na loja de aplicativos. São algumas centenas de comentários por ciclo. Ela lê o que consegue e leva para o comitê a impressão do que viu, não o que os dados dizem. Público: a pessoa de produto, e o líder de suporte que participa da mesma reunião.

## 2. Proposta de valor
Em vez de chegar ao comitê com impressão, chegar com contagem. Em um minuto ela vê qual assunto mais se repete no ciclo e quantos comentários sustentam isso.

## 3. Escopo do MVP
Dentro desta versão:
- Registrar um feedback colado de qualquer canal, sem identificar o cliente.
- Classificar em cinco categorias fechadas: Performance, Usabilidade, Integrações, Cobrança e Suporte.
- Listar os feedbacks por categoria, com a contagem de cada uma no topo.

Fora desta versão:
- Puxar os comentários direto da ferramenta de NPS ou da loja de aplicativos.
- Responder ao cliente, por qualquer canal.
- Separar por produto, por plano ou por segmento de cliente.
- Relatório para exportar ou enviar por email.

## 4. Fluxo principal
1. A pessoa abre a tela de registro com a caixa de texto vazia e o botão Analisar desligado.
2. Cola o texto de um feedback e clica em Analisar.
3. A tela mostra que está analisando, e o botão fica desligado.
4. A tela mostra a categoria escolhida e o motivo em uma frase.
5. A pessoa clica em Ver na lista e encontra o item no topo, com a contagem por categoria atualizada.

## 5. Componentes
Telas: registro e lista.
Dados: o texto do feedback, a categoria, o motivo, a data e o status.
IA: o agente classificador, que decide a categoria e escreve o motivo.

## 6. Papel da IA
A IA decide: a categoria de cada feedback, entre as cinco da lista, e escreve o motivo em uma frase.
A IA não decide: nada fora dessas cinco categorias, não cria categoria nova, não responde ao cliente e não apaga nem edita feedback registrado.
Quando não tem segurança: marca o feedback como revisão, escreve por que ficou em dúvida, e o item aparece na lista com esse status.

## 7. Critério de pronto
Um feedback colado aparece na lista com categoria e motivo, e a contagem daquela categoria aumenta em um.
