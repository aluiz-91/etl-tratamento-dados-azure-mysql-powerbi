# Desafio DIO: Processando e Transformando Dados com Power BI, MySQL e Azure

## 📋 Sobre o Projeto
Este repositório contém a solução desenvolvida para o desafio prático da DIO, focado em engenharia, limpeza, tratamento e modelagem de dados. O projeto demonstra um fluxo de ETL (*Extract, Transform, Load*) robusto integrando banco de dados relacional, ambiente em nuvem e ferramentas de transformação.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Power Query:** Motor de transformação de dados responsável pela limpeza profunda, tratamento de valores nulos, ajuste de tipos e estruturação das tabelas.
* **MySQL:** Gestão, consultas estruturadas e extração de dados do banco relacional.
* **Microsoft Azure:** Integração de dados, suporte a serviços e armazenamento em ambiente de computação em nuvem.
* **Power BI (Modelagem):** Importação, estruturação e criação do modelo de dados relacional (Esquema Estrela).
* **Git & GitHub:** Versionamento de código e estruturação do portfólio.

---

## ⚙️ Principais Transformações Aplicadas (ETL)
Durante o tratamento no Power Query, foram aplicadas as seguintes regras de negócio e boas práticas de engenharia de dados:
* **Tratamento de Nulos em `Super_ssn`:** Identificação e validação do colaborador sem supervisor direto (o Diretor geral, James E. Borg).
* **Operações de Mescla (*Merge*):** Cruzamento de dados para enriquecer as tabelas, unindo departamentos aos respetivos gerentes e associando departamentos às suas localizações (`dept_locations`), garantindo combinações únicas.
* **Uso Adequado de Mesclar vs. Acrescentar:** Utilização exclusiva de *Merge* para cruzamento de atributos relacionais estruturais, evitando duplicações indevidas de linhas (*Append*).
* **Agrupamento de Dados (*Group By*):** Agrupamento de colaboradores por gerente para contabilizar o rácio e a distribuição de equipas.
* **Ajuste de Tipos de Dados:** Padronização correta de colunas de data e conversão do campo de horas (`Hours`) para formato numérico adequado, eliminando formatações monetárias indevidas.
* **Limpeza e Otimização:** Remoção de colunas técnicas e redundantes desnecessárias para a camada de visualização e relatórios.

---

## 🚀 Etapas de Desenvolvimento do Projeto
1. **Conexão e Extração:** Configuração e conexão com as fontes de dados utilizando MySQL e recursos hospedados no Azure.
2. **Tratamento e Transformação (Power Query):**
   * Correção de tipos de dados e padronização de nomenclaturas.
   * Tratamento de inconsistências, valores ausentes e remoção de duplicadas.
   * Criação de colunas condicionais e personalizadas conforme as regras de negócio exigidas.
3. **Modelagem de Dados:** Estabelecimento de relacionamentos precisos e criação de tabelas fato e dimensões preparadas para análise.

---

## 📂 Estrutura do Repositório
```text
├── sql/         # Scripts e consultas SQL utilizadas
├── powerbi/     # Arquivos de modelo e transformação (.pbix)
└── README.md    # Documentação do projeto
