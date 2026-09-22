# Criar a chave do modelo

Passo a passo para usar o Gemini no plano gratuito. Leva uns três minutos, e não pede cartão.

**Antes:** você precisa de uma conta Google. Se a sua for de empresa, pode ser que o administrador tenha bloqueado essa criação. Nesse caso, use uma conta pessoal.

## Passo a passo

1. Abra `aistudio.google.com/apikey` no Chrome, logado na sua conta Google.
2. Se for a primeira vez, aceite os termos de uso. Quem nunca usou ganha um projeto criado automaticamente. Quem já tem conta no Google Cloud precisa importar um projeto antes, em Dashboard, Projects, Import projects.
3. Clique em **Create API key**.
4. Escolha o projeto que aparecer na lista e confirme.
5. Copie a chave. Ela aparece uma vez só, inteira. Se fechar sem copiar, crie outra: não custa nada.
6. Guarde onde a sua ferramenta pede segredos. No Replit, em Secrets. Ou espere: quando você mandar integrar o modelo, ela abre o campo sozinha. Nome sugerido: `GEMINI_API_KEY`.

## O que é gratuito

O plano gratuito dá tokens de entrada e saída sem custo, com limite de chamadas por minuto e por dia. Para o curso, sobra.

Uma coisa a saber: no plano gratuito, o conteúdo que você manda pode ser usado pelo Google para melhorar os modelos deles. **Não mande dado real de cliente.** No curso isso não é problema, porque a base é sintética.

## Se der erro

| O que acontece | O que fazer |
|---|---|
| Create API key não aparece, ou diz sem permissão | A conta é de uma organização que bloqueia. Use conta pessoal, ou peça ao administrador |
| Erro 429 no app | Você passou do limite por minuto ou por dia. Espere e tente de novo |
| A chave para de funcionar | Chave sem restrição e sem uso por muito tempo é bloqueada. Crie outra: as novas já nascem certas |

## Se você quiser usar outro modelo

O curso não depende do Gemini. Qualquer modelo com chave própria serve. O que muda é onde você cria a chave. O resto é igual: copiar, guardar no lugar de segredos, e nunca deixar no código.
