# Desafio 4 - Git

**Imagine o seguinte cenário:**

Em um projeto realizado em sua equipe, você precisa realizar uma alteração em seu script.

Esse ajuste trata-se da inclusão de um campo adicional na dim_product. Estre projeto já está em Produção na e versionado na Branch Master do GitHub.

Quais seriam os comandos e cuidados necessários desde a criação de sua Branch até o Pull Request.

## Entrega do código

### 1. Atualização Local:

Primeiramente, devo me certificar de que a cópia local do repositório está atualizada com a brach do GitHub.

```bash
git checkout master
git pull origin master
```

Isso garante que estou trabalhando com a versão mais recente do código que está em produção.

### 2. Criação de uma Nova Branch:

Criação de uma nova branch a partir da master para realizar as alterações (com um nome que faça sentido com o que será feito no código).

```bash
git checkout -b feature/additional-dim-product-field
```

### 3. Implementação das Alterações:

Realizações  das modificações necessárias no script para incluir o campo adicional na dim_product.

### 4. Commit e Push das Alterações:

Após a implementação, adicionarei as modificações, farei commit das mudanças com um texto exmplicativo e um push na branch nova do GitHub.

```bash
git add .
git commit -m "Adiciona campo adicional na dim_product"
git push origin feature/additional-dim-product-field
```

### 5. Abertura de um Pull Request:

Abertura de um novo Pull Request comparando a branch feature/additional-dim-product-field com a branch master.

Descrição das alterações realizadas e marcação dos revisores apropriados para revisar o código.

## Pós entrega do código

### 6. Revisão e Integração:

Os revisores irão analisar as alterações no Pull Request.

### 7. Merge do Pull Request:

Com as alterações aprovadas, será feito o merge do Pull Request na branch master.

### 8. Atualização do Ambiente de Produção:

Após o merge, as alterações estão na branch master. Dessa forma, será necessário um novo processo para atualização do ambiente de produção com os dados atualizados do GitHub, como por CI/CD ou ação da pessoa/equipe responsável pela operação.