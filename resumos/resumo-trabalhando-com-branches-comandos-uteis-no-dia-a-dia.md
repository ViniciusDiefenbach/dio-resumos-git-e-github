# Trabalhando com Branches - Comandos Úteis no Dia a Dia

Anteriormente, vimos que é possível utilizar o comando git pull para baixar as atualizações do repositório remoto e resolver conflitos. Porém, ao utilizar branches, você também pode apenas baixar as atualizações de uma branch com o seguinte comando...

```git fetch <remote-name> <branch-name>```

Caso queira verificar as diferenças de determinada branch com outra, você pode utilizar o comando abaixo...

```git diff <name-branch-1> <name-branch-2>```

Uma vez que você notou as diferenças, você pode realizar as junção/mescla das branches se desejar com o comando...

```git merge <name-branch>```

## Notas
*Nota1: O comando git pull faz todo esse processo por debaixo dos panos também, porém é interessante saber esse processo para alterações mais minuciosas*

*Nota2: Caso a branch esteja disponível no repositório local, você pode utilizar somente o nome de branch. Caso a branch esteja disponível somente no repositório remoto, você pode identifica-la da seguinte maneira: \<name-remote>/\<name-branch>*

*Nota3: você também pode clonar o repositório de uma branch específica com o comando... ```git clone <path> --branch <name-branch> <--single-branch>```*

*Nota4: você pode utilizar do comando ```git stash``` para arquivar arquivos staged (pode ser muito útil para criação de branches). Uma vez que você precisa trabalhar com as informações arquivadas, você pode utilizar o comando ```git stash apply``` para voltar as alterações arquivadas ou ```git stash pop``` para remover as alterações arquivadas*

[Clique Aqui para Voltar](/README.md)