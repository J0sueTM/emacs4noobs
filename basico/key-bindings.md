# [Básico](README.md) &#129170; Key Bindings

Como vimos na seção [como o Emacs funciona](como-o-emacs-funciona.md), o editor é tecnicamente um encapsulador de Macros. Iremos aprender um pouco mais pra frente como esses modos são criados e chamados em runtime; porém, existe um tipo de Macro que você usa todos os dias fora do editor, e talvez nunca tenha parado pra pensar acerca deles.

Estou me referindo às KeyBindings (combinações de teclas). Não sabe do que estou falando?:

- Salvar um arquivo (Ctrl + S)
- Nova aba no navegador (Ctrl + N)
- Selecionar todo o texto (Ctrl + A)

Esses comandos são chamados de KeyBindings. São simplesmente declarações que denotam, dependendo da aplicação que, quando o usuário clicar essa tecla, e essa tecla, e aquela, faça tal coisa, como os exemplos dados a cima. Lembrando que esses que listei são exemplos, não necessariamente funcionam da mesma maneira no Emacs.

O Emacs usa esta função em praticamente todo o contexto de edição de texto. A partir deste momento, quero que se forçe a parar de usar as setas do teclado. Com o Emacs aberto, você não vai precisar mover suas mãos, **NUNCA MAIS** (kkk talvez precise, mas você me entendeu).

## Nomenclatura

Digitar Ctrl, Alt, etc, pelo resto desse aulão seria desnecessário. Portanto, estarei utilizando a seguinte convenção de diminutivos:

- C: Control
- M: Meta (Alt)
- Space: Espaço

Abra seu Emacs, e vamos que vamos:

## Movimento

O Emacs utiliza de KeyBindings semânticas, ou seja, que procuram sinalizar significado. Por exemplo, `f` para forward, `b` para backwards, etc.

### Caractere

- Ir um caractere para frente: `C-f`
- Ir um caractere para trás: `C-b`

### Linha

- Ir uma linha para cima: `C-p`
- Ir uma linha para baixo: `C-n`
- Ir para o começo da linha: `C-a`
- Ir para o fim da linha: `C-e`
- Ir para linha de n°: `M-g-g`

### Palavra

- Ir uma palavra para frente: `M-f`
- Ir uma palavra para trás: `M-b`

### Avançado

- Ir para o começo do arquivo: `M-<`
- Ir para o fim do arquivo: `M->`

## Edição

- Deletar caractere embaixo do cursor ou texto selecionado: `C-d`
- Deletar palavra em frente ao cursor: `M-d`
- Deletar toda a linha para frente do cursor: `C-k`
- Colar: `C-y`
- Desfazer: `C-/`

### Seleção

Seleção seria o mesmo que clicar Shift e selecionar o texto com o mouse, em algum outro editor de texto para realizar operações como, por exemplo, copiar, cortar, etc. Vale lembrar que, mesmo no modo de seleção, as Key Bindings de movimento continuam as mesmas.

- Selecionar todo o arquivo: `C-x-h`
- Entrar ou sair do modo de seleção: `C-Space`
- Copiar texto selecionado: `M-w`

### Pesquisa

Existe duas maneiras principais de pesquisar no Emacs. Pesquisar para frente, e para trás do cursor. Caso você queira pesquisar por todo o documento, já que talvez não saiba se o que procura está para frente ou para trás do cursor, basta usar a KeyBinding de ir para o começo do arquivo, e então pesquisar para frente.

- Pesquisar para frente: `C-s`
- Pesquisar para trás: `C-r`

## Conclusão

O Emacs possui diversas outras KeyBindings, as quais você irá aprender mais pra frente. Entretanto, até o momento, acredito que essas que listei serão o suficiente para que você começe a hackear o editor. Caso esteja curioso, basta digitar `C-h-h`, e o Emacs irá te mostrar todas as KeyBindings existentes.

<div align="center" markdown=1>
    <a href="como-o-emacs-funciona.md">&#129168; Como o Emacs funciona</a>
    ·
    <a href="../README.md">Home</a>
    ·
    <a href="buffers.md">Buffers &#129170;</a>
</div>
