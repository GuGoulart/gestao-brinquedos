# Projeto Spring Boot - Gerenciamento de Brinquedos

## Descrição do Projeto

Este projeto é uma aplicação backend para uma empresa de brinquedos infantis (até 14 anos), desenvolvida em Java com Spring Boot e Maven. O sistema implementa um CRUD completo para gerenciar brinquedos, conectando-se a um banco de dados Oracle na tabela `TDS_TB_Brinquedos` via JPA.

Os endpoints REST permitem criar, consultar, atualizar e excluir brinquedos, utilizando os campos: Id, Nome, Tipo, Classificação, Tamanho e Preço. Os testes das APIs são realizados via Postman, usando `localhost` na porta `8080` com servidor Tomcat.

O acesso ao banco é feito via `JpaRepository`, e o projeto conta com validações usando Bean Validation para garantir a integridade dos dados antes do commit.

## Configuração Inicial

A configuração do projeto foi feita pelo Spring Initializr, incluindo as principais dependências para Web, JPA, Oracle Driver e Validation.

![Configuração do Spring Initializr]![imagem](https://github.com/user-attachments/assets/2ce832a4-9143-4977-8974-c5882e37b400)


## Explicação do CRUD

- **Create (POST):** Insere um novo brinquedo no banco de dados.  
- **Read (GET):** Lista todos os brinquedos ou busca por ID.  
- **Update (PUT):** Atualiza os dados de um brinquedo existente.  
- **Delete (DELETE):** Remove um brinquedo pelo ID.

## Validações, JPA e Conexão Oracle

- **Validações:** São aplicadas anotações de Bean Validation para garantir campos obrigatórios e formatos corretos (ex: `@NotNull`, `@Size`).  
- **JPA:** Utiliza `JpaRepository` para facilitar a persistência e recuperação dos dados na tabela Oracle.  
- **Conexão Oracle:** Configurada via `application.properties`, conectando ao banco Oracle `ORACLE_FIAP` para operações de CRUD.

## Testes no Postman

Foram realizados testes completos das APIs usando Postman, contemplando todos os métodos CRUD. Os prints das telas mostram requisições e respostas esperadas para cada endpoint.

*Exemplo de prints:*

![Teste GET Brinquedos]![imagem (2)](https://github.com/user-attachments/assets/a51254b6-2b16-47ab-b751-5178036896e8)
![Teste POST Brinquedo]![imagem (1)](https://github.com/user-attachments/assets/c04a2b7b-5c5f-43e3-90ad-638f8cbaebcf)
![Teste PUT Brinquedo]![imagem (3)](https://github.com/user-attachments/assets/fb174671-e2ef-4e06-9d63-ead0a237ca87)
![Teste DELETE Brinquedo]![imagem (4)](https://github.com/user-attachments/assets/57e263a4-9c7c-4337-8a62-ee7fab0206c6)
![Teste GET Brinquedos após o DELETE]![imagem (5)](https://github.com/user-attachments/assets/a64f3d35-b562-4ad1-9a95-df1026f04bb7)


## Tecnologias Utilizadas

- Java 17  
- Spring Boot  
- Spring Data JPA  
- Oracle Database  
- Maven  
- Bean Validation  
- IDE: IntelliJ

---

## Integrantes do Grupo

- Gustavo Goulart Bretas - RM: 555708 

---

