- **Atualizar as dependências do package.json**
`npm i -g npm-check-updates`

 - (Branch) **_basicamente existe a branch principal (ramo principal) e os ramos secundários_**
**Criar uma branch secundária**
`git checkout -b namebranch`

- **Clonar uma branch secundária**
`git clone -branch namebranch git://remoterepository.git`
`git checkout -b namebranch`

- **Alternar o apontamento no grafo (na árvore)**
`git checkout master (aponta para o branch master) `
`git checkout namebranch (aponta para o branch secundárior) `

- **Apontamento para os ramos**
Para tornar o seu ramo secudário (branch secundária) o ramo master, basta, primeiramente,
apontar para o **ramo master** utilizando o comando `git checkout master` , em seguida, deve-se explicitar qual dos **ramos secundários** será a sua nova branch master, utilizando o MERGE ->  `git merge origin/ramosecundario` . 

- **Deletar um branch remoto (um branch que está no github, por exemplo)**
`git push origin --delete branch`

- **Deletar um branch local**
`git branch -d nome_do_branch` -> **`-d`** exclui apenas se vc já fez o `merge` ou o `push` do projeto 
`git branch -D nome_do_branch` -> **`-D`** exclui o branch independente de seu status de `push` ou `merge`, então (**CAUTION**), 
