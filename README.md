* Baozi Store API



* Sobre o projeto



A Baozi Store API é uma API REST desenvolvida como atividade prática da disciplina de Desenvolvimento Web Back-End da UNINTER.



O projeto simula o sistema de gerenciamento de uma loja fictícia de produtos de informática, permitindo realizar o cadastro, a consulta e a exclusão de clientes, produtos e pedidos, utilizando um banco de dados relacional.



* Tecnologias utilizadas



\- Java 25

\- Spring Boot 4.2.0

\- Spring Web

\- Spring Data JPA

\- Hibernate

\- MySQL 8.0

\- Maven

\- Eclipse IDE

\- Postman

\- Git e GitHub



* Estrutura do projeto



&#x20;   com.baozistore

&#x20;   ├── BaoziStoreApiApplication.java

&#x20;   ├── controller

&#x20;   │   ├── ClienteController.java

&#x20;   │   ├── ProdutoController.java

&#x20;   │   └── PedidoController.java

&#x20;   ├── model

&#x20;   │   ├── Cliente.java

&#x20;   │   ├── Produto.java

&#x20;   │   └── Pedido.java

&#x20;   └── repository

&#x20;       ├── ClienteRepository.java

&#x20;       ├── ProdutoRepository.java

&#x20;       └── PedidoRepository.java



* Endpoints da API



Clientes



| Método | Endpoint | Descrição |

|---|---|---|

| POST | /clientes | Cadastrar cliente |

| GET | /clientes | Listar todos os clientes |

| GET | /clientes/{id} | Buscar cliente por ID |

| DELETE | /clientes/{id} | Excluir cliente |



Produtos



| Método | Endpoint | Descrição |

|---|---|---|

| POST | /produtos | Cadastrar produto |

| GET | /produtos | Listar todos os produtos |

| GET | /produtos/{id} | Buscar produto por ID |

| DELETE | /produtos/{id} | Excluir produto |



Pedidos



| Método | Endpoint | Descrição |

|---|---|---|

| POST | /pedidos | Cadastrar pedido |

| GET | /pedidos | Listar todos os pedidos |

| GET | /pedidos/{id} | Buscar pedido por ID |

| DELETE | /pedidos/{id} | Excluir pedido |



* Banco de dados



O projeto utiliza o MySQL para o armazenamento dos registros.



Nome do banco de dados: `baozi\_store`



As tabelas são gerenciadas pelo Hibernate por meio do Spring Data JPA.



* Como executar



1\. Clone o repositório:



&#x20;      git clone https://github.com/MuriloVitoriano/baozi-store-api-dev-web.git



2\. Acesse a pasta do projeto:



&#x20;      cd baozi-store-api-dev-web



3\. Crie o banco de dados no MySQL:



&#x20;      CREATE DATABASE baozi\_store;



4\. Configure um usuário MySQL com permissão de acesso ao banco de dados.



5\. Configure as variáveis de ambiente:



&#x20;  - DB\_USERNAME: usuário do MySQL.

&#x20;  - DB\_PASSWORD: senha do MySQL.



6\. Execute a aplicação pelo Eclipse ou pelo Maven Wrapper no Windows:



&#x20;      mvnw.cmd spring-boot:run



7\. A API estará disponível em:



&#x20;      http://localhost:8080



* Testes realizados



Os 12 endpoints foram testados utilizando o Postman, verificando as operações de cadastro, listagem, consulta por ID e exclusão de clientes, produtos e pedidos.



\## Segurança



As credenciais do banco de dados são configuradas por meio de variáveis de ambiente, evitando a exposição da senha no código-fonte.



* Autor



\--Murilo Vitoriano Bezerra--



Instituição: Centro Universitário Internacional — UNINTER



Disciplina: Desenvolvimento Web Back-End



Ano: 2026



* Finalidade



Projeto desenvolvido para fins acadêmicos, com o objetivo de aplicar os conhecimentos de desenvolvimento de APIs REST, arquitetura em camadas e integração com banco de dados.

