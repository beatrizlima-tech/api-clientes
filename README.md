# 📦 API Clientes - Spring Boot

![Java](https://img.shields.io/badge/Java-21-red?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.x-green?style=for-the-badge&logo=springboot)
![Build](https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge&logo=postgresql)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=for-the-badge)

---

## 📌 Sobre o projeto

A API Clientes é uma aplicação backend desenvolvida em Java com Spring Boot, responsável pelo gerenciamento de clientes (CRUD completo), utilizando conexão direta com banco de dados PostgreSQL via JDBC.

O projeto foi desenvolvido com foco em organização de código, boas práticas de API REST, integração com banco de dados relacional e documentação com Swagger/OpenAPI.

---

## 🚀 Funcionalidades

✔ Cadastro de clientes  
✔ Atualização de clientes  
✔ Exclusão lógica de clientes  
✔ Consulta de clientes por nome  
✔ Integração com PostgreSQL  
✔ Documentação via Swagger  

---

## 🧱 Tecnologias utilizadas

- Java 21  
- Spring Boot  
- Spring Web MVC  
- JDBC (Connection Factory manual)  
- PostgreSQL  
- SpringDoc OpenAPI (Swagger)  
- Maven  

---

## 🏗️ Estrutura do projeto

src/main/java/br/com/cotiinformatica/api_clientes/

├── configurations → Configurações gerais (CORS, Swagger)  
├── controllers → Endpoints da API  
├── dtos → Objetos de entrada (requests)  
├── entities → Entidades do sistema  
├── factories → Conexão com banco de dados (JDBC)  
├── repositories → Acesso ao banco (SQL puro)  

---

## 🔗 Endpoints da API

### Clientes

| Método | Endpoint              | Descrição           |
|--------|----------------------|---------------------|
| POST   | /api/v1/clientes     | Criar cliente       |
| PUT    | /api/v1/clientes/{id}| Atualizar cliente   |
| DELETE | /api/v1/clientes/{id}| Excluir cliente     |
| GET    | /api/v1/clientes/{nome} | Buscar por nome |

---

## ⚙️ Como executar o projeto

### 1. Clonar o repositório
git clone https://github.com/beatrizlima-tech/api-clientes.git

---

### 2. Criar banco de dados
CREATE DATABASE clientesdb;

---

### 3. Configurar application.properties
spring.datasource.url=jdbc:postgresql://localhost:5432/clientesdb  
spring.datasource.username=postgres  
spring.datasource.password=postgres  

---

### 4. Executar aplicação
mvn spring-boot:run

---

### 5. Acessar Swagger
http://localhost:8080/swagger-ui.html

---

## 📊 Arquitetura

Controller → Repository → JDBC → PostgreSQL

---

## 📌 Melhorias futuras

- Migrar JDBC para Spring Data JPA  
- Adicionar autenticação JWT  
- Implementar validação com Bean Validation  
- Criar testes automatizados completos  
- Dockerizar aplicação  

---

## 👩‍💻 Autora

Beatriz Lima  
GitHub: https://github.com/beatrizlima-tech
