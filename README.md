# 📋 CRUD de Cadastro de Clientes com Java e MySQL

Este projeto consiste em um sistema de **Cadastro de Clientes** com operações CRUD (Create, Read, Update, Delete), utilizando **Java** com **JDBC** para a comunicação com o banco de dados **MySQL**. O sistema permite o gerenciamento completo de clientes, incluindo a validação de dados e tratamento de erros.

## 🧾 Enunciado da Atividade

> Desenvolver um sistema de cadastro de clientes com operações CRUD, utilizando Java, banco de dados MySQL e validações específicas.  
> **Professora:**  Juliana Forin Pasquini Martinez
---

## ✅ Funcionalidades

- **Cadastrar Cliente**  
  - Nome, CPF (único e válido), E-mail, Telefone, Endereço, Data de Nascimento (YYYY-MM-DD)
- **Listar Clientes**  
  - Exibição de todos os clientes
  - Busca por nome ou CPF
- **Atualizar Cliente**  
  - Edita todas as informações, exceto o CPF
- **Remover Cliente**  
  - Exclusão pelo CPF
- **Validações**  
  - Formato correto de CPF, e-mail, telefone e data
  - Campos obrigatórios preenchidos
  - Mensagens claras de erro para CPF duplicado, cliente inexistente etc.

---

## 🛠 Tecnologias Utilizadas

- **Java** (Orientação a Objetos)
- **JDBC** (Java Database Connectivity)
- **MySQL** (Sistema Gerenciador de Banco de Dados)

---

## 🗃 Estrutura da Tabela `clientes`

```sql
CREATE TABLE clientes (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nome VARCHAR(100),
  cpf VARCHAR(14) UNIQUE,
  email VARCHAR(100),
  telefone VARCHAR(20),
  endereco VARCHAR(200),
  data_nascimento DATE
);
```

## 📌 Observações

- A arquitetura segue boas práticas de Orientação a Objetos.

---
Por:
>[Raphaela Barbosa Monteiro](https://github.com/raphaelamonteiro) e
>[Raul Germano Rosendo de Oliveira Duarte](https://github.com/Raul-Germano-Rosendo)

---
