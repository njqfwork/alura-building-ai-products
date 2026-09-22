# Git pelo Replit, passo a passo

Tudo pela tela, sem terminal. Os nomes dos botões estão como aparecem no Replit em português e no GitHub em inglês. Se algum mudar, siga o caminho: ele continua o mesmo.

## As palavras

| Palavra | O que é |
|---|---|
| Git | O sistema que guarda as versões do código |
| GitHub | O site onde fica a cópia do código, fora do Replit |
| Repositório | A pasta do projeto no GitHub |
| Commit | Uma foto do projeto, com uma frase do que mudou |
| Push | Mandar os commits do Replit para o GitHub |
| Pull | Trazer para o Replit o que mudou no GitHub |
| Branch | Uma linha paralela do projeto. A principal se chama `main` |
| origin | O nome que o Git dá ao repositório no GitHub |
| Pull Request e Merge | O pedido para juntar uma branch na `main`, e o ato de juntar |

O ponto salvo do Replit também volta versões, mas mora dentro do Replit. O commit, depois do push, fica fora.

## Antes: a conta no GitHub

Crie uma conta gratuita em [github.com](https://github.com) e guarde o login e a senha.

## Primeira vez: ligar o projeto ao GitHub

1. **Confira as chaves.** Cole o [prompt 01](prompts/01-github.md) na ferramenta e corrija o que ele apontar.
2. **Abra o Git.** Na área de ferramentas do Replit, clique no **+** e escolha **Git**.
3. **Conecte o GitHub.** Entre com a sua conta e autorize o Replit. Ele só mexe nos repositórios que você escolher.
4. **Crie o repositório.** Nome curto, sem espaço, como o nome do produto. Marque **privado** antes de criar.
5. **Envie.** Se houver alterações, escreva a frase do commit e faça o commit. Depois, clique em **Push**.
6. **Confira no GitHub.** Clique no nome do repositório, no topo da aba Git. Tem que aparecer **Private** ao lado do nome, as fichas e o arquivo de regras têm que estar lá, e a sua chave não pode estar.

## Como ler a aba Git

| O que aparece | O que significa |
|---|---|
| Nome no topo, ao lado do ícone de branch | A branch em que você está. O normal é `main` |
| Remote Updates · `origin/main` | O repositório no GitHub |
| **Pull** | Traz o que mudou no GitHub |
| **Push** | Envia os seus commits para o GitHub. Fica apagado quando não há nada para enviar |
| **Sincronizar alterações** | Faz Pull e Push de uma vez |
| "Não há alterações para fazer commit." | Tudo o que mudou já virou commit |
| Lista de commits do Replit Agent | Normal. O Agent faz commit sozinho a cada etapa |
| **Fazer push do branch como 'origin/...'** | Você está numa branch que não é a `main`, e ela ainda não existe no GitHub. Veja [a seção abaixo](#quando-o-trabalho-ficou-em-outra-branch) |

## O hábito: mudou e funcionou, envie

Como o Agent já faz os commits, o seu trabalho quase sempre é só o envio.

1. Confira se o topo da aba Git mostra `main`.
2. Clique em **Push**, ou em **Sincronizar alterações**.
3. No GitHub, veja se o último commit aparece com o horário de agora.

## Quando o trabalho ficou em outra branch

Às vezes o Agent constrói uma tarefa maior, como o login, numa branch separada. O trabalho fica pronto, mas fora da `main`.

**Como perceber:**
- O topo da aba Git mostra outro nome, como `login` ou `feature/login`.
- Aparece o botão **Fazer push do branch como 'origin/...'**.
- No GitHub aparece a faixa "This branch is 1 commit behind feature/login".

**Como juntar, pela tela:**

1. **No Replit,** com a branch do trabalho selecionada, clique em **Fazer push do branch como 'origin/...'**.
2. **No GitHub,** abra o repositório. Clique em **Compare & pull request**, na faixa amarela, ou em **Contribute** e depois em **Open pull request**.
3. **Confira a direção:** *base* é `main` e *compare* é a sua branch. Clique em **Create pull request**.
4. **Espere o GitHub checar.** O botão fica cinza por alguns segundos, com a mensagem "Checking for the ability to merge automatically".
5. **Junte:** clique em **Merge pull request** e depois em **Confirm merge**. Ninguém precisa aprovar: o repositório é seu. Se quiser, clique em **Delete branch**.
6. **No Replit,** clique no nome da branch, no topo da aba Git, e escolha `main`. Depois clique em **Pull**.
7. **Publique de novo,** para o link ter o que você juntou.

**Dois cuidados:**
- O Replit roda o código da branch selecionada. Na `main` antes do merge, o app aparece sem o que foi feito na outra branch.
- O banco é um só para todas as branches. Se o trabalho mudou tabelas, a `main` pode dar erro até você juntar.

## Problemas comuns

| O que acontece | O que fazer |
|---|---|
| **Push** apagado | Não há nada novo para enviar. Está tudo no GitHub |
| O envio é recusado, dizendo que está desatualizado | Clique em **Pull** primeiro e depois em **Push**, ou use **Sincronizar alterações** |
| O Pull Request mostra conflito | Não resolva sozinho. Feche o Pull Request sem juntar e peça ajuda |
| A chave apareceu no GitHub | Apague a chave no Google AI Studio e crie outra. A antiga já vazou, mesmo que você apague o arquivo. Guarde a nova nos Secrets |
| O repositório ficou público | No GitHub, em Settings, no fim da página, mude para privado |
