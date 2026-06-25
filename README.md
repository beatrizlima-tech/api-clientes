# 👥 API Clientes

![Java](https://img.shields.io/badge/Java-21-red?style=for-the-badge\&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.x-green?style=for-the-badge\&logo=springboot)
![Build](https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge\&logo=postgresql)
![Swagger](https://img.shields.io/badge/Swagger-OpenAPI-85EA2D?style=for-the-badge\&logo=swagger)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=for-the-badge)

---

# 📌 Sobre o projeto

A API Clientes é uma aplicação backend desenvolvida com **Java** e **Spring Boot** para gerenciamento de clientes, oferecendo operações de cadastro, consulta, atualização e exclusão lógica de registros.

O projeto foi desenvolvido com foco na construção de APIs REST, integração com banco de dados PostgreSQL utilizando JDBC, organização em camadas e documentação utilizando Swagger/OpenAPI.

---

# 🚀 Funcionalidades

* ✅ Cadastro de clientes
* ✅ Atualização de clientes
* ✅ Exclusão lógica de clientes
* ✅ Consulta de clientes por nome
* ✅ Integração com PostgreSQL
* ✅ Documentação da API com Swagger/OpenAPI
* ✅ Configuração de CORS para integração com aplicações frontend

---

# 🧱 Tecnologias Utilizadas

* Java 21
* Spring Boot
* Spring Web MVC
* JDBC
* PostgreSQL
* Swagger / OpenAPI
* Maven
* REST API

---

# 🏗️ Estrutura do Projeto

```text
src/main/java/br/com/cotiinformatica/api_clientes/

├── configurations
├── controllers
├── dtos
├── entities
├── factories
└── repositories
```

---

# 🔗 Endpoints da API

## Clientes

| Método | Endpoint                  | Descrição                 |
| ------ | ------------------------- | ------------------------- |
| POST   | `/api/v1/clientes`        | Cadastrar cliente         |
| PUT    | `/api/v1/clientes/{id}`   | Atualizar cliente         |
| DELETE | `/api/v1/clientes/{id}`   | Realizar exclusão lógica  |
| GET    | `/api/v1/clientes/{nome}` | Buscar clientes pelo nome |

---

# ⚙️ Como Executar o Projeto

## 1. Clonar o repositório

```bash
git clone https://github.com/beatrizlima-tech/api-clientes.git
```

---

## 2. Criar o banco de dados

```sql
CREATE DATABASE clientesdb;
```

Execute também o script de criação da tabela disponível no projeto.

---

## 3. Configurar o arquivo `application.properties`

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/clientesdb
spring.datasource.username=postgres
spring.datasource.password=postgres
```

---

## 4. Executar a aplicação

```bash
mvn spring-boot:run
```

---

## 5. Acessar a documentação

```text
http://localhost:8080/swagger-ui.html
```

---

# 📊 Arquitetura

```text
Cliente (Frontend)
        │
        ▼
Controller
        │
        ▼
Repository
        │
        ▼
JDBC
        │
        ▼
PostgreSQL
```

---

# 📌 Melhorias Futuras

* [ ] Migrar JDBC para Spring Data JPA
* [ ] Implementar autenticação com JWT
* [ ] Adicionar Bean Validation
* [ ] Criar testes automatizados
* [ ] Dockerizar a aplicação
* [ ] Padronizar respostas HTTP da API
* [ ] Implementar tratamento global de exceções

---

# 👩‍💻 Autora

**Beatriz Lima de Oliveira**

🔗 GitHub:
https://github.com/beatrizlima-tech
