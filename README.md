# Desafio DIO: Processando e Transformando Dados com Power BI, MySQL e Azure

## 📋 Sobre o Projeto
Este repositório contém a solução desenvolvida para o desafio prático da **DIO**, focado em engenharia, limpeza, tratamento e modelagem de dados. O projeto demonstra um fluxo de ETL (*Extract, Transform, Load*) robusto integrando banco de dados relacional, ambiente em nuvem e ferramentas de transformação.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Power Query:** Motor de transformação de dados responsável pela limpeza profunda, tratamento de valores nulos, ajuste de tipos e estruturação das tabelas.
* **MySQL:** Gestão, consultas estruturadas e extração de dados do banco relacional.
* **Microsoft Azure:** Integração de dados, suporte a serviços e armazenamento em ambiente de computação em nuvem.
* **Power BI (Modelagem):** Importação, estruturação e criação do modelo de dados relacional (Esquema Estrela).
* **Git & GitHub:** Versionamento de código e estruturação do portfólio.

---

## ⚙️ Etapas de Desenvolvimento do Projeto
1. **Conexão e Extração:** Configuração e conexão com as fontes de dados utilizando **MySQL** e recursos hospedados no **Azure**.
2. **Tratamento e Transformação (Power Query):**
   * Correção de tipos de dados e padronização de nomenclaturas.
   * Tratamento de inconsistências, valores ausentes e remoção de duplicadas.
   * Criação de colunas condicionais e personalizadas conforme as regras de negócio exigidas.
3. **Modelagem de Dados:** Estabelecimento de relacionamentos precisos e criação de tabelas fato e dimensões preparadas para análise.

---

## 📁 Estrutura do Repositório
```text
├── sql/                     # Scripts e consultas SQL utilizadas
├── powerbi/                 # Arquivos de modelo e transformação (.pbix)
└── README.md                # Documentação do projeto
