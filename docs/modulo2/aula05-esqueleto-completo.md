# 2.5 · O esqueleto completo

!!! abstract "Hoje você vai…"
    Descobrir o segredo da linha mágica, conhecer a estrutura completa de uma página "de verdade" e aprender a deixar recadinhos no código. ⏱️ ~1h

---

## Explicação

Até agora, a gente escreveu páginas "pela metade", e o navegador foi bonzinho e mostrou mesmo assim. Mas toda página profissional tem um **esqueleto completo**. Ele é sempre o mesmo, então você aprende uma vez e usa para sempre.

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="utf-8">
    <title>Título da aba</title>
  </head>
  <body>
    <!-- Tudo o que aparece na página vem aqui -->
  </body>
</html>
```

Vamos por partes:

| Parte | O que é |
|---|---|
| `<!DOCTYPE html>` | Avisa ao navegador: "isto é uma página HTML moderna". É sempre a primeira linha. |
| `<html lang="pt-BR">` | A caixa que guarda **a página inteira**. O `lang` diz em que língua ela está escrita. |
| `<head>` | A **cabeça**: informações **sobre** a página, que **não aparecem** nela. |
| `<body>` | O **corpo**: tudo o que **aparece** na página. Seus títulos, textos, listas e imagens moram aqui. |

!!! example "Pense numa roupa na loja"
    - O `<body>` é a **roupa**: é o que todo mundo vê.
    - O `<head>` é a **etiqueta de dentro**: tamanho, tecido, como lavar. Está lá, é importante, mas ninguém vê quando você está usando.

### O que vai no `<head>`?

Por enquanto, duas coisas:

- **A linha mágica, revelada!** 🪄 `<meta charset="utf-8">` diz ao navegador qual "alfabeto" a página usa. O **UTF-8** é o alfabeto que tem acentos, ç, emojis e letras de todas as línguas do mundo. Por isso o "Olá" aparecia certinho!
- **O `<title>`**: o texto que aparece **na aba do navegador** e nos resultados do Google. Não confunda com o `<h1>`, que aparece **dentro** da página.

### Comentários: recadinhos no código 📝

```html
<!-- Isto é um comentário. O navegador ignora! -->
```

Tudo o que fica entre `<!--` e `-->` é **invisível** na página. Serve para deixar recados para você mesma (ou para quem for ler o seu código): "aqui começa a parte dos bolos", "lembrar de trocar essa foto"…

---

## Exemplo pronto: o cardápio de verdade

Crie `pratica/cardapio-completo.html`:

```html
<!DOCTYPE html>
<html lang="pt-BR">
  <head>
    <meta charset="utf-8">
    <title>Cardápio | Doceria Açúcar e Afeto</title>
  </head>
  <body>
    <!-- Cabeçalho do cardápio -->
    <h1>Doceria Açúcar e Afeto</h1>
    <p>Doces feitos com <strong>muito carinho</strong>, do jeitinho que a vovó fazia.</p>

    <!-- Seção de docinhos -->
    <h2>Docinhos</h2>
    <ul>
      <li>Brigadeiro: <strong>R$ 3,00</strong></li>
      <li>Beijinho: <strong>R$ 3,00</strong></li>
    </ul>

    <!-- Seção de bolos -->
    <h2>Bolos</h2>
    <ul>
      <li>Bolo de cenoura: <strong>R$ 45,00</strong></li>
    </ul>
  </body>
</html>
```

Resultado:

<iframe class="resultado" src="../exemplos/modulo2/cardapio-completo.html" height="380" title="Resultado do exemplo"></iframe>

Abra no navegador e olhe **a aba lá em cima**: está escrito "Cardápio | Doceria Açúcar e Afeto". E os comentários? Sumiram! 🪄

### ⚡ Atalho: o esqueleto pronto

Escrever o esqueleto toda vez cansa, né? O VS Code tem um atalho (que também **não é IA**, é um modelo pronto que sempre gera a mesma coisa):

1. Crie um arquivo `.html` vazio.
2. Digite só um ponto de exclamação: `!`
3. Aperte ++tab++ (ou ++enter++, se aparecer uma sugestão).

Ele escreve o esqueleto inteiro! Vão vir umas linhas a mais, que você ainda não conhece (uma tal de `viewport`). Pode deixar lá: ela ajuda a página a ficar boa no celular, e a gente fala dela mais pra frente. Só lembre de trocar o `lang="en"` por `lang="pt-BR"`.

---

## ✏️ Mexe aí

1. Mude o texto do `<title>` e atualize. Olhe a aba!
2. Escreva um parágrafo `<p>` **dentro do `<head>`** (fora do `<body>`). O que acontece? Depois tire de lá.
3. Escreva um comentário com uma receita secreta. 🤫 Ela aparece na página?

??? question "O que aconteceu no item 2?"
    Provavelmente o parágrafo **apareceu mesmo assim**. O navegador é bonzinho e tenta consertar os nossos erros. Mas não conte com isso: em páginas maiores, essa "ajudinha" pode bagunçar tudo. **O que aparece na página vai no `<body>`.** Sempre.

!!! warning "Comentário não é cofre"
    O comentário não aparece na página, mas **qualquer pessoa pode ver o código** de um site (você vai aprender como no Módulo 3!). Então nada de senhas ou segredos de verdade em comentários. A receita secreta da vovó, só se ela deixar. 😄

---

## 🎯 Desafio 2.5

Hora de deixar a sua página `sobre-mim/index.html` profissional:

1. Coloque tudo o que você já fez dentro do **esqueleto completo**. Pode usar o atalho `!`.
2. Escreva um `<title>` assim: `Sobre mim | Seu Nome`.
3. Deixe **pelo menos 2 comentários** marcando as partes da página (por exemplo, `<!-- Apresentação -->` e `<!-- Coisas que eu amo -->`).
4. Confira no navegador se tudo continua aparecendo certinho, e se o título está na aba.

Ritual de entrega 📦: `"Desafio 2.5: esqueleto completo"`.

---

## ✅ Checklist

- [ ] Sei o esqueleto completo: `<!DOCTYPE>`, `<html>`, `<head>` e `<body>`
- [ ] Sei a diferença entre `<head>` (não aparece) e `<body>` (aparece)
- [ ] Sei para que serve o `<meta charset="utf-8">`
- [ ] Sei a diferença entre `<title>` (na aba) e `<h1>` (na página)
- [ ] Sei escrever comentários `<!-- -->`
- [ ] Sei usar o atalho `!` no VS Code
