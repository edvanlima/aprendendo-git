aprendendo-git
==============

```bash
# criação da chave de segurança
ssh-keygen -t rsa -C "seu_email@provedor.com"

# criando um diretório
mkdir aprendendo-git
cd aprendendo-git

# transformar o diretório atual em um repositório do Git
git init

# vericando quais os arquivos que pertencem ao nosso repositório
git ls-files

# vericando o estado dos arquivos do nosso projeto
git status

# adicionando o arquivo index.html ao repositório
git add index.html

# informando ao Git o nosso nome e e-mail
git config user.name "[nome]"
git config user.email "[email]]"

# denir um nome de usuário e e-mail para todo o sistema
git config --global user.name "[nome]"
git config --global user.email "[email]"

# a executando o nosso primeiro commit do projeto
git commit -m "Início do projeto"

```

Congurando o repositório remoto
-------------------------------

Congurar sincronização com o repositório local

```bash
git remote add origin https://github.com/[nome]/aprendendo-git.git


git remote -v 


origin https://github.com/[seu_usuario_no_github]/curso-git.git (fetch)
origin https://github.com/[seu_usuario_no_github]/curso-git.git (push)


Fazendo o primeiro push


git push origin master
```


Trabalhando com branches:
-------------------------
```bash
git branch

* master


git branch aprendendo
git branch


  aprendendo
* master


git checkout aprendendo
git branch

* aprendendo
  mast


git log

commit 8b9e4267b379248d933d2270fbff8d69feb439e9 (HEAD -> aprendendo, origin/master, master)
Author: [nome] <[email]>
Date:   Thu Sep 21 11:58:26 2017 -0300

    mensagem teste

commit ceb681eff6ea29324726522d1196ecd1325034db
Author: [nome] <[email]>
Date:   Thu Sep 21 11:22:02 2017 -0300

    aprendendo-git

git add README.md
git commit -m "adicionado uma branch"
git push -u origin aprendendo



# mostrar branch remota
git branch -r

# atualizer o repositorio local
git pull

# criando branch local outro usuario e dizendo a branch remota correspondente
git branch -t aprendendo origin/aprendendo

git merge aprendendo

# atualizando repositorio remoto
git push origin master
```

