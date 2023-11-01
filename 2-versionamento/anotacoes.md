# Versionamento de codigo

## Visão Geral

### O que é versionamento de codigo

  O versionamento de codigo nos ajuda a manter o codigo coerente e permite que equipes tenham acesso a alterações que foram feitas por colegas, assim permitindo que não haja discrepancia entre os codigos de desenvolvedores diferente ou equipes diferentes, alem de preservar ve rsões antigas do codigo, permitindo retornar a uma versão anterior se algo acontecer.

### O que é git

  O Git é uma ferramenta de versionamento de codigo amplamente utiliza pelos desenvolvedores

### O que é github

  O Github é uma plataforma para hospedagem de codigo no qual podemos utiliza-lo para armazenar nosso codigo fonte e seu historico de versao, tambem é um local que proporciona um ambiente colaborativo,
  possibilitando desenvolvedores a ajudar em projetos de terceiros.

## Configuração

- git config --global user.name "Paulo"
- git config user.name -> mostra o nome configurado
- git config --global init.defaultBranch main
- git config --global --list
- git config --global credential.helper (store OU cache)
- git config --global --show-origin credential.helper
- ssh-keygen -t ed25519 -C "<paulolds086543@gmail.com>"

## Primeiros passos

### Criando e Clonando

- git clone <git@github.com>:PaulCod/hello-world-dio.git repo-clonado -> muda o nome do repositorio
- git remote -v -> Mostra os repositorios vinculados
- git remote add origin <https://github.com/PaulCod/repo-remoto.git>
- git clone URL --branch feature1 --single-branch
- git push origin main

### Salvando alterações no repositorio Local

- git status
- git log
- git add .
- git commit -m "Hello World"
- .gitkeep -> para manter pasta vazia

## Desfazendo alterações no repositorio local

- git restore <File name>
- git --amend -m "Hello World"
- git commit --amend
- git reset (--hard ou --soft ou --mixed)
- git reflog

## Enviando e baixando alteração para o remoto

- git pull

## Trabalhando com Branchs

- git checkout -b teste
- git checkout main
- git branch -v
- git branch
- git branch -d teste

- git fetch origin main
- git diff main origin/main
- git merge origin/main

- git clone URL --branch teste --single-branch
- git stash     (pop apply)
