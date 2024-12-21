# Governança e Qualidade de Dados com Great Expectations

Este repositório contém um exemplo prático de validação de dados em um Data Warehouse utilizando a ferramenta open source **Great Expectations**. O objetivo é garantir a qualidade e a governança de dados em tabelas de dimensões e fatos.

## Funcionalidades

- Validação de dados em tabelas:
  - `dim_produto`
  - `dim_canal`
  - `dim_cliente`
  - `fato_venda`
- Geração de relatórios em formato PDF para cada tabela validada.
- Integração com PostgreSQL utilizando uma arquitetura local baseada em Docker.

## Tecnologias

- **Great Expectations**: para validação e governança de dados.
- **PostgreSQL**: banco de dados utilizado para armazenar os dados.
- **Docker**: para criar o ambiente local com PostgreSQL de forma simples e isolada.
- **Python**: para executar a validação dos dados.

## Estrutura do Repositório

```plaintext
.
├── script.py                   # Código Python principal de validação com Great Expectations
├── modelo_fisico.sql           # Script para criação do modelo físico (tabelas do banco de dados)
├── etl.sql                      # Script SQL para popular as tabelas com dados
├── validation_reports          # Diretório contendo os relatórios gerados (PDFs)
│   ├── validation_report_dim_produto.pdf
│   ├── validation_report_dim_canal.pdf
│   ├── validation_report_dim_cliente.pdf
│   └── validation_report_fato_venda.pdf
├── requirements.txt            # Dependências do projeto
└── README.md                   # Documentação do projeto
