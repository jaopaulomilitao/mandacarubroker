# MandaCaru Broker API

## Descrição
A MandaCaru Broker API é uma aplicação Spring Boot desenvolvida para oferecer funcionalidades de gerenciamento de ações (stocks). Ela permite realizar operações básicas de CRUD (Create, Read, Update, Delete) sobre os dados das ações, fornecendo endpoints acessíveis via HTTP.
## Recursos

### Listar Todas as Ações
Este endpoint retorna uma lista de todas as ações disponíveis no sistema.

**Endpoint:**
```http
GET /stocks
```

### Obter uma Ação por ID

Este endpoint retorna os detalhes de uma ação específica com base no seu ID.

**Endpoint:**
```http
GET /stocks/{id}
```

### Criar uma Nova Ação
Este endpoint cria uma nova ação com base nos dados fornecidos no corpo da solicitação.

**Endpoint:**
```http
POST /stocks
```
**Corpo da Solicitação (Request Body):**

```JSON
{
  "symbol": "BBAS3",
  "companyName": "Banco do Brasil SA",
  "price": 56.97
}

```
### Atualizar uma Ação por ID
Este endpoint atualiza os detalhes de uma ação específica com base no seu ID, utilizando os dados fornecidos no corpo da solicitação.

**Endpoint:**
```http
PUT /stocks/{id}
```
**Corpo da Solicitação (Request Body):**

```JSON
{
  "symbol": "BBAS3",
  "companyName": "Banco do Brasil SA",
  "price": 59.97
}

```

### Excluir uma Ação por ID
Este endpoint exclui uma ação específica com base no seu ID.

**Endpoint:**
```http
DELETE /stocks/{id}
```


## Uso
Para começar a usar a MandaCaru Broker API, siga estes passos:

1. Clone o repositório: git clone https://github.com/seu-usuario/MandaCaruBrokerAPI.git
2. Importe o projeto em sua IDE preferida.
3. Configure o banco de dados e as propriedades de aplicação conforme necessário.
4.Execute o aplicativo Spring Boot.
5. Acesse a API em http://localhost:8080.

## Requisitos
Para executar a MandaCaru Broker API, você precisará dos seguintes requisitos:

Java 11 ou superior
Maven
Banco de dados (PostgreSQL recomendado)

## Tecnologias Utilizadas
A MandaCaru Broker API foi desenvolvida utilizando as seguintes tecnologias:

Spring Boot: para criação da aplicação web.
Spring Data JPA: para acesso e manipulação dos dados no banco de dados.
Maven: para gestão de dependências e construção do projeto.
PostgreSQL: como banco de dados relacional.

## Contribuições
Contribuições são bem-vindas! Antes de enviar uma solicitação de pull, por favor, discuta as alterações que você deseja fazer.

## Licença
Este projeto está licenciado sob a [Licença MIT](LICENSE).

## Relatório de Qualidade de Software - Parte 1
Para mais detalhes sobre o funcionamento da API e sua analise estática e dinâmica consulte: [Relatório](https://docs.google.com/document/d/1cSUQFjB8lOhpcq33s7c6t8mIoRofmEQhkZzYjjK7LCM/edit?usp=sharing)


