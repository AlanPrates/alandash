---
layout: post
title: "Sistema de Arquivo Linux /PT-BR"
tags: tutorial
comments: true
---

Utilizando comandos Bourne shell (sh) crie a árvore de diretórios representada na figura abaixo e
os arquivos solicitados, numa CLI (command line interface) Linux (emulador JSLinux1
), considerando, estritamente o que se pede nos passos a seguir (um comando por passo).

![image](https://raw.githubusercontent.com/AlanPrates/img/main/Captura%20da%20Web_17-4-2022_23250_.jpeg){: .modal}

1. Crie os diretórios da estrutura acima a partir do diretório raiz do emulador JSLinux.
2. Sem utilizar um editor de texto, crie, no diretório Direito, um arquivo chamado a.txt, cujo
   conteúdo deverá ser: "Tenho que estudar mais!".
3. Mova o arquivo a.txt para o diretório Baixo.
4. Copie o arquivo a.txt para o diretório Esquerdo.
5. Mude o nome do arquivo a.txt (diretório Esquerdo) para b.txt.
6. Copie o diretório Meio para dentro do diretório Direito.
7. Elimine o diretório Meio criado no passo (1).
8. Copie os conteúdos dos arquivos a.txt e b.txt para um novo arquivo no diretório SO, chamado
   c.txt.
   O script acima deve ser entregue num arquivo TXT, sendo a primeira linha o nome da equipe
   (dupla).

```
1/root@pop-os:/$ mkdir -p so/{esquerdo,meio/baixo,direito}

2/root@pop-os:/$ echo 'Tenho que estudar mais!' > so/direito/a.txt

3/root@pop-os:/$ mv so/direito/a.txt so/meio/baixo/

4/root@pop-os:/$ cp so/meio/baixo/a.txt so/esquerdo/

5/root@pop-os:/$ mv so/esquerdo/a.txt so/esquerdo/b.txt

6/root@pop-os:/$ cp -R so/meio so/direito/

7/root@pop-os:/$ rm -rf so/meio/

8/root@pop-os:/$ cat so/esquerdo/b.txt so/direito/meio/baixo/a.txt > so/c.txt
```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
