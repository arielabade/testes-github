## Encontrando branches

O git pode estar não mapeando suas branches. Com o comando git fetch, você é atualiziado de todos os branches e tags que não estão reconhecidos por você.

É útil para utilizar a branch de outra pessoa do mesmo time.

```
git fetch -a
git checkout funcionalidiade_x
git branch
```

O fetch é utilizado para reconheccer novas branches

## Recebendo atualizações

Quando existem novas informações da branch, o conteúdo delaa deve atualizado com

```
git pull
```

É interessante utiliizar git pull periodicamente para evitar conflitos.

É interessante para pegar o conteúdo interno da branch que recebeu o fetch.


## Veiculação de repositórios

Rastrear ou remover repositórios, de acordo coom a necessidade.

Esse comando mostra aonde o repositório está alocado:
```
git remote -v
```

Esse comando conecta a um repositório remoto:
```
git remote add origin <linK>
```

Esse comando desconecta de um repositório remoto:

```
git remote rm origin
```

## Submodules

Ter dois ou mais projetos em um repositório só.

É possível adicionar uma dependência ao projeto atual, mantendo suas estrutura separadas.

É bom utilizar esse comando para criar dependências específicas do projeto.

```
git submodule add <repo>
```

Para listar todos os submodulos

```
git submodule
```

Para atualizar o submodulo:

```
git push ---recurse-subomoddules=on-demand
```
