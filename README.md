# API Restful Products

Esta é uma API Restful CRUD de gerenciamento de produtos, representando meu primeiro contato com Spring Boot. O projeto foi feito juntamente ao vídeo "[Spring boot 3 | Curso Completo](https://www.youtube.com/watch?v=wlYvA2b1BWI&ab_channel=MichelliBrito)" da Michelli Brito, que serviu como uma base de estudo e prática para desenvolvimento de APIs.

## Pré-requisitos

- [Java](https://www.oracle.com/java/technologies/javase-downloads.html) instalado
- [MySQL Workbench](https://www.mysql.com/products/workbench/) instalado e configurado

## Configuração do Banco de Dados

1. Crie um banco de dados MySQL para o projeto.
2. Atualize as configurações do banco de dados no arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/seu_banco_de_dados
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

## Executando o Projeto

1. Clone o repositório:

```bash
git clone https://github.com/renebttg/api-products.git
cd api-products
```

2. Execute o Maven Wrapper para iniciar a aplicação:

```bash
./mvnw.cmd clean spring-boot:run
```

## Rotas da API

- **GET /products**: Retorna todos os produtos.
- **GET ONE /products/{id}**: Retorna um produto específico por ID.
- **POST /products**: Adiciona um novo produto.
- **PUT /products/{id}**: Atualiza um produto existente por ID.
- **DELETE /products/{id}**: Deleta um produto existente por ID.

## Exemplo de Requisição

Adicione um novo produto:

```bash
curl -X POST -H "Content-Type: application/json" -d "{\"name\": \"Nome do Produto\", \"value\": 9999.00}" http://localhost:8080/products
```

## Contribuindo

Sinta-se à vontade para contribuir! Abra uma [issue](https://github.com/renebttg/api-products/issues) ou envie um pull request.

## Licença

Este projeto é licenciado sob a [Apache License (ASF)](https://www.apache.org/licenses/LICENSE-2.0).


