[Página Inicial](Home)|
|---|

# Como Gerênciar Páginas de Wiki

* Escrever em uma Wiki nada mais nada menos é como escrever um Programa.
* Temos que definir os links e informações que serão mostrados, para isso existem formas fáceis de mexer com uma Wiki

### Conteúdo 1: NÃO ALTERAR A WIKI PELA WEB

---

* A wiki, sendo no Github,Gitlab ou BitBucket funcionam de duas Formas:
    1. Pode Gerênciar uma Página pela própria Web 
    2. Pode Gerênciar as Páginas usando um Editor de Texto

* A primeira forma é a pior forma de mexer com Wikis, devido que como trabalhamos com imagens e links, é extremamente não prático mexermos com essas informações pela web
* Imagens e Links podem quebrar se for mudado de localização e isso pode ser uma grande dor de cabeça com o tempo, para isso usamos editores de texto para trabalharmos.

---

### Conteúdo 2: COMO GERÊNCIAR SUA WIKI

---

* Uma Wiki nada mais é que um Repositório que pode ser baixado para editar, onde funciona da seguinte forma:
    * O link de um repositório normal, como este, para clonar é o seguinte:
        * `https://github.com/F4NT0/SISOP.git`
    * O link de uma Wiki, como deste projeto possui um **.wiki**, como exemplo:
        * `https://github.com/F4NT0/SISOP.wiki.git`
<br>

* Para baixar a Wiki de um projeto, faça como o .gif abaixo

<img src="images/wiki_manager/wiki_clone.gif">

---

### Conteúdo 3: COMO COLOCAR IMAGENS

---

* Nunca coloque uma imagem como **Attach** direto pela web, porque com isso a imagem fica em um limbo de links aleatorios criados pelo Github, fazendo com que quando migrar a wiki é perdido todas as fotos e videos.

* Para colocar imagem se deve colocar a imagem dentro de um diretório pelo seu editor de texto favorito, onde você cria o Diretório e coloca as imagens.

* Abaixo o exemplo deste Diretório

<img src="images/wiki_manager/image_folder.png">

* Depois de colocado a imagem no Diretório, devemos chamar a imagem no texto markdown por via de tag ou por via de estrutura de imagem:

**Chamando por Tag**

* Podemos utilizar a tag de imagem do HTML para poder chamar uma imagem de dentro do nosso diretório, como no diretório acima queremos pegar a logo do nosso Sistema Operacional:
* O caminho até a Imagem é `images/sovaco_logo.png`
* Se o seu arquivo Markdown se encontra no Diretório Raiz de sua wiki(o diretório principal da wiki) fica mais fácil de chamar o caminho até o diretório, ficando assim

```html
<img src="images/sovaco_logo.png">
```

* Se estiver mais interno, vai colocando **..** até o local da imagem,como por exemplo

```html
<img src="../images/sovaco_logo.png">
```

* Com a estrutura da Tag podemos redefinir o tamanho da imagem como quisermos, onde somente temos que chamar o **Width** ou o **Height** que queremos da imagem.

```html
<img src="images/sovaco_logo.png" width="200">
```

**Chamando por Estrutura de Imagem**

* Markdown possui uma estrutura própria que serve para chamar uma imagem da mesma forma que a tag, mas não podemos alterar o tamnho ou modificar ela.
* Essa estrutura é assim:  `![]()`
* Colocamos dentro dos **[]** o nome da imagem que queremos
* Colocamos dentro dos **()** o caminho até a imagem

```markdown
![minha imagem](images/sovaco_logo.png)
```

---

### Conteúdo 4: COMO ESCREVER EM MARKDOWN

* Markdown é uma Linguagem de Texto que estrutura como o Texto vai aparecer, essa Wiki toda é feita utilizando essa linguagem.
* Existem estruturas
