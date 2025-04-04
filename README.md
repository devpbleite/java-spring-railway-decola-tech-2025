# Java Spring Railway - Decola Tech 2025

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Java](https://img.shields.io/badge/Java-17-orange)](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2-brightgreen)](https://spring.io/projects/spring-boot)

## 📝 Descrição

Este projeto foi desenvolvido como parte do bootcamp **Decola Tech 2025** da DIO, focado em boas práticas de desenvolvimento com Java e Spring Boot. A aplicação demonstra a criação de uma API RESTful com deploy na plataforma Railway.

## 🔧 Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.2**
- **Spring Data JPA**
- **Spring Security**
- **Spring Cloud**
- **Swagger**
- **PostgreSQL**
- **Railway para Deploy**

## 📋 Pré-requisitos

Para executar o projeto localmente, você precisará ter instalado:

- Java JDK 17+
- PostgreSQL (H2 localmente)

## 🚀 Instalação

1. Clone o repositório:
```bash
git clone https://github.com/devpbleite/java-spring-railway-decola-tech-2025.git
cd java-spring-railway-decola-tech-2025
```

2. Configure o banco de dados no arquivo `application.properties` (ou utilize as variáveis de ambiente):
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/seu_banco
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

3. Execute a aplicação:
```bash
# Linux/Mac
./gradlew bootRun

# Windows
gradlew.bat bootRun
```

4. Acesse a API em `http://localhost:8080`
5. Acesse a documentação Swagger em `http://localhost:8080/swagger-ui.html`

## 🔄 CI/CD com Railway

Este projeto utiliza a plataforma Railway para implementar um pipeline de CI/CD. A cada push para a branch main, o Railway:

1. Constrói a aplicação
2. Executa os testes
3. Realiza o deploy automaticamente

## 📚 Endpoints da API

A documentação completa dos endpoints está disponível via Swagger após iniciar a aplicação.

Principais endpoints:

- `GET /api/v1/products` - Lista todos os produtos
- `GET /api/v1/products/{id}` - Busca um produto por ID
- `POST /api/v1/products` - Cria um novo produto
- `PUT /api/v1/products/{id}` - Atualiza um produto existente
- `DELETE /api/v1/products/{id}` - Remove um produto


## 📊 Estrutura do Projeto

```
src
├── main
│   ├── java
│   │   └── com
│   │       └── devpbleite
│   │           ├── config
│   │           ├── controller
│   │           ├── exception
│   │           ├── model
│   │           ├── repository
│   │           ├── security
│   │           └── service
│   └── resources
│       ├── application.properties
│       ├── application-dev.properties
│       └── application-prod.properties
└── test
    └── java
        └── com
            └── devpbleite
                ├── controller
                ├── repository
                └── service
```

## 🔗 Links Úteis

- [Documentação do Spring Boot](https://docs.spring.io/spring-boot/docs/current/reference/html/)
- [Railway](https://railway.app/)
- [Programa Decola Tech 2025](https://www.dio.me/bootcamp/decola-tech-2025)

## ✒️ Autor

- **Pablo Leite** - [devpbleite](https://github.com/devpbleite)

---

⌨️ com ❤️ por [devpbleite](https://github.com/devpbleite)
