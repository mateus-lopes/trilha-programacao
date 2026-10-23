# 2.3 · Listas

!!! abstract "Hoje você vai…"
    Transformar a receita de brigadeiro em página, com listas de ingredientes e de passos. ⏱️ ~1h

---

## Explicação

Listas estão em todo lugar: lista de compras, ingredientes, ficha de treino, o menu de um site… O HTML tem dois tipos principais.

### Lista sem ordem: `<ul>`

Para coisas em que a **ordem não importa**, como ingredientes ou lista de compras. Cada item ganha uma bolinha (•).

```html
<ul>
  <li>Leite condensado</li>
  <li>Manteiga</li>
  <li>Chocolate em pó</li>
</ul>
```

### Lista numerada: `<ol>`

Para coisas em que a **ordem importa**, como o passo a passo de uma receita. Cada item ganha um número, **sozinho**!

```html
<ol>
  <li>Misture tudo na panela.</li>
  <li>Leve ao fogo.</li>
  <li>Mexa até desgrudar.</li>
</ol>
```

### Decifrando os nomes

| Tag | Vem do inglês | Quer dizer |
|---|---|---|
| `<ul>` | ***u**nordered **l**ist* | Lista sem ordem |
| `<ol>` | ***o**rdered **l**ist* | Lista com ordem (numerada) |
| `<li>` | ***l**ist **i**tem* | Item da lista |

Repare que **todo** item é um `<li>`, nos dois tipos de lista. O que muda é só a "caixa" de fora: `<ul>` ou `<ol>`.

!!! tip "Use o recuo para se organizar"
    Viu que os `<li>` estão um pouco para a direita? O navegador não liga para esse espaço, mas **você** liga: fica muito mais fácil enxergar o que está dentro de quê. É o mesmo recuo do Módulo 1! Para fazer, aperte ++tab++ no começo da linha.

---

## Exemplo pronto: receita de brigadeiro 🍫

Lembra da receita da lição 1.1? Agora ela vira página! Crie `pratica/brigadeiro.html`:

```html
<meta charset="utf-8">
<h1>Brigadeiro</h1>

<h2>Ingredientes</h2>
<ul>
  <li>1 lata de leite condensado</li>
  <li>1 colher (sopa) de manteiga</li>
  <li>4 colheres (sopa) de chocolate em pó</li>
  <li>Chocolate granulado</li>
</ul>

<h2>Modo de preparo</h2>
<ol>
  <li>Coloque o leite condensado, a manteiga e o chocolate numa panela.</li>
  <li>Leve ao fogo baixo, mexendo sem parar.</li>
  <li>Quando desgrudar do fundo, desligue o fogo.</li>
  <li>Espere esfriar, faça bolinhas e passe no granulado.</li>
</ol>
```

Resultado:

<iframe class="resultado" src="../exemplos/modulo2/brigadeiro.html" height="420" title="Resultado do exemplo"></iframe>

---

## ✏️ Mexe aí

1. Troque o `<ol>` do modo de preparo por `<ul>` (lembre de trocar **também** o `</ol>` de fechamento). O que acontece com os números?
2. Volte para `<ol>` e coloque um passo novo **no meio** da lista. Repare que os números se ajustam sozinhos!
3. Crie, embaixo de tudo, uma lista de compras do shopping 🛍️ com um `<h2>` e uma `<ul>`.

??? question "Por que os números se ajustam sozinhos?"
    Porque, no `<ol>`, quem coloca os números é o **navegador**, e não você. Se você escrevesse os números à mão, teria que renumerar tudo a cada passo novo. Deixar o computador fazer o trabalho chato é um dos superpoderes de programar. 😎

---

## 🎯 Desafio 2.3

Na sua página `sobre-mim/index.html`:

1. Crie um `<h2>` chamado **"Coisas que eu amo"**.
2. Embaixo dele, uma lista `<ul>` com **pelo menos 5** coisas que você ama.

Ritual de entrega 📦: `"Desafio 2.3: coisas que eu amo"`.

!!! tip "Bônus (opcional)"
    Crie também um **"Meu top 3 sobremesas"** com uma lista numerada `<ol>`, da favorita para a menos favorita.

---

## ✅ Checklist

- [ ] Sei fazer uma lista sem ordem com `<ul>`
- [ ] Sei fazer uma lista numerada com `<ol>`
- [ ] Sei que cada item é um `<li>`
- [ ] Sei escolher qual tipo de lista usar
- [ ] Uso recuo para organizar o meu código
