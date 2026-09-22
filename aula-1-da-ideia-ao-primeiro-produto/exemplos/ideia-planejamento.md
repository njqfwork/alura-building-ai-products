# Especificação · Assistente de planejamento para pequenos negócios
> Exemplo preenchido, para quem chegou sem ideia. Troque o negócio e as áreas pelo seu contexto.

Minha ideia em uma frase: quem toca um negócio pequeno sabe o que incomoda, mas não consegue transformar isso num plano de ação.

## 1. Problema e público
Nome do produto: Plano da Semana.

Quem toca um negócio pequeno, sozinho ou com poucas pessoas, sabe o que está ruim: as vendas caíram, o estoque some, o cliente reclama da entrega. Mas transformar isso em ações concretas para a semana leva tempo que ela não tem, e acaba não acontecendo. Público: quem é dono do negócio e decide sozinho.

## 2. Proposta de valor
Escrever o incômodo em duas frases e receber três ações para a semana, em vez de um plano de trinta páginas que ninguém executa.

## 3. Escopo do MVP

Dentro desta versão:
- Descrever o negócio em poucas linhas e o problema atual.
- Receber três ações para a semana, cada uma com a área e o esforço.
- Listar os planos gerados, do mais recente para o mais antigo.

Fora desta versão:
- Marcar ação como concluída ou acompanhar execução.
- Lembrete por email ou mensagem.
- Vários negócios na mesma conta.
- Números financeiros e projeções.

## 4. Fluxo principal
1. A pessoa abre a tela de plano. Os dois campos estão vazios e o botão Gerar está desligado.
2. Escreve o que o negócio faz e qual o problema da semana. Clica em Gerar.
3. A tela mostra que está gerando.
4. A tela mostra três ações, cada uma com a área e o esforço.
5. A pessoa clica em Ver planos e encontra o plano no topo da lista.

## 5. Componentes
Telas: plano e histórico.
Dados: a descrição do negócio, o problema, as três ações, a data.
IA: o agente de planejamento, que escreve as ações.

## 6. Papel da IA
A IA decide: quais três ações propor, e a área de cada uma entre Vendas, Operação, Atendimento, Preço e Divulgação.
A IA não decide: nada fora dessas cinco áreas, não propõe mais nem menos que três ações, e não fala de valores em dinheiro.
Quando não tem segurança: escreve que o problema está vago e pede uma informação específica, em vez de propor ação.

## 7. Critério de pronto
Um problema escrito em duas frases gera três ações, cada uma com área e esforço, e o plano aparece no histórico.
