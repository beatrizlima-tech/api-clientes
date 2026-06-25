# 👥 API Clientes

![Java](https://img.shields.io/badge/Java-21-red?style=for-the-badge\&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.x-green?style=for-the-badge\&logo=springboot)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge\&logo=postgresql)
![Swagger](https://img.shields.io/badge/Swagger-OpenAPI-85EA2D?style=for-the-badge\&logo=swagger)
![Build](https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=for-the-badge)

---

# 📌 Sobre o projeto

A **API Clientes** é uma aplicação backend desenvolvida com **Java** e **Spring Boot** para gerenciamento de clientes, oferecendo operações completas de cadastro, consulta, atualização e exclusão lógica de registros.

O projeto foi desenvolvido com foco na construção de APIs REST, integração com banco de dados PostgreSQL utilizando JDBC, organização em camadas, documentação com Swagger/OpenAPI e comunicação com aplicações frontend.

---

# 🚀 Funcionalidades

* Cadastro de clientes
* Atualização de clientes
* Exclusão lógica de clientes
* Consulta de clientes por nome
* Integração com PostgreSQL
* Documentação da API com Swagger/OpenAPI
* Configuração de CORS para integração com aplicações frontend

---

# 🧱 Tecnologias utilizadas

* Java 21
* Spring Boot
* Spring Web MVC
* JDBC
* PostgreSQL
* Swagger / OpenAPI
* Maven
* REST API

---

# 🏗️ Estrutura do projeto

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

| Método | Endpoint                  | Descrição                 |
| ------ | ------------------------- | ------------------------- |
| POST   | `/api/v1/clientes`        | Cadastrar cliente         |
| PUT    | `/api/v1/clientes/{id}`   | Atualizar cliente         |
| DELETE | `/api/v1/clientes/{id}`   | Exclusão lógica           |
| GET    | `/api/v1/clientes/{nome}` | Buscar clientes pelo nome |

---

# 📷 Interface

Esta API possui uma aplicação frontend desenvolvida em Angular para consumo dos serviços.

**Frontend:**

👉 https://github.com/beatrizlima-tech/web-clientes

> Em breve serão adicionadas capturas de tela demonstrando a integração entre frontend e backend.

---

# ⚙️ Como executar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/beatrizlima-tech/api-clientes.git
```

### 2. Crie o banco de dados

```sql
CREATE DATABASE clientesdb;
```

Execute também o script SQL disponível no projeto para criação da tabela.

### 3. Configure o arquivo `application.properties`

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/clientesdb
spring.datasource.username=postgres
spring.datasource.password=postgres
```

### 4. Execute a aplicação

```bash
mvn spring-boot:run
```

A API ficará disponível na porta configurada da aplicação.

---

# 📚 Documentação

Após iniciar a aplicação, acesse:

```text
http://localhost:8080/swagger-ui.html
```

---

# 📊 Arquitetura

```text
Frontend Angular
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

# 📌 Melhorias futuras

* Migrar JDBC para Spring Data JPA
* Implementar autenticação JWT
* Adicionar Bean Validation
* Criar testes automatizados
* Dockerizar a aplicação
* Padronizar respostas HTTP
* Implementar tratamento global de exceções

---

# 👩‍💻 Autora

Desenvolvido por **Beatriz Lima**

🔗 GitHub
https://github.com/beatrizlima-tech

💼 LinkedIn
https://www.linkedin.com/in/beatrizlima-tech
