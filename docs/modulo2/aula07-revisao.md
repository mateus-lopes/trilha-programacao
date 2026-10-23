# 2.7 · 🌿 Revisão e página "Sobre mim"

!!! abstract "Hoje você vai…"
    Revisar tudo o que aprendeu de HTML, caçar uns bugs e terminar a sua página "Sobre mim". Hoje **não tem nada novo**: é dia de juntar as peças. ⏱️ ~2h (pode dividir em dois dias!)

---

## Parte 1 · A colinha 📋

Tudo o que você aprendeu neste módulo, num lugar só. Pode voltar aqui sempre que precisar!

| Tag | Para quê | Fecha? |
|---|---|---|
| `<h1>` a `<h6>` | Títulos, do mais importante ao menos | Sim |
| `<p>` | Parágrafo | Sim |
| `<strong>` | Destaque importante (**negrito**) | Sim |
| `<em>` | Ênfase (*itálico*) | Sim |
| `<ul>` | Lista sem ordem (bolinhas) | Sim |
| `<ol>` | Lista numerada | Sim |
| `<li>` | Item de lista | Sim |
| `<img src="" alt="" width="">` | Imagem | **Não** |
| `<a href="">` | Link | Sim |
| `<table>` | Tabela | Sim |
| `<tr>` | Linha da tabela | Sim |
| `<th>` | Célula de cabeçalho | Sim |
| `<td>` | Célula de dado | Sim |
| `<!-- -->` | Comentário (invisível) | — |

E o esqueleto que toda página tem (atalho no VS Code: `!` + ++tab++):

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="utf-8">
    <title>Título da aba</title>
  </head>
  <body>
    <!-- O que aparece na página -->
  </body>
</html>
```

---

## Parte 2 · Caça aos bugs 🐞

Lembra do Brigadeirobô? Agora quem está seguindo as instruções ao pé da letra é o navegador. Cada código abaixo tem **um bug**. Tente achar sozinha antes de abrir a resposta!

**Bug 1:** o título engoliu o resto da página.

```html
<h1>Doceria Açúcar e Afeto<h1>
<p>Os melhores doces da cidade.</p>
```

??? question "Ver a resposta"
    O `<h1>` não foi fechado: faltou a **barra** no segundo. O certo é `</h1>`.

**Bug 2:** a foto não aparece, só o texto do `alt`.

```html
<!-- O arquivo na pasta se chama: bolo-de-cenoura.jpg -->
<img src="imagens/bolo de cenoura.jpg" alt="Bolo de cenoura">
```

??? question "Ver a resposta"
    O nome no `src` tem **espaços**, mas o arquivo tem **hífens**. O nome precisa ser exatamente igual: `imagens/bolo-de-cenoura.jpg`.

**Bug 3:** a lista ficou esquisita.

```html
<h2>Lista de compras</h2>
<ul>
  <li>Tênis de vôlei</li>
  <li>Legging</li>
</ul>
  <li>Garrafinha de água</li>
```

??? question "Ver a resposta"
    O último `<li>` ficou **fora** do `<ul>`. Todo item precisa estar **dentro** da lista, antes do `</ul>`.

**Bug 4:** o link não funciona direito.

```html
<a href="https://pt.wikipedia.org/wiki/Voleibol>Regras do vôlei</a>
```

??? question "Ver a resposta"
    Faltou **fechar as aspas** do `href`. O certo é `href="https://pt.wikipedia.org/wiki/Voleibol"`. Aspas sempre andam em dupla!

!!! tip "Como caçar bugs no HTML"
    Quando algo estiver estranho, confira nesta ordem:

    1. Salvei o arquivo e atualizei o navegador?
    2. Todas as tags que abrem também **fecham**?
    3. As aspas estão **em pares**?
    4. Os nomes de arquivo estão **exatamente** iguais?

---

## Parte 3 · Finalizando o "Sobre mim" 💁‍♀️

Abra a sua página `sobre-mim/index.html` e confira se ela tem **tudo isto**:

- [ ] Esqueleto completo, com `<title>` na aba
- [ ] Um `<h1>` com o seu nome
- [ ] Um parágrafo de apresentação, com algum destaque `<strong>` ou `<em>`
- [ ] Pelo menos **3 seções** com `<h2>`
- [ ] Uma lista (`<ul>` ou `<ol>`)
- [ ] Pelo menos uma imagem, com `alt`
- [ ] Pelo menos um link
- [ ] Uma tabela
- [ ] Comentários marcando as partes
- [ ] Código **organizado com recuo**, fácil de ler

Faltou alguma coisa? Complete! E se quiser, adicione o que tiver vontade: mais fotos, mais seções, outra lista… **A página é sua.** 💕

Ritual de entrega 📦: `"Desafio 2.7: sobre mim completo"`.

!!! tip "Bônus (opcional): uma segunda página"
    Crie, na mesma pasta, o arquivo `receitas.html`, com uma receita que você gosta. Depois, no `index.html`, crie um link para ela:

    ```html
    <a href="receitas.html">Minhas receitas favoritas</a>
    ```

    Repare que o `href` não começa com `https://`: quando o arquivo está **na mesma pasta**, basta o nome dele. Agora você tem um site com **duas páginas**! E lá no `receitas.html`, que tal um link de volta para o `index.html`?

---

## Parte 4 · Olha o quanto você andou 🌱

No GitHub, abra o seu repositório `desafios` e clique no **relógio** com o número de commits (perto do botão verde **Code**). Ali está o **histórico** de tudo o que você entregou, desde a Sessão 0.

Clique no commit do **Desafio 2.1** e depois no do **Desafio 2.7**. Compare: lá no começo, a sua página tinha uma linha. Agora tem esqueleto, seções, lista, foto, link e tabela.

**Você escreveu tudo isso.** 🥹

---

## 🎉 Fim do Módulo 2!

Você agora sabe **HTML**, a língua de todas as páginas da internet. Sério: os sites que você usa todo dia são feitos dessas mesmas tags que você aprendeu.

Agora, a sua página está com um **esqueleto** lindo, mas ainda com cara de documento: letra preta, fundo branco… No **Módulo 3**, chega o **CSS**, e você vai fazer a maquiagem dela: cores, fontes, espaçamentos, tudo com a sua cara. 💄

---

## ✅ Checklist do módulo

- [ ] Sei criar uma página do zero, com o esqueleto completo
- [ ] Sei usar títulos, parágrafos, destaques, listas, imagens, links e tabelas
- [ ] Sei caçar bugs no HTML
- [ ] Minha página "Sobre mim" está completa e entregue!
