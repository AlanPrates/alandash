---
layout: post
title: "Atividade Web /IFBA-Campus Ilhéus"
description: Atividade prática avaliativa Página Barbearia
tags: tutorial
---

                        ATIVIDADE PRÁTICA AVALIATIVA: PÁGINA BARBEARIA

ORIENTAÇÕES:

• Atividade em grupo de até 3 componentes
• Prazo de entrega: Até 28/04/2022

ATIVIDADE:

Utilizando as TAGS de textos e imagens, vídeo, tabelas e as regras CSS já estudadas (inclusive
POSICIONAMENTO), elabore uma página de uma fictícia barbearia chamada “Barba & Bigode” com a
estrutura semelhante a apresentada abaixo

1. As imagens utilizadas estão disponíveis nos arquivos do TEAMS.
2. Desenvolva uma página HTML e o código CSS em arquivo externo.
3. Além da página principal, você deverá criar três outras páginas: nerd, pai e ator. Estas páginas
   devem ser ligadas através de links na página principal. Utilize imagens como links. OBS: Em cada
   uma das páginas criadas adicione um <h1> para o título correspondente: O pai, O nerd e o Ator.`YYYY-MM-DD-name-of-post.ext`

   [Demostração do site pronto][demostração-do-site-pronto]

   [Material complementar][material-complementar]

`Pagina index.html`

```html
<!DOCTYPE html>
<!--
To change this license header, choose License Headers in Project Properties.
To change this template file, choose Tools | Templates
and open the template in the editor.
-->
<html>
  <head>
    <title>Barba e Bigode</title>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link href="estilo.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="topo">
      <img src="imagens/logo.jpg" alt="" />
    </div>

    <header class="header">
      <nav>
        <ul class="menu">
          <li><a href="/">HOME</a></li>
          <li><a href="/">FOTOS & TENDÊNCIAS</a></li>
          <li><a href="/">LOCALIZAÇÃO</a></li>
          <li><a href="/">TRABALHE CONOSCO</a></li>
          <li><a href="/">NOSSAS FILIAS</a></li>
          <li><a href="/">CONTATO</a></li>
        </ul>
      </nav>
    </header>

    <div class="background"></div>

    <h1>Estilos</h1>
    <section class="flex">
      <div>
        <img src="imagens/ator.jpg" />
        <h3>Ator</h3>
      </div>
      <div>
        <img src="imagens/nerd.jpg" />
        <h3>Nerd</h3>
      </div>
      <div>
        <img src="imagens/pai.jpg" />
        <h3>Pai</h3>
      </div>
    </section>

    <h1>Dicas</h1>
    <p>Veja a dica de nossos especialistas</p>
    <div class="videos">
      <video controls loop>
        <source src="videos/dicas_fortalecer.mp4" type="video/mp4" />
        Seu navegador não suporta este formato de vídeo.
      </video>

      <video controls>
        <source src="videos/dicas_fortalecer.mp4" type="video/mp4" />
        Seu navegador não suporta este formato de vídeo.
      </video>

      <video controls>
        <source src="videos/dicas_fortalecer.mp4" type="video/mp4" />
        Seu navegador não suporta este formato de vídeo.
      </video>
    </div>
  </body>

  <rodape class="rodape">
    <ul class="rd">
      <li>
        <a href="/"
          >Copyright © 2021/\2022 Barba Bigode . All rights reserved.</a
        >
      </li>
    </ul>
  </rodape>
</html>
.
```

`Pagina Style.css`

```css
body,
ul,
li,
p {
  margin: 0px;
  padding: 0px;
  list-style: none;
  font-size: 1.2rem;
  font-family: Arial;
}

a {
  text-decoration: none;
  color: green;
}

h1 {
  margin-left: 115px;
  margin-top: 100px;
}
p {
  margin-left: 40px;
  color: green;
}
td {
}
img {
  max-width: 100%;
  /*display: block;*/
}
h3 {
  margin-left: 100px;
  color: green;
}

.topo {
  text-align: center;
}

.header {
  background: #000;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}
.menu {
  display: flex;
}
.menu li {
  margin-left: 90px;
}
.menu li a {
  display: block;
  padding: 10px;
}

.background {
  width: 100%;
  height: 500px;
  background-image: url(imagens/bigode.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.flex {
  display: flex;
  flex-wrap: wrap;
  max-width: 2000px;
  margin-left: 100px;
}
.flex > div {
  flex: 1 1 200px;
  margin: 20px;
}

.videos {
  display: flex;
  margin-top: 50px;
}
.videos > video {
  width: 320px;
  height: 240px;
  flex: 1 1 200px;
  margin: 20px;
}

.rodape {
  background: #000;
  display: flex;
  padding: 50px;
}

.rd {
  display: flex;
}
.rd li {
  margin-left: 600px;
}
```

![image](https://alandash.vercel.app/img/bigode.jpeg){: .modal}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
[demostração-do-site-pronto]: https://alandash.vercel.app/progetos/index.html
[material-complementar]: https://alandash.vercel.app/progetos/materiais-da-atividade.zip
