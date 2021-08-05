#### Configurações em geral

$ git config

* Configurações das variaveis que controlam todos os aspectos que o git verifica e opera.

$ git help <verbo>
$ git <verbo> -h

#### Git Básico

Inicializa o repositorio em um diretorio existente

$ cd <dir_path>
$ git init

Clonando repositorio existente

$ git clone <url> || <newDir>

* Precisa de permissão para se clonar um diretorio

Verificando o status de seus arquivos

$ git status || -s

Tracking/Commiting novos arquvos

$ git add <file> || *
$ git commit
$ git commit -m "Descrição do commit"
$ git commit -a > Pula a etapa de Staging

Unmodifying o arquivo 

$ git checkout --<file> *Este comando é perigoso pq qualquer alteração local é desfeita*

Unstaging o arquivo

$ git reset HEAD <file>

Refazer o ultimo commit

$ git commit -- amend

* Para se ignorar arquivos e extensões deve se criar um arquivo .gitignore

Removendo os arquivos na Staged area

$ git rm <file>

Movendo/Renomenando arquivos

$ git mv file_from file_to

Diferença entre versões

$ git diff > Compara Staged e Unstaged
$ git diff --staged (ou --cached) > Compara Staged e Commit

Logs de commit

$ git log

* O git log tem diversas opções(-) para disponolizar os dados