# Salvando Alterações no Repositório Local

Antes de conhecer os comandos, é importante entender os estágios dos arquivos até chegar o momento de gravar as alterações e subir a um repositório... Leve em consideração a imagem abaixo:

![Etapas: Untracked, unmodified, modified, staged](https://i.sstatic.net/QaeAZ.png)

**Untracked**: arquivos que ainda não foram adicionados ao repositório git;

**Unmodified**: arquivos que foram adicionados, porém não tiveram nenhuma alteração desde o último commit;

**Modified**: arquivos que foram modificados desde o último commit;

**Staged**: arquivos que sofreram alguma alteração e foram adicionados ao git para serem "commitados";

Uma vez que temos um arquivos adicionado ao código fonte (untracked) ou algum arquivo modificado desde o último commit (modified), podemos utilizar o comando ```git add <arquivo || .>``` para preparar a alteração para o Commit (tornando o status do arquivo como staged).

Uma vez que temos arquivos com o status staged, podemos realizar o commit com o seguinte comando ```git commit <-m "Message">```. Esse comando gravará as alterações e tornará os status dos arquivos staged em unmodified.

## Notas
*Nota1: O "." após o "add" adicionará todos os arquivos novos ou modificados*

*Nota2: Para preparar pastas vazias para o commit, você pode criar um arquivo chamado ".gitkeep" dentro da pasta, a fim de armazena-la em seu repositório mesmo sem possuir arquivos*

*Nota3: Para não incluir e evitar o rastreio de determinados arquivos por parte do Git, podemos utilizar o arquivo ".gitignore". Este serve justamente para previnir o Git de adicionar arquivos indesejados ao repositório*

[Clique Aqui para Voltar](/README.md)