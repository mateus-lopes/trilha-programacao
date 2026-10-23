# 2.2 · Títulos e parágrafos

!!! abstract "Hoje você vai…"
    Montar o cardápio de uma doceria com títulos, subtítulos e parágrafos, e dar destaque às partes importantes. ⏱️ ~1h

---

## Explicação

### Títulos: do maior para o menor

O HTML tem **seis** tamanhos de título, do `<h1>` ao `<h6>`. O **h** vem de *heading*, que quer dizer título em inglês.

Mas eles não servem só para mudar o tamanho da letra. Eles mostram **o que é mais importante e o que está dentro de quê**, como as seções de um cardápio:

```text
h1  Doceria Açúcar e Afeto        ← o nome da doceria (o mais importante)
h2      Docinhos                  ← uma seção do cardápio
h3          Brigadeiro            ← um item dentro da seção
h3          Beijinho
h2      Bolos                     ← outra seção
h3          Bolo de cenoura
```

Lembrou do **recuo** do Módulo 1? É a mesma ideia: o que está mais para dentro pertence ao que está em cima. 😉

!!! tip "Regrinhas dos títulos"
    - Use **um só** `<h1>` por página. Ele é o título principal.
    - Não pule níveis: depois de um `<h2>`, vem um `<h3>`, não um `<h5>`.
    - Na prática, quase sempre você vai usar só do `<h1>` ao `<h3>`.

### Parágrafos

Todo texto corrido vai dentro de `<p>`, de **p**arágrafo. Cada `<p>` vira um bloquinho de texto com um espaço em volta.

!!! warning "Apertar Enter no código não pula linha na página"
    O navegador **ignora** os Enters e os espaços extras que você coloca no código. Para separar textos, use parágrafos `<p>` diferentes.

### Dando destaque

Dentro de um parágrafo, você pode destacar pedacinhos:

| Tag | Para quê | Como aparece |
|---|---|---|
| `<strong>` | Algo **importante** | **Negrito** |
| `<em>` | Uma **ênfase**, um jeito diferente de falar | *Itálico* |

---

## Exemplo pronto: cardápio da doceria 🍰

Crie o arquivo `pratica/cardapio.html` com este código:

```html
<meta charset="utf-8">
<h1>Doceria Açúcar e Afeto</h1>
<p>Doces feitos com <strong>muito carinho</strong>, do jeitinho que a vovó fazia.</p>

<h2>Docinhos</h2>

<h3>Brigadeiro</h3>
<p>O clássico de chocolate, com granulado. <strong>R$ 3,00</strong></p>

<h3>Beijinho</h3>
<p>Coco e leite condensado, com um cravo em cima. <strong>R$ 3,00</strong></p>

<h2>Bolos</h2>

<h3>Bolo de cenoura</h3>
<p>Com cobertura de chocolate <em>bem molhadinha</em>. <strong>R$ 45,00</strong></p>
```

Abra no navegador. Deve ficar assim:

<iframe class="resultado" src="../exemplos/modulo2/cardapio.html" height="460" title="Resultado do exemplo"></iframe>

!!! note "Tag dentro de tag"
    Reparou no `<strong>` **dentro** do `<p>`? Tags podem ficar umas dentro das outras. A regra é: **a última que abriu é a primeira que fecha**. Igual a guardar uma caixinha dentro de uma caixa: primeiro você fecha a caixinha, depois a caixa.

    ✅ `<p>Texto <strong>importante</strong></p>`

    ❌ `<p>Texto <strong>importante</p></strong>`

---

## ✏️ Mexe aí

1. Adicione o **Bolo de chocolate** na seção de Bolos, com descrição e preço.
2. Crie uma seção nova, **Tortas**, com pelo menos uma torta.
3. Troque um `<h3>` por `<h1>` e veja o que acontece. Depois desfaça.
4. Coloque `<em>` em alguma palavra da descrição do beijinho.

??? question "Por que não posso usar h1 só porque fica grande?"
    Porque o título não é sobre **tamanho**, é sobre **importância**. Programas que leem a tela para pessoas cegas, e o Google, usam os títulos para entender como a página é organizada. O tamanho e a aparência a gente muda depois com CSS, do jeito que quiser!

---

## 🎯 Desafio 2.2

Na sua página `sobre-mim/index.html`:

1. Embaixo do `<h1>` com o seu nome, escreva **um parágrafo se apresentando**, com 2 ou 3 frases. Quem é você, o que você faz, o que gosta de fazer.
2. Use `<strong>` em pelo menos **uma** coisa importante.
3. Crie um `<h2>` chamado **"Por que estou aprendendo a programar"** e escreva um parágrafo sobre isso.

Ritual de entrega 📦: `"Desafio 2.2: apresentação"`.

---

## ✅ Checklist

- [ ] Sei usar títulos do `<h1>` ao `<h3>`, do mais importante para o menos
- [ ] Sei que só deve existir **um** `<h1>` por página
- [ ] Sei usar parágrafos `<p>`
- [ ] Sei destacar com `<strong>` e `<em>`
- [ ] Sei que a última tag que abriu é a primeira que fecha
