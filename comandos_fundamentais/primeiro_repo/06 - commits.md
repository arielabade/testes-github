## Por que commitar certo?

Quando o commit não é objetivo com relação as atualizações que ele propõe, e quando ele não é intuitivo com relação ao que ele foi entregue, ele é um commit ruim.

##### Vantagens:

- Facilita revisões futuras
- Padroniza o crescimento do projejto
- Faacilitar manutenção no futuro
- Melhora os logs
- Melhore a ccorreção de bugs

##### Boas práticas

- Padronizar os commits
- Não realize commits separados que poderiam ser um commit só
- 


##### Private branches

1) Clonar a master normalmente com git clone
2) A partir do clone da master fazer outro clone
3) Esse clone será chamado de private branch
4) A private branch conterá o desenvolvimento da funcionalidade e todos os commits realizados
5) Depois que a funcionalidade for resolvida, você transfere todo o código da private branch para a branch clonada inicial.

Para isso, vai precisar:

```
git rebase private_branch branch_destino
```

- O rebase vai mostrar todos os commits e substituir o "pick" por "squash".
- Se você substituir o "pick" por "reword" você muda o nome do commit, isso é importante para salvar um ponto no projeto.

Apertando ```x!``` O commit é salvo no rebase

E a partiir disso você pode adicionar novos comentários nos seus commits



Leve apenas os commits que vão ser importante para revisão

- Dar git checkout na branch que você deseja subir as alterações da funcionalidade

Crie uma branch privada para o seu trabalho pessoal, que não será compartilhada no repositório final
