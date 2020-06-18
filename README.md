# Desafio 1

### 🚀Sobre o desafio🚀
Neste desafio eu tenho que botar em prática o que aprendi no primeiro módulo do curso GoStack 11 da rocketseat

#### O que deveria ser feito?
Neste desafio a rocketseat criou um template de projeto com 5 rotas, sendo elas:

POST /repositories : Para adicionar repositórios no formato
```
    {
        "title": "Desafio 1",
        "url": "https://medium.com/@raullesteves/github-como-fazer-um-readme-md-bonit%C3%A3o-c85c8f154f8",
        "techs": ["Node.JS", "React"]
    }
```
GET /repositories : Onde retorna todos os repositórios
DELETE /repositories/:id : Para deletar um repositório
PUT /repositories/:id : Atualizar algum repositório
POST /repositories/:id/like: Para dar like em algum repositório

### Atingindo o sucesso do desafio.
Para o sucesso do desafio, deveria passar em todos os testes descritos pela Rocketseat.

#### Testes

Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.

Caso você tenha dúvidas quanto ao que são os testes, e como interpretá-los, dé uma olhada em nosso FAQ.

Para esse desafio temos os seguintes testes:

```should be able to create a new repository:``` Para que esse teste passe, sua aplicação deve permitir que um repositório seja criado, e retorne um json com o projeto criado.

```should be able to list the repositories:``` Para que esse teste passe, sua aplicação deve permitir que seja retornado um array com todos os repositórios que foram criados até o momento.

```should be able to update repository:``` Para que esse teste passe, sua aplicação deve permitir que sejam alterados apenas os campos url, title e techs.

```should not be able to update a repository that does not exist:``` Para que esse teste passe, você deve validar na sua rota de update se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.

```should not be able to update repository likes manually:``` Para que esse teste passe, você não deve permitir que sua rota de update altere diretamente os likes desse repositório, mantendo o mesmo número de likes que o repositório já possuia antes da atualização. Isso porque o único lugar que deve atualizar essa informação é a rota responsável por aumentar o número de likes.

```should be able to delete the repository:``` Para que esse teste passe, você deve permitir que a sua rota de delete exclua um projeto, e ao fazer a exclusão, ele retorne uma resposta vazia, com status 204.

```should not be able to delete a repository that does not exist:``` Para que esse teste passe, você deve validar na sua rota de delete se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.

```should be able to give a like to the repository:``` Para que esse teste passe, sua aplicação deve permitir que um repositório com o id informado possa receber likes. O valor de likes deve ser incrementado em 1 a cada requisição, e como resultado, retornar um json contendo o repositório com o número de likes atualizado.

```should not be able to like a repository that does not exist:``` Para que esse teste passe, você deve validar na sua rota de like se o id do repositório enviado pela url existe ou não. Caso não exista, retornar um erro com status 400.


