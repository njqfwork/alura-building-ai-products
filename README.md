# Building AI Products · Material da turma

Prompts, modelos e exemplos das aulas do curso Building AI Products, da Alura Skills & Go. Com este repositório você consegue refazer o curso inteiro, do começo ao fim.

## Como usar

- Siga o [passo a passo abaixo](#o-curso-passo-a-passo). Para os detalhes de uma aula, abra o guia dela, dentro da pasta da aula: `guia-da-aula-1.md`, `guia-da-aula-2.md` e `guia-da-aula-3.md`.
- Prefere ler tudo numa página só, com botão de copiar em cada prompt? Baixe o repositório e abra o arquivo `guia.html` no navegador.
- Cada prompt está num arquivo próprio: uma explicação curta em cima e o texto para colar embaixo.
- O que está entre colchetes você troca pelo seu caso. Exemplo: `[seu produto]`.
- **Chat de IA** é o assistente que você já usa: ChatGPT, Claude, Gemini ou outro.
- **Ferramenta de construção** é onde o app é construído. Na aula usamos o Replit. Os prompts servem para Lovable e similares: onde aparecer `replit.md`, use o arquivo de regras da sua ferramenta.

## Três regras que valem para o curso inteiro

1. **Chave, senha e dados do banco não vão para o código nem para o GitHub.** A chave fica no lugar de segredos da ferramenta (no Replit, Secrets).
2. **Nenhum dado real de cliente.** Use base sintética. No plano gratuito do Gemini, o que você manda pode ser usado para treinar o modelo.
3. **Uma correção por mensagem.** Se a correção piorou, volte ao ponto salvo em vez de corrigir de novo.

## O curso, passo a passo

Siga na ordem: cada aula parte do que a anterior deixou pronto. Cada passo aponta para o arquivo com os detalhes.

### Aula 1 · Da ideia ao produto no ar

O que você faz: escreve a especificação do produto e constrói a primeira versão na ferramenta, com a decisão da IA ainda simulada.

1. **Escolha a ideia.** Uma base de dados que você reúne sozinho e uma IA que decide algo sobre ela. Sem ideia, use um dos [exemplos prontos](aula-1-da-ideia-ao-primeiro-produto/exemplos/).
2. **Escreva a especificação** nos sete campos do [modelo](aula-1-da-ideia-ao-primeiro-produto/modelos/especificacao-em-branco.md).
3. **Traduza a especificação** num prompt de construção, no chat de IA: [prompt 01](aula-1-da-ideia-ao-primeiro-produto/prompts/01-traducao.md). Leia o último bloco e apague ele.
4. **Construa num Replit App novo:** [prompt 02](aula-1-da-ideia-ao-primeiro-produto/prompts/02-construcao.md). Leia o plano antes de confirmar e corte o que você não pediu com o [prompt 03](aula-1-da-ideia-ao-primeiro-produto/prompts/03-cortar-o-plano.md).
5. **Corrija uma coisa por vez:** [molde de correção](aula-1-da-ideia-ao-primeiro-produto/prompts/04-correcao.md).
6. **Publique** e abra o link numa janela anônima.
7. **Prepare a Aula 2:** crie conta no Google AI Studio e gere a base sintética com o [prompt 05](aula-1-da-ideia-ao-primeiro-produto/prompts/05-base-sintetica.md).

**Pronto quando:** o link publicado abre, o fluxo vai do início ao fim, e o seu critério de pronto confere na tela.

Detalhes: [guia da Aula 1](aula-1-da-ideia-ao-primeiro-produto/guia-da-aula-1.md).

### Aula 2 · A IA e o banco de dados entram no produto

O que você faz: os dados passam a ficar num banco, você escreve e testa a ficha do agente, e a IA passa a decidir de verdade.

1. **Mude as regras do projeto:** [prompt 01](aula-2-agentes-na-pratica/prompts/01-regras.md).
2. **Crie o banco:** [prompt 03](aula-2-agentes-na-pratica/prompts/03-banco.md). Se não souber o que guardar, antes use o [prompt 02](aula-2-agentes-na-pratica/prompts/02-o-que-guardar.md). Depois, carregue a base sintética.
3. **Escreva a ficha do agente** no [modelo](aula-2-agentes-na-pratica/modelos/ficha-do-agente-em-branco.md). Exemplo: [ficha do Vértice](aula-2-agentes-na-pratica/exemplos/vertice-ficha.md).
4. **Calibre a ficha** numa conversa nova do chat de IA: [prompt 05](aula-2-agentes-na-pratica/prompts/05-calibrar-ficha.md).
5. **Crie a chave do Gemini** pelo [passo a passo](aula-2-agentes-na-pratica/modelos/chave-do-modelo.md) e **ligue a ficha ao app:** [prompt 06](aula-2-agentes-na-pratica/prompts/06-ia-no-app.md).
6. **Teste os limites:** um caso fora do assunto e um ambíguo. Se falhar, corrija a ficha, não o código.
7. **Faça o agente consultar a base:** [prompt 07](aula-2-agentes-na-pratica/prompts/07-consultar-base.md).

**Pronto quando:** a decisão vem do modelo, muda quando você edita a ficha, e a chave não aparece em lugar nenhum do código.

Detalhes: [guia da Aula 2](aula-2-agentes-na-pratica/guia-da-aula-2.md).

### Aula 3 · GitHub, login e vários agentes

O que você faz: guarda uma cópia do código no GitHub, coloca login no produto com cada pessoa vendo só os próprios dados, e conhece o loop e os projetos com vários agentes.

1. **Crie uma conta gratuita** em github.com.
2. **Mande o código para o GitHub, pela tela:** siga o [Git passo a passo](aula-3-github-login-loops-e-varios-agentes/git-passo-a-passo.md). Antes do primeiro envio, use o [prompt 01](aula-3-github-login-loops-e-varios-agentes/prompts/01-github.md).
3. **Coloque o login:** [prompt 02](aula-3-github-login-loops-e-varios-agentes/prompts/02-login.md). Depois, faça a [conferência em cinco passos](aula-3-github-login-loops-e-varios-agentes/guia-da-aula-3.md#2-login-e-cada-pessoa-vendo-só-o-que-é-dela).
4. **Confira se o login está na `main`.** Se a aba Git mostrar outra branch, junte pela tela: [quando o trabalho ficou em outra branch](aula-3-github-login-loops-e-varios-agentes/git-passo-a-passo.md#quando-o-trabalho-ficou-em-outra-branch).
5. **Envie para o GitHub e publique de novo.**
6. **Leia o resumo do que vimos sem construir:** o Ralph loop e os vários agentes, no [guia da Aula 3](aula-3-github-login-loops-e-varios-agentes/guia-da-aula-3.md#3-o-que-vimos-sem-construir).

**Pronto quando:** o repositório está privado e sem chave, uma segunda conta abre o app e vê a lista vazia, e a `main` do GitHub tem o login.

Detalhes: [guia da Aula 3](aula-3-github-login-loops-e-varios-agentes/guia-da-aula-3.md).

### Aula 4

Entra no repositório depois da aula.

## O que usamos no curso

| Para quê | O que usamos |
|---|---|
| Construir o app | Replit Agent |
| Guardar os dados | Banco do próprio Replit |
| Login | Login do próprio Replit (Replit Auth) |
| Modelo de IA | Gemini, com chave gratuita do Google AI Studio |
| Cópia do código fora da ferramenta | GitHub, em repositório privado |

## O exemplo das aulas

O **Vértice** é um SaaS de gestão de tarefas inventado para o curso. O produto não existe e todos os dados dele são fictícios. Ele aparece nos exemplos para mostrar cada passo com um caso concreto.
