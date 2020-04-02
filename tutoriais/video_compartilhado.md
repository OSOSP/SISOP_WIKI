# Como criar um Link Compartilhado no Google Drive

### Passo 1

* Se deseja baixar um Vídeo do Youtube pelo Linux, baixe o programa **youtube-dl**
* Comandos de Instalação:
    * Baixe o Python: `sudo apt install python`
    * Baixe o pip do Python: `sudo apt install python-pip`
    * Baixe o Programa youtube-dl pelo pip: `sudo -H pip install --upgrade youtube-dl`
* Quando o programa estiver instalado, copie o link do video, clicando com o segundo botão do mouse no video e clicando em **copy video url**
* Vá no terminal e coloque: `youtube-dl linkDoVideo`
* Vai baixar o programa no Diretório onde vc estiver

### Passo 2

* Quando estiver baixado, enviamos para o google drive e seguimos os seguintes passos para criar um Link compartilhável
1. Clicamos com o segundo botão no vídeo e selecionamos **Geral Link Compartilhável**
2. Clicamos para gerar um Link Compartilhável
3. Clique em **configurações de compartilhamento**
4. Clique para alterar as pessoas que podem ver e selecione **mais**
5. Defina que qualquer um que tiver esse link pode ver o vídeo
6. Copie o Link do Vídeo

**Exemplo**

---

<img src="images/google_drive/sharing_video.gif">

---


### Passo 3

* Abra a sua Wiki com um Editor de texto(no meu caso é o vscode)
* crie a estrutura `[![]()]()`
* na estrutura interna `![]()` vai a imagem que vai aparecer como um Link
    * Ex: `![nomeDaImagem](caminhoParaAImagem)`
* na estrutura externa `[]()` dentro do **[]** fica a extrutura da imagem e a **()** fica o link do google drive

**Exemplo**

---

<img src="images/google_drive/link_videos.png">

---

#### Finalização

* Toda vez que alguem clicar na imagem, vai direto para o Link do Google Drive Público, que somente pode ser acessado por esse Link

**Exemplo**

---

<img src="images/google_drive/">

---