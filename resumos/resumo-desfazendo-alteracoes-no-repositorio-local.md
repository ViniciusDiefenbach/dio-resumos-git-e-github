# Desfazendo Alterações no Repositório Local

Para corrigir um repositório git inicializado incorretamente, basta utilizar o comando:

```rm -rf .git```

*Por baixo dos panos este comando exclui a pasta oculta .git criada a partir da inicialização do repositório.*

**Descartar Mudanças Não-Commitadas:** digamos que eu tenha alterado um arquivo e desejo voltar a sua versão do commit (antes de minha alteração). Para tal, posso utilizar o comando:

 ```git restore <arquivo || .>```.

**Ajustar o Nome do Último Commit (Amend):** para ajustar o nome do último commit, podemos utilizar o seguinte comando ```git commit --amend <-m "Message">```.

**Desfazer determinado Commit:** primeiro passo, ```git log```. Este comando mostrará todos os commits realizados. Uma vez que você encontrou o commit que deseja voltar, copie seu identificador e utilize o comando ```git reset \<id-commit> <--soft || --hard || --mixed (default)>```.

*--soft*: Desfará todos os commits realizados até o id \<id-commit> e as alterações estarão com o status "staged" (prontas para a realização de um novo commit);

*--mixed*: Desfará todos os commits realizados até o id \<id-commit> e as alterações estarão com o status "unstaged" (untracked ou modified);

*--hard*: Desfará todos os alterações e commits realizados até o id \<id-commit> (as alterações não ficarão salvas e serão excluídas);

**Lista detalhada dos commits, resets, ammends, ...:** para tal, utilize o comando ```git reflog```. Ele mostra os registros não apenas dos commits mas também de outras ações que necessitam deste histórico.

**Preparei um arquivo para commit indesejadamente:** para remover arquivos staged e torna-los untracked ou modified, devo utilizar o comando ```git restore --staged <arquivo || .>``` (ao fazer isso, as alterações não são excluídas).

## Notas
*Nota1: O comando ```git reset``` também pode ser utilizado para arquivos (removendo alterações staged, modified ou untracked - estas são simplesmente apagadas, não fica nenhum registro) -> ```git reset <arquivo || .>```*

[Clique Aqui para Voltar](/README.md)