#### Configurações em geral

Configurações das variaveis que controlam todos os aspectos que o git verifica e opera.
```
$ git config
```
```
$ git help <verbo>
$ git <verbo> -h
```
#### Git Básico

Inicializa o repositorio em um diretorio existente
```
$ cd <dir_path>
$ git init
```
Clonando repositorio existente
```
$ git clone <url> || <newDir>
```
> Precisa de permissão para se clonar um diretorio

Recuperar o ultimo meta-data do repositorio
```
$ git fetch
```
Recuperar o ultimo meta-data do repositorio e da merge com o diretorio local
```
$ git pull
```
Verificando o status de seus arquivos
```
$ git status || -s
```
Tracking/Commiting novos arquvos
```
$ git add <file> || *
$ git commit
$ git commit -m "Descrição do commit"
$ git commit -a > Pula a etapa de Staging
```
> Para se ignorar arquivos e extensões deve se criar um arquivo .gitignore

Unmodifying o arquivo 
```
$ git checkout --<file> 
```
> Este comando é perigoso pq qualquer alteração local é desfeita*

Unstaging o arquivo
```
$ git reset HEAD <file>
```
Refazer o ultimo commit
```
$ git commit -- amend
```
Removendo os arquivos na Staged area
```
$ git rm <file>
```
Movendo/Renomenando arquivos
```
$ git mv <file_from> <file_to>
```
Diferença entre versões
Compara Staged e Unstaged
```
$ git diff
```
Compara Staged e Commit
```
$ git diff --staged (ou --cached)
```
Logs de commit
```
$ git log
```
> O git log tem diversas opções(-) para disponolizar os dados

Verificar a branch do URL do repositorio
```
$ git branch
```
Adiciona branch ao repositorio
```
$ git branch <newBranch>
```
alterar branch ao repositorio
```
$ git checkout <newBranch>
```
Fazer o merge entre dois branchs
```
$ git merge <newBranch>
```
Remover a branch do repositorio
Delete branch locally
```
$ git branch -d localBranchName
```
Delete branch remotely
```
$ git push origin --delete remoteBranchName
```
Verificar a origem do URL do repositorio
```
$ git remote -v
```
Remover a origem do repositorio
```
`$ git remote remove origin`
```
Adiciona outro repositorio
```
$ git remote add <Shortname> <URL>
```
> Você pode adicionar mais de uma origem 

Referenciar repositorio
```
$ git fetch <Shortname>
$ git push <Shortname> <Branch>
```
Verificar repositorio
```
$ git remote show <Shortname>
```
> Mostra o status dos repositorios 

Renomear repositorio
```
$ git remote rename <Name> <newName>
```

