
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

Volta para o commit anterior mas salva as alterações feitas até agora

### Recuperando stash

1) Gerar uma lista de stashes com uma lista de arquivos salvos em stash.

```
git stash list
```

2) Depois de saber qual arquivo você quer recuperar, basta executar

```
git stash <name>
```

### Removendo stash

1) Ver quais a lista de stashes

```
git stash list
```

2) Remover de acordo com a indexação

```
git stash drop 3
```

obs: dificilmente você remove algo, para manter o histórico de criação

### Criando tags

O intuito de criar uma tag é ter controle do projeto para entender o que está ocorrendo com a branch. Marca os estágios de desenvolvimento e é muito utilizado em gerenciamento de projetos.

```
git tag -a <nome> -m "<msg>"
```

obs: tag não é stash
obs: geralmente  a elaboração de tags é bem definida, com o intuito de evitar redundância.



### Alterando tags



