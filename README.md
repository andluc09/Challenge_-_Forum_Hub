# Challenge - Forum Hub

## 📋 Descrição do Projeto

ㅤㅤㅤEste projeto é uma API REST desenvolvida com Spring Boot que implementa um CRUD (CREATE, READ, UPDATE, DELETE) permitindo o gerenciamento de tópicos utilizando uma base de dados relacional para a persistência da informação. Além de incluir a funcionalidade de autenticação/autorização de usuários por meio de JWT para restringir o acesso à informação, seguindo as melhores práticas de segurança.

## Ferramentas utilizadas

-  **Java 17**

-  **Spring Boot**

-  **Spring Security**

-  **JPA / Hibernate**

-  **Banco de Dados: MySQL**

-  **Lombok**

-  **JWT - JSON Web Tokens**

## Funcionalidades

- Registro e autenticação de usuários.

- Criação, listagem, atualização e exclusão de tópicos.

- Validação de dados de entrada.

- Retorno de informações detalhadas sobre os tópicos.

## 🛠 Instalação

1. **Clone o repositório**

   ```bash
   git clone https://github.com/andluc09/Forum_Hub.git
   cd Forum_Hub

2. **Configure o Banco de Dados**

No arquivo src/main/resources/application.properties, adicione as configurações necessárias para o banco de dados. 

3. **Execute o Projeto**

   ```bash
   ./mvnw spring-boot:run

Utilize o comando acima para executar a aplicação.

## Gerando o Token JWT

Para gerar um token JWT, você deve primeiro autenticar um usuário. Siga os passos abaixo:

1. **Faça uma requisição POST para o endpoint `/login` com as credenciais do usuário:**

   - **URL**: `http://localhost:8080/login`
   - **Body**:
     ```json
     {
       "login": "seu_login",
       "senha": "sua_senha"
     }
     ```

2. **Resposta esperada:**
   Se a autenticação for bem-sucedida, você receberá um token JWT no formato:

   ```json
   {
     "token": "seu_token_jwt"
   }

## Testando a API

Utilize ferramentas como **Insomnia** ou **Postman** para testar a API de forma prática e intuitiva.

## Endpoints Principais

- **POST /login**: 
  - Autentica o usuário e retorna um token JWT.

- **POST /topicos**: 
  - Cria um novo tópico com os dados fornecidos.

- **GET /topicos**: 
  - Lista todos os tópicos disponíveis.

- **GET /topicos/{id}**: 
  - Retorna detalhes de um tópico específico, onde `{id}` é o identificador do tópico.

- **PUT /topicos/{id}**: 
  - Atualiza informações de um tópico existente, onde `{id}` é o identificador do tópico.

- **DELETE /topicos/{id}**: 
  - Deleta um tópico específico, onde `{id}` é o identificador do tópico.

## Autor

<div><a href="https://github.com/andluc09" style="text-decoration: none;">
<img style="border-radius: 50%;" width="150px;" src="https://avatars.githubusercontent.com/u/70043466?v=4" alt="André Santos"/>

<strong>André Santos</strong></a></div> 

[![Linkedin Badge](https://img.shields.io/badge/-André_Santos-blue?style=flat-square&logo=Linkedin&logoColor=white&link=[https://www.linkedin.com/in/thalya-alves/])](https://www.linkedin.com/in/andre-lucas-backend-java/)
