# [Básico](README.md) &#129170; Buffers

Segura o coração que lá vem mais macros. Como eu disse na parte anterior, o Emacs possui uma macro pra praticamente qualquer coisa; e se não tem, pra criar outro é 2 palito (vamos ver isso na seção avançado). Vamos aprender, agora, sobre um dos blocos fundamentais do Emacs, as Janelas e os Buffers.

Os buffers são basicamente camadas de visualização do conteúdo de um arquivo. Não entendeu? kkk não se preocupe, vou lhe explicar um pouco melhor. Quando você abre um arquivo no Emacs (KeyBinding abaixo), o artefato de visualização desse arquivo é aberto em uma janela, mas a janela em si não é a mesma coisa que o buffer: O buffer está contido na janela, mas a janela é existente por si só.

Diferencie da seguinte maneira: Janela é o retângulo onde o texto é desenhado. Sempre existe pelo menos uma janela, mas nuca menos que isso. O buffer é um temporário acesso ao conteúdo de um arquivo, que será desenhado em uma ou mais janelas que forem selecionadas.

Abra o seu Emacs. Assim que aberto, caso você não tenha modificado nada, teremos uma Janela, e 3 buffers abertos. JOSUÉ? 3 BUFFERS, ONDE? NÃO ESTOU VENDO. Calma meu caro, como eu disse anteriormente, o buffer não necessariamente precisa estar sendo desenhado em uma janela.

Para ver quais buffers estão abertos no momento, existem duas maneiras: `C-x-b` irá abrir uma janela à direita, listando os buffers abertos. No seu caso, provavelmente estarão listados:

- **\*About GNU Emacs\***: A página inicial
- **\*scratch\***: Um rascunho
- **\*Messages\***: Mensagens que geralmente aparecem no Buffer de comando

A partir daqui, basta navegar entre as opções listadas e clicar `<Return>` que o buffer selecionado será aberto na janela que estava desenhando o buffer de listagem dos buffers (confuso, eu sei, teste no seu Emacs e ficará um pouco mais concreto).

A outra maneira, não muito diferente, lista os buffers igualmente, mas abre a listagem no buffer de comando, que é aquele lá embaixo do Emacs, que as vezes aparece algumas mensagens (aliás, essas mensagens vêm lá do buffer de \*Messages\*, como disse anteriormente). Realize isso pressionando `C-x b`, então digite o buffer que queira abrir. Caso não lembre, basta digitar `<Tab>`, e os buffers serão listados consequentemente.

## Keybindings

### Janela

- Fechar a janela que estou no momento: `C-x 0`
- Fechar todas as janelas menos a que estou: `C-x 1`
- Abrir uma janela para baixo: `C-x 2`
- Abrir uma janela para o lado: `C-x 3`
- Pular para a próxima janela: `C-x o`

### Buffer

- Carregar arquivo em um buffer: `C-x f`
- Reabrir buffer em outra janela: `C-x-b`
- Reabrir buffer na janela que estou: `C-x b`
- Deletar buffer: `C-x k`

## Conclusão

Não se preocupe se os conceitos apresentados aqui não entraram na cabeça de primeira mão, com o tempo você se acostuma, nem percebendo que um dia teve que entender esse conteúdo.

<div align="center" markdown=1>
    <a href="key-bindings.md">&#129168; Key Bindings</a>
    ·
    <a href="../README.md">Home</a>
    ·
    <a href="command-buffer.md">Command Buffer &#129170;</a>
</div>
