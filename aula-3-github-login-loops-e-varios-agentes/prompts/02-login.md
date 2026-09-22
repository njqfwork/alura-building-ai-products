# Login, e cada pessoa vê só o que é dela

Cole na ferramenta de construção. O pedido usa o login que a própria ferramenta oferece, que já traz a tela de entrar, o cadastro e a recuperação de senha. O item 2 evita que os registros criados antes do login sumam da lista, junto com o histórico da Aula 2. O item 3 faz o agente ler só o histórico de quem está usando. O item 5 define o que vê quem ainda não entrou. Depois, confira os cinco passos do [guia da aula](../guia-da-aula-3.md#2-login-e-cada-pessoa-vendo-só-o-que-é-dela).

```
Quero adicionar login ao produto, usando o login que a própria ferramenta
oferece. Permita entrar com [email].

1. Cada registro passa a pertencer à pessoa que o criou.
2. Os registros criados antes do login ainda não têm dono. Passe todos
   para a primeira conta que entrar, que será a minha.
3. Tudo que o app lê passa a ser só da pessoa logada, inclusive o
   histórico que o agente lê antes de decidir.
4. Um botão de sair, visível em todas as telas.
5. Quem não está logado vê só uma tela com o nome do produto e o botão
   Entrar.

Antes de construir, liste o que você vai fazer e espere minha confirmação.
```
