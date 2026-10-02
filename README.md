# Desafio DIO: Processando e Transformando Dados com Power BI, MySQL e Azure

## 📋 Sobre o Projeto
Este repositório contém a solução desenvolvida para o desafio prático da DIO, focado em engenharia, limpeza, tratamento e modelagem de dados[span_0](start_span)[span_0](end_span). O projeto demonstra um fluxo de ETL (*Extract, Transform, Load*) robusto integrando banco de dados relacional, ambiente em nuvem e ferramentas de transformação[span_1](start_span)[span_1](end_span).

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Power Query:** Motor de transformação de dados responsável pela limpeza profunda, tratamento de valores nulos, ajuste de tipos e estruturação das tabelas[span_2](start_span)[span_2](end_span).
* **MySQL:** Gestão, consultas estruturadas e extração de dados do banco relacional[span_3](start_span)[span_3](end_span).
* **Microsoft Azure:** Integração de dados, suporte a serviços e armazenamento em ambiente de computação em nuvem[span_4](start_span)[span_4](end_span).
* **Power BI (Modelagem):** Importação, estruturação e criação do modelo de dados relacional (Esquema Estrela)[span_5](start_span)[span_5](end_span).
* **Git & GitHub:** Versionamento de código e estruturação do portfólio[span_6](start_span)[span_6](end_span).

---

## ⚙️ Principais Transformações Aplicadas (ETL)
Durante o tratamento no Power Query, foram aplicadas as seguintes regras de negócio e boas práticas de engenharia de dados:
* **Tratamento de Nulos em `Super_ssn`:** Identificação e validação do colaborador sem supervisor direto (o Diretor geral, James E. Borg).
* **Operações de Mescla (*Merge*):** Cruzamento de dados para enriquecer as tabelas, unindo departamentos aos respetivos gerentes e associando departamentos às suas localizações (`dept_locations`), garantindo combinações únicas.
* **Uso Adequado de Mesclar vs. Acrescentar:** Utilização exclusiva de *Merge* para cruzamento de atributos relacionais estruturais, evitando duplicações indevidas de linhas (*Append*).
* **Agrupamento de Dados (*Group By*):** Agrupamento de colaboradores por gerente para contabilizar o rácio e a distribuição de equipas.
* **Ajuste de Tipos de Dados:** Padronização correta de colunas de data e conversão do campo de horas (`Hours`) para formato numérico adequado, eliminando formatações monetárias indevidas.
* **Limpeza e Otimização:** Remoção de colunas técnicas e redundantes desnecessárias para a camada de visualização e relatórios[span_7](start_span)[span_7](end_span).

---

## 🚀 Etapas de Desenvolvimento do Projeto
1. **Conexão e Extração:** Configuração e conexão com as fontes de dados utilizando MySQL e recursos hospedados no Azure[span_8](start_span)[span_8](end_span).
2. **Tratamento e Transformação (Power Query):**
   * Correção de tipos de dados e padronização de nomenclaturas[span_9](start_span)[span_9](end_span).
   * Tratamento de inconsistências, valores ausentes e remoção de duplicadas[span_10](start_span)[span_10](end_span).
   * Criação de colunas condicionais e personalizadas conforme as regras de negócio exigidas[span_11](start_span)[span_11](end_span).
3. **Modelagem de Dados:** Estabelecimento de relacionamentos precisos e criação de tabelas fato e dimensões preparadas para análise[span_12](start_span)[span_12](end_span).

---

## 📂 Estrutura do Repositório
```text
├── sql/         # Scripts e consultas SQL utilizadas[span_13](start_span)[span_13](end_span)
├── powerbi/     # Arquivos de modelo e transformação (.pbix)[span_14](start_span)[span_14](end_span)
└── README.md    # Documentação do projeto[span_15](start_span)[span_15](end_span)
