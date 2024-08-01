# Trabalhando com Branches - Criando, Mesclando, Deletando e Tratando Conflitos

Em resumo, uma branch é uma ramificação (tradução literal) de seu repositório. Ela serve para testar uma funcionalidade incerta de seu código por exemplo. É como se fosse criado uma outra linha do tempo para seu repositório. Por padrão, a branch criada aponta para o commit atual (mantendo as alterações realizada até o momento da criação da branch). Segue uma imagem que ilustra esse pensamento:

![Ilustração Branches](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

**Criação de uma branch:** para tal, utilize o seguinte comando...

```git checkout -b <name-branch>```

**Trocar de branch:** para tal, utilize o seguinte comando...

```git checkout <name-branch>```

**Verificar branches e indexes de cada branch:** para tal, utilize o seguinte comando...

```git branch <-v>```

**Remover uma branch:** para tal, utilize o seguinte comando...

```git branch -d <name-branch>```

[Clique Aqui para Voltar](/README.md)