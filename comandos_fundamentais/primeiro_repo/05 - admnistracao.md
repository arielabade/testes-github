
O objetivo dessa sessão é admnistrar o repositório do github para que seja mais fácil gerenciar ele, e também para que ele fique mais leve.

## Limpar arquivos untracked

Para limpar arquivos que não estão sendo trackeados:

```
git clean
```

OBS: arquivos não traqueados ocorrem quando você não usou o git add . ou foram arquivos que naturalmente não subiram pro github.

Cuidado para não excluir nenhum arquivo que estava no stashing e era pra você adicionar.

## Limpar arquivos desnecessários identificados pelo git

```
git gc
```

Melhora o uso da memória por que exclui os arquivos que o git julga não serem mais necessários.

Muito utilizado para melhorar a performance com relação a arquivos mais antigos, para deixar as operações do git mais leves

## Checando integridade de arquivos

Verifica a integridade de arquivos e sua conectividade

```
git fsck
```

Verifica possíveis corrupções em arquivos, código inconsistente, etc.

## Checando os logs de referência

É uma versão do gggit log, só que mais completa.

```
git reflog
```

Checa até as mudanças de branches. Diferente do git log, que apenas armazena os commits de uma branch.

O tempo de duração de expiração padrão de um reflog é de 30 dias, mas isso é configurável.

## Comprimindo repositório

Transformando o repo para arquivo

```
git archive --format zip --output files.zip
```

Assim o arquivo files esterá em formato zip.

Isso é interessante quando você precisa das coisas com urgência.




