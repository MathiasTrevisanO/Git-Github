GIT

Entrar na pasta que vai ser trabalhada e usar o comando git init para criar a pasta git;
comando git status para verificar se foi feito algum commit
Se editar o arquivo, o arquivo é Untracked;
Se fizer o comando git add nome_arquivo e der um git status, o arquivo vira um Staged, ou seja, o arquivo está preparado para commitar.
Para commitar é so digitar o comando git commit -m "nome_da_mensagem", onde deve a mensagem deve ser dita o que foi alterado no codigo.
Antes de commitar, utilizar o comando git diff para verificar o que foi modificado.
git checkout nome_arquivo faz com que todas modificações do arquivo sejam apagadas.
Para tirar todo o arquivo commitado utiliza-se o comando git reset --mixed hash (a hash é obtida pelo git log).

GITHUB

CRIAR REPOSITORIO

git init na pasta para mandar os arquivos pro github;
se nao tiver feito um git add, fazer este passo do git;
fazer o commit;
utilizar o comando git remote add origin chave_do_repositorio_GITHUB (pegar a chave gerada no github);
git push -u origin master envia o arquivo pro github.

MODIFICAÇOES NO GITHUB

com as modificações feitas no arquivo, fazer um commit sendo git commit -am "nome_da_mensagem"
git push origin master (master é o branch)

CLONAR

g clone chave_repositorio_github nome_arquivo

FORK - faz uma copia do projeto da pessoa e pode mandar as modificações pro dono do projeto. Diferente do clone, onde são repositorios que eu criei.

BRANCH

git checkout -b nome_do_branch  esse comando cria um branch
git checkout master altera o branch para master
git branch -D nome_do_branch apaga o branch

MERGE

com varios branchs criados, o merge faz com que apareça todos os commits realizados. O comando para dar o merge aparecer todos os commits no git log é git merge nome_branch, onde ele vai mesclar o commit feito separado e junta com a branch master

REBASE

git rebase nome_branch - faz com que o commit da branch vá para o topo da lista de logs na branch master
