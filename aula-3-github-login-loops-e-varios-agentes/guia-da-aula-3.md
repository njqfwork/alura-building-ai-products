# Aula 3 · GitHub, login, loops e vários agentes

**Você sai com:** o código com uma cópia no GitHub, em repositório privado, e o app com login, em que cada pessoa vê só os próprios dados, inclusive o histórico que o agente lê. E com dois conceitos para decidir o próximo passo do seu produto: o loop e os projetos com vários agentes.

## O caminho

### 1. O código no GitHub

Até aqui tudo mora dentro do Replit: o código, o banco e a chave. O GitHub guarda uma cópia do código fora. É a parte que mais costuma travar, então ela tem um guia só dela, feito para seguir pela tela, sem terminal:

**[Git pelo Replit, passo a passo](git-passo-a-passo.md)**

O resumo:

1. Crie uma conta gratuita em [github.com](https://github.com).
2. Cole o [prompt 01](prompts/01-github.md) e corrija o que ele apontar.
3. No Replit, abra o **Git**, conecte o GitHub, crie o repositório **privado** e clique em **Push**.
4. No GitHub, confira: aparece **Private**, e a sua chave não está lá.

Daqui para frente: mudou e funcionou, **Push**. O Agent já faz os commits sozinho.

### 2. Login, e cada pessoa vendo só o que é dela

Sem login, o app é de ninguém: quem tem o link vê tudo, e o agente lê o histórico de todo mundo. O login da própria ferramenta (no Replit, o Replit Auth) já traz a tela de entrar, o cadastro, a recuperação de senha e guarda a senha fora do seu banco. Por isso o pedido não fala dessas telas. Se um dia o produto precisar de marca própria, ou de sair do Replit, existe serviço de login à parte, como o Clerk.

1. Cole o [prompt 02](prompts/02-login.md) na ferramenta.
2. Com o login pronto, abra o painel **Auth** do projeto, em **Configure**: deixe o email ligado e coloque o nome e o ícone do app.
3. Confira, nesta ordem:
   1. Deslogado, aparece só a tela com o botão Entrar.
   2. Entrar com email funciona.
   3. Na tela de login, o link de esqueci a senha manda o email.
   4. O botão de sair funciona.
   5. Numa janela anônima, uma segunda conta vê a lista vazia.
4. Confira o topo da aba Git. Se mostrar outra branch que não a `main`, o login ficou fora dela: junte seguindo [quando o trabalho ficou em outra branch](git-passo-a-passo.md#quando-o-trabalho-ficou-em-outra-branch).
5. Envie com **Push** e publique de novo.

### 3. O que vimos sem construir

Nestes dois blocos ninguém construiu nada. Ficam aqui em resumo, para consulta.

**O Ralph loop** repete o mesmo pedido até o trabalho ficar pronto. A cada volta o agente trabalha e grava o progresso em arquivos e no Git, depois confere se o critério combinado foi atingido: se sim, para; se não, começa outra volta do zero, lendo o que ficou gravado. Sempre com um limite de voltas, porque cada volta é uma chamada paga. Ele só funciona quando o pronto se confere sem você, como testes que passam. Quando o pronto depende de opinião, o loop fica girando sem saber parar.

**Vários agentes** não são agentes conversando entre si: são etapas, cada uma com a própria ficha, e cada agente a mais é uma chamada a mais em toda decisão. Num projeto assim, cada agente é um arquivo com a ficha dele, e um comando define o fluxo: quem roda, em que ordem e o que passa adiante. Vale a pena quando aparece um destes sinais:

| Sinal | O que significa |
|---|---|
| Dois trabalhos numa ficha | Os critérios brigam: acertar cada caso e resumir o conjunto, por exemplo |
| Contexto grande demais | O que o agente precisa ler já não cabe bem numa chamada só |
| Erro caro | Errar custa tanto que vale pagar uma segunda opinião independente |
| Etapas diferentes | Cada passo precisa de ferramentas ou informações diferentes |

Se nenhum aparece no seu produto, um agente bem escrito resolve. Escreva uma linha: o seu produto precisa disso hoje? Se não, qual sinal diria que chegou a hora? Essa linha volta no fechamento da Aula 4, na ficha que cada um leva pronta.

## Prompts

| Arquivo | Quando | Onde colar |
|---|---|---|
| [01-github.md](prompts/01-github.md) | Antes do primeiro envio ao GitHub | Ferramenta de construção |
| [02-login.md](prompts/02-login.md) | Com o código já no GitHub | Ferramenta de construção |

## Outros arquivos

| Arquivo | O que é |
|---|---|
| [git-passo-a-passo.md](git-passo-a-passo.md) | O Git inteiro pela tela do Replit, com o que fazer quando o trabalho fica em outra branch |

## Tarefa até a Aula 4

1. Use o seu produto umas vinte vezes ao longo da semana.
2. Anote o que ele errar. Na Aula 4, cada erro vira um caso de teste.
3. Depois de cada mudança que funcionar, clique em **Push**.
4. Opcional: peça a um colega para testar com a conta dele.
