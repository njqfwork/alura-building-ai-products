# Construir a primeira versão

Cole num Replit App novo, no chat do Agent, com a resposta da tradução (sem o último bloco) no lugar do colchete. As sete regras criam o arquivo `replit.md`, que a ferramenta segue daqui para frente. A última linha faz o Agent mostrar o plano antes de construir: leia com calma, porque corrigir o plano custa quase nada. Se a sua ferramenta não for o Replit, troque `replit.md` pelo nome do arquivo de regras dela.

```
[cole aqui a resposta da tradução, sem o último bloco]

Antes de começar, crie o arquivo replit.md com estas regras, e siga elas
em todas as tarefas seguintes:
1. Não criar banco de dados nem login nesta versão. O servidor existe, mas não
   guarda nada: os dados ficam na memória do navegador.
2. Nenhuma chamada a serviço de IA nesta versão. A decisão é simulada dentro
   do aplicativo, com aviso na tela.
3. Não trocar a stack depois da primeira versão.
4. Não instalar biblioteca nova sem me perguntar antes.
5. Ao fim de cada mudança, rodar, conferir e me dizer o que mudou.
6. Você pode acrescentar neste arquivo o que o projeto passou a ser: stack,
   arquivos principais, como rodar. Não apague nem reescreva o que já está
   aqui, e não crie regra nova sem me perguntar antes.
7. Faça tudo em um único artefato web, sem API Server separado, com o preview
   funcionando na raiz. Publicar sempre com servidor, nunca como site estático,
   e manter uma rota de saúde respondendo.

Se a criação do projeto substituir este arquivo, recrie ele com estas sete
regras antes de continuar.

Depois disso, liste as tarefas que você vai executar e espere minha
confirmação. Não construa nada que esteja em FORA DESTA VERSÃO.
```
