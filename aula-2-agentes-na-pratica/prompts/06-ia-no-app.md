# Ligar a ficha ao app

Cole na ferramenta de construção, depois de criar a chave ([passo a passo](../modelos/chave-do-modelo.md)). Troque os colchetes: `[modelo]` pelo Gemini, com a chave do Google AI Studio; `[nome do arquivo]` por algo como ficha-do-agente.md; `[nome do botão]` pelo texto exato do botão na sua tela; `[o que a pessoa escreveu]` pelo que chega do usuário, como o texto do feedback; `[NOME_DO_SECRET]` por GEMINI_API_KEY. Depois de construir, cole a sua ficha dentro do arquivo criado. Para conferir, edite uma linha da ficha e mande o mesmo caso: a decisão tem que mudar sem você pedir nada à ferramenta. E procure a chave no código: se achar, está errado. Se a ferramenta sugerir uma integração de IA própria, recuse: na Aula 4 você mede o custo por chamada, e isso só funciona com a sua chave.

```
Quero substituir a resposta simulada por uma decisão de verdade, tomada pelo
[modelo].

Vou colocar no projeto um arquivo de texto com as instruções do agente. O app
deve ler esse arquivo a cada decisão, e não copiar o conteúdo para dentro do
código: quando eu editar o arquivo, o comportamento tem que mudar sem precisar
pedir nada a você.

Faça o seguinte:
1. Crie o arquivo [nome do arquivo] na raiz do projeto, com o conteúdo que eu
   vou colar depois.
2. Quando a pessoa clicar em [nome do botão], o app lê esse arquivo, manda ele
   junto com [o que a pessoa escreveu] para o modelo, e mostra na tela a
   decisão e o motivo que voltarem.
3. Guarde o resultado na tabela que já existe, com o status.
4. A chave fica no secret [NOME_DO_SECRET] e só pode ser usada no servidor. O
   navegador nunca pode ler essa chave. Peça o valor do secret quando precisar.

Antes de construir, liste o que você vai fazer e espere minha confirmação.
Não use nenhuma integração de IA sem me perguntar antes.
```
