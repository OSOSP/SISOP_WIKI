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

---

* Markdown é uma Linguagem de Texto que estrutura como o Texto vai aparecer, essa Wiki toda é feita utilizando essa linguagem.
* Existem estruturas especificas para usar quando escreve em Markdown, onde podemos inventar coisas interessantes com elas.

**CRIANDO ABA DE TELAS**

* Podemos criar um Header com todos os Links vinculando telas, onde usamos a seguinte estrutura

```markdown
[]()
|---|
```
* O simbolo `[]()` serve para colocarmos o nome da tela(nos **[]**) e o link para o Markdown da tela(nos **()**).
* O simbolo `|---|` serve para estruturar esse link como em uma **Aba**, onde cada link deve ter um desses.
* Exemplo em Markdown:

```markdown
[Página Inicial](Home)|[Aulas do Professor](Aulas_Professor)
|---|---|
```

* Exemplo na prática:

[Página Inicial](Home)|[Aulas do Professor](Aulas_Professor)
|---|---|


**COLOCANDO TEXTO EM NEGRITO**

* Podemos colocar o texto que estamos escrevendo em negrito usando `**` em cada lado do texto.
* Exemplo em Markdown:

```text
**Texto**
```

* Exemplo na Prática: **Texto**

**COLOCANDO O TEXTO EM ITÁLICO**

* Podemos colocar o texto que estamos trabalhando em itálico usando `_` em cada lado do texto.
* Exemplo em Markdown:

```text
_Texto_
```

* Exemplo na prática: _Texto_

**MARCANDO TEXTO ESPECIFICO**

* Se usar **`** em cada lado do texto vai fazer com que o texto fique sublinhado
* Exemplo em Markdown:

```text
`Texto`
```

* Exemplo na prática: `Texto`

**CRIANDO TABELAS**

* Podemos criar facilmente tabelas, onde somente temos que dividir em colunas usando **|**.
* Para marcar o titulo das Colunas, devemos embaixo de cada titulo colocar **|---|**
* Exemplo em Markdown:

```markdown
Primeia Coluna | Segunda Coluna
|---|---|
Linha 1, Coluna 1| Linha 1, Coluna 2
Linha 2, Coluna 1| Linha 2, Coluna 2
```

* Exemplo na Prática:

Primeia Coluna | Segunda Coluna
|---|---|
Linha 1, Coluna 1| Linha 1, Coluna 2
Linha 2, Coluna 1| Linha 2, Coluna 2

**TÍTULOS**

* Podemos colocar um Título em cada página da Wiki usando uma **#** antes de cada titulo
* Quanto mais **#** colocamos, menor o título vai ficando
* Exemplo em Markdown:

```markdown
# Titulo Maior
## Sub-titulo Menor
### Menor ainda
#### Menor ainda
```

* Exemplo prático:

# Titulo Maior
## Sub-titulo Menor
### Menor ainda
#### Menor ainda

**DIVISÃO DE TEXTOS**

* Usamos os Símbolos **---** antes e depois de um texto para deixar ele separado do resto
* Exemplo em Markdown:

```markdown
---

Texto Separado

---

```

* Exemplo na prática:

---

Texto Separado

---

**SEPARANDO TEXTOS**

* Como você pode ter percebido, existe um ponto escuro no inicio de cada linha de texto, esse ponto é um `*` colocado no inicio de cada linha de texto, onde com ele podemos separar o texto em tópicos.
* Quando mais `*` forem colocado com um espaço ele vai criando sub-tópicos para um assunto.
* Exemplo em Markdown:

```markdown
* A
    * A.1
        * A.1.1
            * A.1.1.1
```

* Exemplo Prático:

* A
    * A.1
        * A.1.1
            * A.1.1.1

* Podemos também usar números, colocando um ponto do lado do número
* Exemplo em Markdown:

```markdown
1. A
    1. A.1
2. B
    1. B.1
        1. B.1.1
```

* Exemplo na Prática:

1. A
    1. A.1
2. B
    1. B.1
        1. B.1.1

**COLOCANDO CÓDIGO NO TEXTO**

* Uma coisa incrivel do Markdown é que podemos fazer highlight de código usando a seguinte estrutura em Markdown:

<img src="images/wiki_manager/markdown_code.png">

* Sempre coloque o nome da linguagem que deseja fazer highlight depois dos primeiros **```**

* Na prática fica assim:

```java
public class Teste{
    public static void main(String[] args){
        System.out.println("Hello World"):
    }
}
```

**Link de Acesso Rápido**

* Podemos colocar uma tag em uma área do Texto para o sistema ir mais rápido até o conteúdo se ele for muito extenso.




