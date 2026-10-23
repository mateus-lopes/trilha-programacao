# 2.4 · Imagens e links

!!! abstract "Hoje você vai…"
    Montar uma vitrine de esmaltes com fotos, colocar links na página e aprender o que são **atributos**. ⏱️ ~1h

---

## Explicação

### Atributos: os detalhes da etiqueta

Até agora, as tags só diziam **o que** cada coisa é. Mas às vezes a tag precisa de **informações extras**. Uma foto, por exemplo: qual foto? De que tamanho?

Essas informações extras se chamam **atributos**. Eles ficam **dentro** da tag de abertura, sempre no formato `nome="valor"`:

```html
<img src="esmalte.jpg" alt="Esmalte rosa" width="200">
```

Aqui tem três atributos: `src`, `alt` e `width`. Repare que o valor fica sempre **entre aspas**.

### Imagens: `<img>`

```html
<img src="imagens/esmalte-rosa.svg" alt="Vidro de esmalte rosa" width="80">
```

| Atributo | Para quê |
|---|---|
| `src` | **Onde** está a imagem (de *source*, "fonte") |
| `alt` | Uma **descrição** da imagem, em texto |
| `width` | A **largura** da imagem, em pixels (os pontinhos da tela) |

!!! note "A tag que não fecha"
    O `<img>` é uma das poucas tags que **não tem fechamento**. Faz sentido: não existe "conteúdo" dentro de uma imagem, a própria imagem é o conteúdo.

!!! tip "Por que o `alt` é importante?"
    O `alt` aparece quando a imagem não carrega. E pessoas cegas usam programas que **leem a página em voz alta**: é o `alt` que conta para elas o que tem na foto. Sempre escreva um!

### Onde fica a imagem: o caminho

O `src="imagens/esmalte-rosa.svg"` quer dizer: "a partir de onde esta página está, entre na pasta `imagens` e pegue o arquivo `esmalte-rosa.svg`". Isso se chama **caminho**.

```
pratica/
├── vitrine.html        ← a página está aqui
└── imagens/
    └── esmalte-rosa.svg   ← e a imagem está aqui
```

!!! warning "Nomes de arquivo sem surpresas"
    O nome no `src` precisa ser **exatamente igual** ao nome do arquivo, letra por letra, incluindo a extensão (`.jpg`, `.png`, `.webp`, `.svg`…). Para evitar dor de cabeça, dê nomes:

    - **sem espaços** (use `-` no lugar): `esmalte-rosa.jpg` ✅ `esmalte rosa.jpg` ❌
    - **sem acentos**: `cafe.jpg` ✅ `café.jpg` ❌
    - **em letras minúsculas**

### Links: `<a>`

```html
<a href="https://pt.wikipedia.org/wiki/Esmalte_de_unha">Leia sobre esmaltes na Wikipédia</a>
```

- `href` é **para onde** o link leva (o endereço do site).
- O texto entre `<a>` e `</a>` é o que aparece **para clicar**.

O **a** vem de *anchor*, que quer dizer "âncora" em inglês.

---

## Exemplo pronto: vitrine de esmaltes 💅

### 1. Baixando as imagens

1. Dentro da pasta `pratica`, crie uma pasta chamada `imagens`.
2. Baixe as três imagens abaixo: clique com o **botão direito** em cada link → **Salvar link como…** → salve na pasta `pratica/imagens`.
    - [esmalte-rosa.svg](../exemplos/modulo2/imagens/esmalte-rosa.svg)
    - [esmalte-vermelho.svg](../exemplos/modulo2/imagens/esmalte-vermelho.svg)
    - [esmalte-nude.svg](../exemplos/modulo2/imagens/esmalte-nude.svg)

### 2. O código

Crie `pratica/vitrine.html`:

```html
<meta charset="utf-8">
<h1>Vitrine de esmaltes 💅</h1>

<h2>Rosa Chiclete</h2>
<img src="imagens/esmalte-rosa.svg" alt="Vidro de esmalte rosa" width="80">
<p>Cremoso, ótimo para o verão.</p>

<h2>Vermelho Paixão</h2>
<img src="imagens/esmalte-vermelho.svg" alt="Vidro de esmalte vermelho" width="80">
<p>O clássico que nunca sai de moda.</p>

<h2>Nude Areia</h2>
<img src="imagens/esmalte-nude.svg" alt="Vidro de esmalte nude" width="80">
<p>Discreto e elegante.</p>

<p>Quer saber mais sobre cuidados com as unhas? <a href="https://pt.wikipedia.org/wiki/Esmalte_de_unha">Leia sobre esmaltes na Wikipédia</a>.</p>
```

Resultado:

<iframe class="resultado" src="../exemplos/modulo2/vitrine.html" height="560" title="Resultado do exemplo"></iframe>

!!! tip "Dá para usar emoji!"
    Viu o 💅 no título? Emojis funcionam direto no HTML, graças à linha mágica. No Windows, aperte ++win+period++ para abrir o teclado de emojis (no Mac, ++ctrl+cmd+space++).

---

## ✏️ Mexe aí

1. Mude o `width` de um esmalte para `200`. E para `20`. 🔍
2. **Estrague de propósito** o `src` de uma imagem (troque `rosa` por `roza`). O que aparece no lugar da foto? Depois conserte.
3. Troque o link da Wikipédia pelo site da sua loja de roupa favorita.

??? question "O que apareceu no item 2?"
    Apareceu o **texto do `alt`** (e, dependendo do navegador, um ícone de imagem quebrada). É o navegador avisando: "não encontrei a imagem, mas olha a descrição dela". Quando uma imagem não aparecer, **a primeira coisa a conferir é o nome do arquivo no `src`**.

---

## 🎯 Desafio 2.4

Na sua página `sobre-mim/index.html`:

1. Crie a pasta `sobre-mim/imagens`.
2. Salve lá uma **foto de algo que você ama** (sua sobremesa favorita, uma bola de vôlei, um esmalte…). Pode ser da internet: botão direito na imagem → **Salvar imagem como…**. Lembre das regras de nome!
3. Coloque a foto na página com `<img>`, com um `alt` caprichado e um `width` que deixe ela num tamanho bom.
4. Coloque um **link** para um site que você gosta, com um texto explicando o que é.

Ritual de entrega 📦: `"Desafio 2.4: foto e link"`. A imagem vai junto na entrega, porque o `git add .` pega tudo!

!!! warning "Fotos pessoais"
    No Módulo 4, esta página vai para a internet, e **qualquer pessoa** vai poder ver. Por isso, escolha agora só fotos que você não se importa de mostrar para todo mundo. 😉

---

## ✅ Checklist

- [ ] Sei o que é um **atributo** (`nome="valor"`)
- [ ] Sei colocar imagens com `<img>`, usando `src`, `alt` e `width`
- [ ] Sei o que é um **caminho** e por que o nome do arquivo precisa ser exato
- [ ] Sei criar links com `<a href="...">`
