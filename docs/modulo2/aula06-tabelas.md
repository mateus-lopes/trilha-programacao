# 2.6 · Tabelas

!!! abstract "Hoje você vai…"
    Montar a tabela de preços de um salão de beleza e organizar informações em linhas e colunas. ⏱️ ~1h

---

## Explicação

Algumas informações ficam muito melhores numa **tabela**: preços, horários, uma ficha de treino… Tudo o que você organizaria numa planilha.

Uma tabela é feita de **linhas**, e cada linha é feita de **células** (os quadradinhos):

| Tag | Vem do inglês | Quer dizer |
|---|---|---|
| `<table>` | *table* | A tabela inteira |
| `<tr>` | ***t**able **r**ow* | Uma **linha** |
| `<th>` | ***t**able **h**eader* | Uma célula de **cabeçalho** (o título da coluna) |
| `<td>` | ***t**able **d**ata* | Uma célula **normal**, com dado |

O jeito de pensar é **linha por linha**, de cima para baixo. Dentro de cada linha, as células vão da esquerda para a direita:

```html
<table border="1">
  <tr>                       <!-- linha 1: os títulos -->
    <th>Serviço</th>
    <th>Preço</th>
  </tr>
  <tr>                       <!-- linha 2: um serviço -->
    <td>Manicure</td>
    <td>R$ 30,00</td>
  </tr>
</table>
```

!!! note "E esse border?"
    Sem ele, a tabela fica **sem as linhas** em volta das células, e é difícil enxergar onde cada uma começa. O `border` é um jeito antigo e simples de mostrar as bordas. No Módulo 3, você vai aprender a fazer bordas **bonitas** com CSS e não vai mais precisar dele.

---

## Exemplo pronto: tabela de preços do salão 💇‍♀️

Crie `pratica/salao.html`:

```html
<meta charset="utf-8">
<h1>Studio Bela</h1>
<h2>Tabela de preços</h2>

<table border="1">
  <tr>
    <th>Serviço</th>
    <th>Preço</th>
    <th>Duração</th>
  </tr>
  <tr>
    <td>Manicure</td>
    <td>R$ 30,00</td>
    <td>40 min</td>
  </tr>
  <tr>
    <td>Pedicure</td>
    <td>R$ 35,00</td>
    <td>50 min</td>
  </tr>
  <tr>
    <td>Escova</td>
    <td>R$ 60,00</td>
    <td>1h</td>
  </tr>
</table>
```

!!! tip "Esqueleto"
    Para os exemplos ficarem curtinhos, eles continuam só com a linha mágica. Mas, se quiser praticar, coloque este exemplo dentro do esqueleto completo!

Resultado:

<iframe class="resultado" src="../exemplos/modulo2/salao.html" height="280" title="Resultado do exemplo"></iframe>

Repare que o `<th>` aparece em **negrito** e **centralizado**: o navegador já sabe que ele é um título.

!!! warning "Todas as linhas com o mesmo número de células"
    Se a primeira linha tem 3 células, **todas** as outras precisam ter 3 também. Se uma linha tiver menos, a tabela fica torta. Contar as células é a primeira coisa a fazer quando uma tabela fica estranha.

---

## ✏️ Mexe aí

1. Adicione uma linha nova para **Design de sobrancelha**, com preço e duração.
2. Adicione uma **coluna nova**, chamada **"Profissional"**. Dica: você vai precisar adicionar uma célula em **cada** linha!
3. Apague uma célula `<td>` de uma linha só e veja a tabela ficar torta. Depois conserte.

??? question "Por que adicionar uma coluna dá mais trabalho que adicionar uma linha?"
    Porque o HTML monta a tabela **linha por linha**. Uma linha nova é um bloco `<tr>` só, todo junto. Já uma coluna fica "espalhada": é uma célula a mais em cada uma das linhas. Por isso, antes de montar uma tabela, vale pensar bem quais colunas ela vai ter.

---

## 🎯 Desafio 2.6

Na sua página `sobre-mim/index.html`, crie uma nova seção com `<h2>` e uma tabela. Escolha **uma**:

- 🏋️ **"Meu treino"**: colunas **Dia** e **Treino** (ex.: Segunda | Pernas)
- 📅 **"Minha semana"**: colunas **Dia** e **O que eu faço** (ex.: Terça | Estudo programação 😎)

A tabela precisa ter uma linha de cabeçalho com `<th>` e **pelo menos 3 linhas** de dados.

Ritual de entrega 📦: `"Desafio 2.6: tabela"`.

---

## ✅ Checklist

- [ ] Sei montar uma tabela com `<table>`, `<tr>`, `<th>` e `<td>`
- [ ] Sei que a tabela é montada **linha por linha**
- [ ] Sei a diferença entre `<th>` (cabeçalho) e `<td>` (dado)
- [ ] Sei que todas as linhas precisam ter o mesmo número de células
