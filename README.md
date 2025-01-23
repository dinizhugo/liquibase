# Projeto de Estudos - Liquibase

Este é um repositório dedicado a estudos e testes com o **Liquibase**, uma ferramenta de gerenciamento de mudanças no banco de dados. O objetivo deste projeto é entender e aplicar conceitos fundamentais do Liquibase, além de aprender a realizar operações de versionamento e controle de mudanças em bancos de dados relacionais.

## Tecnologias

- **Liquibase**: Ferramenta de controle de versão de banco de dados.
- **MySQL**: Banco de dados relacional utilizado no projeto.
- **Java**: Linguagem de programação utilizada para interagir com o Liquibase.
- **Maven**: Gerenciador de dependências e construção utilizado no projeto.

## Funcionalidades

O projeto inclui os seguintes cenários:

1. **Criação de tabelas**: Definição de schema inicial do banco de dados.
2. **Alterações no banco de dados**: Inclusão de novas tabelas, remoção de tabelas existentes, adição e alteração de colunas, e inserção de dados.
3. **Versionamento do banco de dados**: Uso de Liquibase para aplicar mudanças de forma controlada e versionada.

## Como Rodar

### Pré-requisitos

- **Java 17 ou superior** (para rodar o Liquibase e o Maven)
- **Maven** (para gerenciar dependências)
- **MySQL** (ou outro banco de dados relacional)

### Passo 1: Configuração do banco de dados

1. Instale o **MySQL** e crie um banco de dados para o projeto (ex: `redesocial`).
   
2. Configure a conexão no arquivo `liquibase.properties` com as credenciais e URL do banco de dados:
   
   ```properties
   changeLogFile=src/main/dbschema/changelog/db.changelog-root.xml
   url=jdbc:mysql://localhost:3306/redesocial
   driver=com.mysql.cj.jdbc.Driver
   username=root
   password=senha_do_banco
