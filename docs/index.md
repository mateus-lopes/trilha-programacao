---
title: Início
hide:
  - navigation
  - toc
---

<style>
/* Landing da página inicial: só vale aqui dentro de .tp-landing. As cores vêm do tema, então
   o modo claro e o escuro funcionam sozinhos. */
.tp-landing { --tp-raio: 16px; }
.tp-hero {
  text-align: center;
  padding: 2.5rem 0 2rem;
}
.tp-hero .tp-broto { font-size: 3.2rem; line-height: 1; }
.md-typeset .tp-hero .tp-titulo {
  display: block;
  margin: 0.8rem 0 0.6rem;
  font-size: clamp(1.9rem, 6vw, 3rem);
  font-weight: 800;
  line-height: 1.15;
  letter-spacing: -0.02em;
  color: var(--md-default-fg-color);
}
.tp-hero .tp-titulo span { color: var(--md-primary-fg-color); }
.md-typeset .tp-hero .tp-sub {
  max-width: 34rem;
  margin: 0 auto 1.6rem;
  font-size: 1.05rem;
  color: var(--md-default-fg-color--light);
}
.tp-acoes { display: flex; flex-wrap: wrap; gap: 0.6rem; justify-content: center; }
.md-typeset .tp-acoes .md-button { margin: 0; }
.tp-selos {
  display: flex; flex-wrap: wrap; gap: 0.5rem; justify-content: center;
  margin-top: 1.4rem; font-size: 0.8rem; color: var(--md-default-fg-color--light);
}
.tp-selos span {
  padding: 0.25rem 0.7rem; border-radius: 99px;
  background: var(--md-code-bg-color);
}
.md-typeset .tp-landing h2 {
  text-align: center; margin: 2.6rem 0 1.2rem; font-weight: 700;
}
.tp-grade {
  display: grid; gap: 0.8rem;
  grid-template-columns: repeat(auto-fit, minmax(13rem, 1fr));
}
.tp-cartao {
  padding: 1rem 1.1rem; border-radius: var(--tp-raio);
  background: var(--md-code-bg-color);
  border: 1px solid var(--md-default-fg-color--lightest);
}
.tp-cartao .tp-emoji { font-size: 1.6rem; line-height: 1; }
.md-typeset .tp-cartao strong { display: block; margin: 0.5rem 0 0.2rem; }
.md-typeset .tp-cartao p { margin: 0; font-size: 0.85rem; color: var(--md-default-fg-color--light); }
.tp-trilha { list-style: none; margin: 0 !important; padding: 0; }
.md-typeset .tp-trilha li { margin: 0; }
.tp-passo {
  display: flex; gap: 0.9rem; align-items: flex-start;
  padding: 0.8rem 0.4rem; border-bottom: 1px solid var(--md-default-fg-color--lightest);
}
.md-typeset a.tp-passo, .md-typeset a.tp-passo:hover { text-decoration: none; }
.md-typeset a.tp-passo { color: inherit; border-radius: 10px; transition: background 0.15s; }
.md-typeset a.tp-passo:hover { background: var(--md-code-bg-color); }
.md-typeset a.tp-passo:hover .tp-nome { color: var(--md-primary-fg-color); }
.tp-num {
  flex: none; display: flex; align-items: center; justify-content: center;
  width: 2rem; height: 2rem; border-radius: 99px; font-weight: 700; font-size: 0.85rem;
  background: var(--md-primary-fg-color); color: var(--md-primary-bg-color);
}
.tp-passo.em-breve .tp-num { background: var(--md-code-bg-color); color: var(--md-default-fg-color--light); }
.md-typeset .tp-passo p { margin: 0; font-size: 0.85rem; color: var(--md-default-fg-color--light); }
.tp-passo .tp-nome { font-weight: 600; }
.tp-passo.em-breve .tp-nome { color: var(--md-default-fg-color--light); }
.tp-breve {
  margin-left: 0.4rem; font-size: 0.7rem; font-weight: 600; padding: 0.1rem 0.5rem;
  border-radius: 99px; background: var(--md-code-bg-color); color: var(--md-default-fg-color--light);
}
.tp-final { text-align: center; padding: 1rem 0 0.5rem; }
</style>

