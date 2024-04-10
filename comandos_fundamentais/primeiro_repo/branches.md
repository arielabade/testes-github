
Branch é a forma do git que separa as versões dos projetos.

Quando um projeto é criado, ele iinicia na branch master, mas cada nova feature do projetto fica em um branch separado. É uma boa prática que cada desenvolvedor seja responsável por uma parte do projetot afim de evitar conflitos enttre branches.

Após a finalização do projetot da branch, elas são unidas, com intuito de entregar o código fonte final.

### Criando e visualizando branches

Criar uma branch é muito utilizada no dia a dia, por que quando você vai desenvolver uma funcionalidade, uma branch nova precisa ser criada

```
git branch first_branch
git branch second_branch
```

Quando você inicializa a branch, a branch é igual ao master

### Deletar branches

```
git branch -d second_branch
```

Não é comum deletar branches, mas é uma boa práttica manter o histórico.

### Mudar o branch

Transitar entre branches

```
git checkout master
```

Esse comando muda a branch para a master, mas é necessário ter cuidado ao utilizar ele, pois ele carrega todas as alterações da branch anterior para a branch alvo.

Salve todas as alterações necessárias antes de mudar de branch.

### Unindo branches

Unir uma branch com a branch de outro desenvolvedor ou com a master

1) Escolha a branch de destino

```
gitt checkout master
```

2) Escolha a branch que você deseja unir

```
git merge first_branch
```

3) Caso existam conflittos, resolva

### Stash

Prosseguir com outra solução, mas não perder o código que fez atté agora.

```
git stash
```

Voltta para o commit anterior mas salva as alterações feitas até agora

### Recuperando stash


### Removendo stash


### Criando tags

### Alterando tags



