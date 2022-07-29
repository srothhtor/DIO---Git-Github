### Comandos básicos ###



*  Se você precisar de ajuda ao usar Git, existem três maneiras de obter a ajuda para qualquer um dos comandos Git: 
  * git help {comando}
    git {comando} --help
    man git- {comando}	

* Caso você esteja iniciando o monitoramento de um projeto existente com Git, você precisa ir para o diretório do projeto e digitar

  * git init

* Você clona um repositório com **git clone [url]**. Por exemplo, caso você queria clonar a biblioteca Git do Ruby chamada Grit, você pode fazê-lo da seguinte forma:

  * git clone

* Para passar a monitorar um novo arquivo, use o comando **git add**. Para monitorar o arquivo **README**, você pode rodar isso:

  * 'git add README'

* A principal ferramenta utilizada para determinar quais arquivos estão em quais estados é o comando:

  * git status

* Se o comando **git status** for muito vago — você quer saber exatamente o que você alterou, não apenas quais arquivos foram alterados — você pode utilizar o comando.

  * git diff

* Armazena o conteúdo atual do índice em um novo commit, juntamente com uma mensagem de registro do usuário que descreve as mudanças.

  - Se usa o commit depois de já ter feito o **git add**, para fazer o commit:
      - git commit -m "Mensagem 

  - Para commitar também os arquivos versionados mesmo não estando no Stage basta adicionar o parâmetro -a
    - git commit **-a** -m "Mensagem

  - Refazendo commit quando esquecer de adicionar um arquivo no Stage:
    - git commit -m "Mensagem" **--amend**

* Para remover um arquivo do Git, você tem que removê-lo dos arquivos que estão sendo monitorados (mais precisamente, removê-lo da sua área de seleção) e então fazer o commit. O comando **git rm** faz isso e também remove o arquivo do seu diretório para você não ver ele como arquivo não monitorado (untracked file) na próxima vez.

  * git rm -f {arquivo}

* Diferente de muitos sistemas VCS, o Git não monitora explicitamente arquivos movidos.
  É um pouco confuso que o Git tenha um comando **mv**. Se você quiser renomear um arquivo no Git, você pode fazer isso com

  * git mv arquivo_origem arquivo_destino