<div class="tp-landing" markdown>

<section class="tp-hero">
  <div class="tp-broto">🌱</div>
  <h1 class="tp-titulo">Aprenda a programar <span>do zero</span>, no seu ritmo.</h1>
  <p class="tp-sub">Uma trilha leve, com lições curtinhas e projetos com a sua cara. Não precisa saber nada antes: nem o que é código, nem inglês de computador, nem matemática difícil.</p>
  <div class="tp-acoes">
    <a class="md-button md-button--primary" href="modulo0/">Começar a trilha →</a>
    <a class="md-button" href="#como-funciona">Ver os módulos</a>
  </div>
  <div class="tp-selos">
    <span>⏱️ Lições de ~1 hora</span>
    <span>🆓 Gratuito</span>
    <span>🧡 Sem pressa</span>
  </div>
</section>

## O que você vai criar

<div class="tp-grade">
  <div class="tp-cartao"><div class="tp-emoji">💁‍♀️</div><strong>Página "Sobre mim"</strong><p>Bonita e publicada na internet, com um link só seu.</p></div>
  <div class="tp-cartao"><div class="tp-emoji">🏐</div><strong>Placar de vôlei</strong><p>Um placar que funciona com botões.</p></div>
  <div class="tp-cartao"><div class="tp-emoji">🏋️</div><strong>Contador de séries</strong><p>Para usar na academia.</p></div>
  <div class="tp-cartao"><div class="tp-emoji">🛍️</div><strong>Carrinho de compras</strong><p>Que soma o total sozinho.</p></div>
  <div class="tp-cartao"><div class="tp-emoji">🏆</div><strong>Projeto final</strong><p>Escolhido por você, juntando tudo.</p></div>
</div>

## Como a trilha é organizada { #como-funciona }

<ol class="tp-trilha">
  <li><a class="tp-passo" href="modulo0/"><span class="tp-num">0</span><span><span class="tp-nome">Preparando o cantinho</span><p>Deixar o computador pronto e entender como estudar por aqui.</p></span></a></li>
  <li><a class="tp-passo" href="modulo1/"><span class="tp-num">1</span><span><span class="tp-nome">Pensando como programadora</span><p>O que é programar, sem nenhum código ainda.</p></span></a></li>
  <li><div class="tp-passo em-breve"><span class="tp-num">2</span><span><span class="tp-nome">HTML</span><span class="tp-breve">em breve</span><p>Criar páginas: o esqueleto de todo site.</p></span></div></li>
  <li><div class="tp-passo em-breve"><span class="tp-num">3</span><span><span class="tp-nome">CSS</span><span class="tp-breve">em breve</span><p>Deixar as páginas bonitas: a maquiagem do site 💄</p></span></div></li>
  <li><div class="tp-passo em-breve"><span class="tp-num">4</span><span><span class="tp-nome">Página no ar</span><span class="tp-breve">em breve</span><p>Publicar a sua página na internet.</p></span></div></li>
  <li><div class="tp-passo em-breve"><span class="tp-num">5</span><span><span class="tp-nome">JavaScript</span><span class="tp-breve">em breve</span><p>Dar vida às páginas: botões, contas e decisões.</p></span></div></li>
  <li><div class="tp-passo em-breve"><span class="tp-num">6</span><span><span class="tp-nome">Projeto final</span><span class="tp-breve">em breve</span><p>Juntar tudo num projeto seu.</p></span></div></li>
</ol>

!!! tip "Uma coisa importante antes de tudo"
    **Não existe pressa aqui.** Você não está atrasada, não está competindo com ninguém e pode parar quando precisar. Aprender a programar é como treinar na academia: o que faz diferença é ir com constância, não ir com tudo num dia só.

<div class="tp-final">
  <a class="md-button md-button--primary" href="modulo0/">Começar pelo Módulo 0 →</a>
</div>

</div>
