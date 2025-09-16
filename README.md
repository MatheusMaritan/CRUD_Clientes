# Cadastro de Clientes

Projeto em Java para gerenciamento de clientes, implementando as operações básicas de **CRUD (Create, Read, Update, Delete)**.  
A aplicação utiliza **JDBC** para conexão e manipulação de dados em um banco de dados relacional (ex.: MySQL).

---

## 🚀 Funcionalidades

- Cadastrar novos clientes  
- Listar clientes existentes  
- Atualizar informações de clientes  
- Excluir registros do banco de dados  

---

## 🛠️ Tecnologias utilizadas

- **Java SE**  
- **JDBC**  
- **MySQL** (ou outro banco relacional configurado)  

---

## 📂 Estrutura do projeto

src/
├── Cliente.java # Classe modelo (entidade Cliente)
├── ClienteDAO.java # Classe de acesso a dados (CRUD via JDBC)
├── Conexao.java # Classe responsável pela conexão com o banco
└── Main.java # Classe principal para execução do sistema


---

## ⚙️ Pré-requisitos

- **Java JDK 8+**  
- **MySQL** (ou outro SGBD compatível)  
- **Driver JDBC** do banco configurado no classpath  

---

## 🔧 Configuração do Banco de Dados

1. Crie um banco de dados no MySQL:
   ```sql
   CREATE DATABASE cadastro_clientes;
   
   USE cadastro_clientes;
   
   CREATE TABLE cliente (
      id INT AUTO_INCREMENT PRIMARY KEY,
      nome VARCHAR(100) NOT NULL,
      email VARCHAR(100) NOT NULL,
      idade INT
    );

