# 2.1 · Minha primeira página

!!! abstract "Hoje você vai…"
    Criar a sua primeira página de internet, abrir no navegador e aprender o ciclo que você vai repetir para sempre: **escrever → salvar → atualizar**. ⏱️ ~1h

---

## Explicação

### O que é HTML?

Lembra que o computador é bem literal? Quando ele recebe um texto, ele não sabe o que é título, o que é parágrafo, o que é importante. Para ele, é tudo só um monte de letras.

O **HTML** serve para **etiquetar** cada pedaço do texto, dizendo o que ele é. E é literalmente isso: essas etiquetas se chamam **tags**, que em inglês quer dizer… **etiqueta**! 🏷️ Igual à etiqueta de uma roupa, que diz o tamanho e o tecido.

Uma tag fica entre os sinais `<` e `>`. Olha só:

```html
<h1>Olá, mundo!</h1>
```

- `<h1>` é a tag que **abre**: "aqui começa um título".
- `Olá, mundo!` é o **conteúdo**: o que aparece na tela.
- `</h1>` é a tag que **fecha**: "aqui termina o título". Repare na **barra** `/`.

Quase toda tag funciona assim, com abertura e fechamento, que nem um parêntese.

---

## Exemplo pronto

### 1. Criando o arquivo

1. Abra o VS Code com o seu repositório `desafios`.
2. Crie uma pasta nova chamada `pratica`. É aqui que você vai testar os exemplos das lições.
3. Dentro dela, crie um arquivo chamado `ola.html`.

!!! warning "O final do nome importa"
    O `.html` no final do nome se chama **extensão**. É ela que diz ao computador que tipo de arquivo é esse. Sem o `.html`, o navegador não sabe que é uma página.

### 2. Escrevendo o código

Escreva (ou copie) isto no arquivo e salve com ++ctrl+s++:

```html
<meta charset="utf-8">
<h1>Olá, mundo!</h1>
<p>Esta é a minha primeira página.</p>
```

!!! note "E essa primeira linha?"
    A linha `<meta charset="utf-8">` avisa ao navegador que a página tem **acentos**. Sem ela, um "Olá" pode aparecer como "OlÃ¡". 😵 Por enquanto, pense nela como uma **linha mágica** que toda página tem no começo. Na lição 2.5, você vai entender direitinho.

!!! tip "O VS Code completando sozinho"
    Às vezes, quando você digita `<h1>`, o VS Code já escreve o `</h1>` sozinho. Isso **não é IA**, é só um atalho simples do editor para você não esquecer de fechar a tag. Pode usar à vontade!

### 3. Abrindo no navegador

1. No Explorador do VS Code, clique com o botão direito em `ola.html`.
2. Escolha **Revelar no Explorador de Arquivos** (no Mac: **Revelar no Finder**).
3. Na pasta que abrir, dê **dois cliques** em `ola.html`.

O resultado deve ser este:

<iframe class="resultado" src="../exemplos/modulo2/ola.html" height="150" title="Resultado do exemplo"></iframe>

**Você acabou de criar uma página de internet!** 🥳

### 4. O ciclo: escrever → salvar → atualizar 🔄

Agora deixe o VS Code e o navegador abertos, lado a lado se der. Sempre que mudar alguma coisa:

1. **Escreva** a mudança no VS Code.
2. **Salve** com ++ctrl+s++ (no Mac, ++cmd+s++).
3. **Atualize** o navegador com ++f5++ (no Mac, ++cmd+r++).

!!! warning "O erro mais comum de todos"
    "Mudei o código e nada aconteceu!" Em 90% das vezes, é porque esqueceu de **salvar** ou de **atualizar**. Quando o arquivo não está salvo, o VS Code mostra uma **bolinha** ⚪ na aba, no lugar do X.

---

## ✏️ Mexe aí

Teste uma coisa de cada vez, sempre fazendo o ciclo escrever → salvar → atualizar:

1. Troque `Olá, mundo!` pelo seu nome.
2. Adicione outro parágrafo embaixo: `<p>Hoje eu aprendi HTML!</p>`
3. Apague o `</h1>` (só ele) e veja o que acontece com o parágrafo. Depois coloque de volta.

??? question "O que aconteceu no item 3?"
    O parágrafo ficou **grande, igual ao título**! Como o título não foi fechado, o navegador achou que todo o resto da página também fazia parte dele. Esse é um **bug** bem comum: esquecer de fechar uma tag.

---

## 🎯 Desafio 2.1

Hoje começa a sua página **"Sobre mim"**! Ela vai crescer um pouquinho a cada lição deste módulo.

1. No repositório `desafios`, crie uma pasta chamada `sobre-mim`.
2. Dentro dela, crie um arquivo chamado `index.html`.
3. Escreva a linha mágica e um título `<h1>` com o **seu nome**.
4. Abra no navegador para conferir.
5. Faça o ritual de entrega 📦 com a mensagem `"Desafio 2.1: começando o sobre mim"`.

!!! note "Por que `index.html`?"
    **index** é o nome que os sites usam para a **página principal**, tipo a capa de uma revista. Quando a sua página for para a internet, no Módulo 4, esse nome vai fazer diferença.

!!! tip "Uma pasta só para o 'Sobre mim'"
    Neste módulo, os desafios **não** ficam em pastas `desafio-2.1`, `desafio-2.2`… Todos vão para a mesma pasta `sobre-mim`, porque é a mesma página crescendo. Cada entrega fica guardada no histórico do Git, então dá para ver a evolução depois!

---

## ✅ Checklist

- [ ] Sei o que é **HTML** e o que é uma **tag**
- [ ] Sei que a maioria das tags **abre** e **fecha** (com a barra `/`)
- [ ] Sei criar um arquivo `.html` e abrir no navegador
- [ ] Sei o ciclo **escrever → salvar → atualizar**
