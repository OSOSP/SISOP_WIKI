# Wiki de Organização do nosso Repositório

### Nome de Branchs
* Nome das Branchs Funcionam das seguinte formas
   * **Branch de uma Tarefa**
       * A Branch deve ser feita primeiro com o Número da Issue vinculada
          * Ex: Issue #4 - Criar Funções = Nome da Branch: `4_Functions`
   * **Branch de teste de outras Branchs**
       * Quando queremos testar dados de duas Branchs, criamos uma branch e fazemos merge das duas nela
          * Ex: Branch 4_Functions com a Branch 3_Tests = Nome da Branch: `connect_Functions_Tests`
   * **Branch para arrumar um Bug existente de outra Branch**
       * Nunca devemos modificar uma Branch já feita Merge e nem direto na Master, para isso criamos outra branch vinda da Master e arrumamos os bugs nela
          * Ex: quando queremos arrumar Funções de uma Branch já Mergeada ou da Master = Nome da Branch: `bugfix_Functions`

### Mensagem de Commits
* As mensagens de commit devem ser um resumo do que foi modificado, principalmente em inglês


### Comandos Básicos de Git

**GLOSSÁRIO**

<link do repo> = nessa área você coloca o link do Repositório externo do Git(sem as <>)
<nome branch> = nessa área você coloca o nome de sua nova Branch(sem as <>)


Comando|Para que serve
|---|---|
`git clone <link do Repo>`| Clona o Repositório Externo em seu computador
`git branch`| Mostra todas as Branchs vinculadas em seu computador, tem um * na sua Branch atual
`git branch -r`| Mostra todas as Branchs que existem do Projeto
`git checkout -b <nome branch>`| Cria uma nova Branch com os mesmos dados da Branch atual
`git add .`|  Adiciona todas as modificações feitas no projeto (Não Recomendado)
`git add *.java`| Adiciona todos os arquivos modificados que possuem extensão .java
`git commit -m "mensagem"`| Coloca uma mensagem no commit das modificações
`git push origin <nome branch>`| Envia externamente a sua Branch desejada
`git pull`| Baixa todas as modificações que estão externas mas não no seu computador 

[Teste de Imagem](teste_imagem.md)