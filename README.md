# 📊 Sales Pipeline 360: Inteligência Comercial & Financial Analytics
> **Foco:** Transformação de dados brutos em decisões estratégicas utilizando Modelagem Dimensional e IA.

![Status do Projeto](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Stack](https://img.shields.io/badge/Stack-SQL%20|%20Python%20|%20PBI%20|%20LLM-blue)

## 🏢 Contexto de Negócio
Este projeto simula a operação de uma empresa de varejo/distribuição com presença nacional. Como **Analista de Dados**, meu objetivo foi estruturar um pipeline que não apenas reporte o passado, mas identifique padrões de comportamento financeiro para otimizar o fluxo de caixa e a rentabilidade por filial.

## 🏗️ Arquitetura da Solução
[cite_start]O diferencial deste projeto é a construção do **Data Warehouse** antes da visualização:

1.  **Ingestão & Limpeza (Python/Pandas):** Tratamento de dados brutos da Olist (ou sintéticos) para garantir integridade.
2.  [cite_start]**Modelagem Dimensional (BigQuery):** Estruturação em **Star Schema** (Tabela Fato de Vendas + Dimensões: Clientes, Produtos, Tempo e Vendedores).
3.  [cite_start]**Analytics Avançado (SQL):** Criação de métricas de retenção (Cohort), LTV e cálculos de ticket médio ponderado[cite: 14].
4.  [cite_start]**Interface de IA (LlamaIndex):** Camada de consulta em linguagem natural integrada ao banco de dados.
5.  [cite_start]**Visualização (Power BI):** Dashboard executivo focado em Storytelling e KPIs financeiros[cite: 19].

## 🧠 Perguntas de Negócio Respondidas
* **Análise de Rentabilidade:** Quais categorias possuem a melhor margem após custos logísticos?
* **Saúde do Funil:** Qual o ciclo médio de venda por região?
* [cite_start]**Behavioral Finance:** Como as diferentes formas de pagamento impactam a recorrência dos clientes? [cite: 22]

## 📂 Estrutura do Repositório
```text
project_sales_pipeline_360/
  ├─ data/        # Documentação dos datasets e metadados
  [cite_start]├─ notebooks/   # EDA (Análise Exploratória) e Testes de Modelos de ML/LLM [cite: 15]
  [cite_start]├─ sql/         # Scripts de criação do DW, Views e Queries Analíticas [cite: 14]
  [cite_start]├─ powerbi/     # Arquivos .pbix e Guia de Métricas DAX [cite: 19]
  └─ README.md
