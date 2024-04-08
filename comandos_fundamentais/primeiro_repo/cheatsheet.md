
## Configurações iniciais

Fluxo de processo para a criação do github


```C
git init
git add .
git status
git commit -m "Hello world"
git branch -M master
git remote add origin git@github.com:arielabade/testes-github.git
git push -u origin master
```

```C
git remote rm origin //remover da origem
```

Caso ocorra algum erro com o protocolo SSH, tentar o protocolo https

## Mudanças

U = untracked
M = modified

```C
git status = sets the status
```

## Adição

A = added


``` C
git add path/file
git add . \css\styles.css //também adiciona
git add . 
```

Se você não adicionar um comando, ele não estará no controle de versão.

Então você precisa ir adicionando

## Alterações

O objetivo das alterações é fazer elas com ccommits

Arquivos específicos ou vários de uma vez são utilizados com a flag -a

```C
git commit a.txt -m "Enviando um texto"
git commit -m "Enviando alguns textos"
git commit -a -m "Enviando TODOS os textos "

```

- Enviando código depois do git commit
```C
git push
```
 O push serve para igualar a versão da master com a versão dos outros ramos

"Your master is behind..."
"Your master is ahed..."

## Recebendo Alterações

```C
git pull
```

Usados para sincronizar mudanças locais com mudanças remotas. Busca atualizações, e se encontra elas, une elas com o código atual. (pode ter algum conflito)



## Clonagem


## Remoção


![[17+-+Git+do+básico+ao+avançado (1).pdf]]