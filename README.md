# 🗳️ Sistema de Eleição

Sistema web desenvolvido em **PHP e MySQL** para gerenciamento de informações de **eleitores e candidatos**. O projeto foi desenvolvido como atividade acadêmica, com o objetivo de praticar conceitos de desenvolvimento web, banco de dados e operações CRUD.

## 📌 Sobre o Projeto

O **Sistema de Eleição** permite cadastrar, consultar, editar e excluir registros de eleitores e candidatos por meio de uma interface web simples e intuitiva.

O sistema possui duas áreas principais:

* 👥 **Eleitores**
* 🗳️ **Candidatos**

A aplicação utiliza o banco de dados **MySQL** para armazenar as informações e **PHP com PDO** para realizar a comunicação entre o sistema e o banco.

## ⚙️ Funcionalidades

### 👥 Gerenciamento de Eleitores

* Cadastrar novos eleitores;
* Listar eleitores cadastrados;
* Pesquisar por:

  * Nome;
  * Número do título;
  * Cidade;
* Editar informações;
* Excluir eleitores;
* Validação de campos obrigatórios;
* Verificação de títulos eleitorais duplicados.

### 🗳️ Gerenciamento de Candidatos

* Cadastrar candidatos;
* Listar candidatos;
* Editar informações;
* Excluir candidatos;
* Informar número do candidato;
* Informar cargo;
* Informar partido fictício;
* Verificação de números de candidatos duplicados.

## 🛠️ Tecnologias Utilizadas

| Tecnologia     | Utilização                                        |
| -------------- | ------------------------------------------------- |
| **PHP**        | Desenvolvimento do back-end e regras da aplicação |
| **MySQL**      | Banco de dados                                    |
| **HTML5**      | Estrutura das páginas                             |
| **CSS3**       | Estilização e interface                           |
| **PDO**        | Conexão e consultas ao banco de dados             |
| **Git/GitHub** | Versionamento e armazenamento do projeto          |

## 📂 Estrutura do Projeto

```text
Kauan_ATIVIDADE_SAEP/
│
├── css/
│   └── style.css
│
├── candidatos.php
├── candidato_criar.php
├── candidato_editar.php
├── candidato_excluir.php
│
├── eleitor_criar.php
├── eleitor_editar.php
├── eleitor_excluir.php
│
├── index.php
├── db.php
├── functions.php
└── schema.sql
```

## 🗄️ Banco de Dados

O projeto utiliza o banco de dados **MySQL**.

O arquivo `schema.sql` contém a estrutura necessária para criação das tabelas utilizadas pela aplicação.

### Tabela `eleitor`

Armazena informações dos eleitores:

* `id_eleitor`
* `nome`
* `numero_titulo`
* `cidade`

### Tabela `candidato`

Armazena informações dos candidatos:

* `id_candidato`
* `nome`
* `numero_candidato`
* `cargo`
* `partido_ficticio`

## 🚀 Como Executar o Projeto

### 1. Requisitos

Para executar o projeto localmente, é necessário ter instalado:

* PHP;
* MySQL;
* Apache ou outro servidor compatível com PHP;
* XAMPP, WAMP ou ambiente semelhante.

### 2. Clonar o repositório

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
```

Entre na pasta do projeto:

```bash
cd Kauan_ATIVIDADE_SAEP
```

### 3. Configurar o banco de dados

Abra o **MySQL** ou o **phpMyAdmin** e crie o banco:

```sql
CREATE DATABASE eleicao;
```

Depois, selecione o banco:

```sql
USE eleicao;
```

Execute o conteúdo do arquivo:

```text
schema.sql
```

para criar as tabelas e inserir os dados iniciais.

### 4. Configurar a conexão

No arquivo `db.php`, configure os dados de acesso ao MySQL:

```php
$host = 'localhost';
$dbname = 'eleicao';
$user = 'root';
$pass = 'SUA_SENHA';
```

> ⚠️ Não publique senhas reais no GitHub. O ideal é utilizar variáveis de ambiente ou um arquivo de configuração que não seja enviado ao repositório.

### 5. Executar o projeto

Se estiver utilizando XAMPP, coloque a pasta do projeto dentro de:

```text
C:\xampp\htdocs\
```

Inicie:

* Apache
* MySQL

Depois, acesse no navegador:

```text
http://localhost/Kauan_ATIVIDADE_SAEP/
```

## 🔄 Operações CRUD

O sistema utiliza o conceito de **CRUD**:

| Operação   | Descrição                          |
| ---------- | ---------------------------------- |
| **Create** | Cadastro de eleitores e candidatos |
| **Read**   | Consulta e listagem dos registros  |
| **Update** | Edição dos registros               |
| **Delete** | Exclusão dos registros             |

## 🔐 Segurança

O projeto utiliza alguns mecanismos básicos para melhorar a segurança da aplicação, como:

* Consultas preparadas com **PDO**;
* Validação de campos obrigatórios;
* Verificação de registros duplicados;
* Uso de `htmlspecialchars()` para tratamento da saída de dados;
* Conversão de IDs para valores inteiros antes das consultas.

## 🎓 Objetivo Acadêmico

Este projeto foi desenvolvido com finalidade acadêmica, buscando aplicar na prática conhecimentos relacionados a:

* Desenvolvimento de aplicações web;
* Programação em PHP;
* Banco de dados relacionais;
* SQL;
* Operações CRUD;
* Conexão entre back-end e banco de dados;
* HTML e CSS;
* Organização de projetos.

## 📚 Aprendizados

Durante o desenvolvimento, foram praticados conceitos como:

* Conexão entre PHP e MySQL;
* Criação e manipulação de tabelas;
* Utilização de `SELECT`, `INSERT`, `UPDATE` e `DELETE`;
* Utilização de formulários HTML;
* Validação de informações;
* Consultas preparadas;
* Organização de arquivos PHP;
* Desenvolvimento de interfaces para sistemas administrativos.

## 👨‍💻 Autor

**Kauan**

Projeto desenvolvido para fins acadêmicos — **SAEP / Desenvolvimento de Sistemas**.

---

⭐ **Projeto desenvolvido para prática e aprendizado em desenvolvimento web.**
