# 📊 Sales Pipeline 360: Inteligência Comercial & Financial Analytics
> **Foco:** Transformação de dados brutos em decisões estratégicas utilizando Modelagem Dimensional, Estatística Aplicada e IA.

![Status do Projeto](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![Stack](https://img.shields.io/badge/Stack-SQL%20|%20Python%20|%20PBI%20|%20LLM-blue)

---

## 🏢 1. Contexto de Negócio
Muitas empresas de varejo e distribuição sofrem com a **"miopia de dados"**: possuem milhares de registros de vendas, mas não conseguem identificar quais clientes são realmente lucrativos ou qual o impacto real dos custos logísticos na margem final.

Este projeto foi desenvolvido para atuar como o **Data Warehouse (DW)** central de uma operação nacional. O objetivo é permitir que a diretoria financeira e comercial tome decisões baseadas em evidências, otimizando o fluxo de caixa e a rentabilidade por filial através de uma visão 360º da operação.

---

## 🏗️ 2. Arquitetura da Solução
O diferencial deste projeto é a construção da infraestrutura de dados completa antes da camada de visualização:

1.  **Tratamento e Engenharia de Atributos (Python/Pandas):** Limpeza de dados brutos da Olist (ou sintéticos), tratamento de nulos, padronização de tipos e criação de novas variáveis como *Lead Time* e *Margem de Contribuição*.
2.  **Modelagem Dimensional (BigQuery):** Estruturação em **Star Schema** (Esquema Estrela), organizando os dados em Tabelas Fato de Vendas e Dimensões (Clientes, Produtos, Tempo e Vendedores) para máxima performance analítica.
3.  **Analytics Avançado (SQL):** Desenvolvimento de métricas de retenção (*Cohort*), *Lifetime Value* (LTV) e cálculos de ticket médio ponderado utilizando CTEs e *Window Functions*.
4.  **Interface de IA (LlamaIndex):** Implementação de uma camada de consulta em linguagem natural integrada ao BigQuery, democratizando o acesso ao dado para usuários não técnicos.
5.  **Visualização Estratégica (Power BI):** Dashboard executivo focado em *Storytelling* e indicadores financeiros de alto impacto.

---

## 🛠️ 3. Tecnologias & Hard Skills Aplicadas
* **SQL (BigQuery):** Modelagem dimensional, Joins complexos, CTEs e funções de janela.
* **Python:** `Pandas` para ETL, `Scikit-Learn` para clusterização K-means e `Matplotlib/Seaborn` para análise exploratória.
* **Power BI:** Modelagem de dados, DAX avançado (`CALCULATE`, `ALL`, `DATESYTD`) e design de dashboards.
* **IA/LLM:** `LlamaIndex` para estruturação de RAG (Redação Aumentada por Recuperação) sobre dados tabulares.

---

## 🧠 4. Inteligência de Negócio: Perguntas Respondidas

O pipeline foi desenhado para responder a desafios críticos divididos em 4 pilares:

### 💰 Pilar 1: Performance de Vendas e Crescimento
* **Crescimento Mensal (MoM):** Qual a taxa de crescimento da receita mês a mês e onde estão os gargalos de sazonalidade?
* **Ticket Médio por Categoria:** Como o ticket médio varia entre categorias e quais regiões possuem maior poder de compra?
* **Concentração de Receita (Pareto):** Quais são os 20% de produtos responsáveis por 80% do faturamento?

### 👥 Pilar 2: Comportamento do Cliente (Behavioral Analytics)
* **Segmentação RFM:** Como os clientes se distribuem nos clusters de Recência, Frequência e Valor?
* **Lifetime Value (LTV):** Qual o valor projetado que cada cluster de cliente traz para a companhia?
* **Análise de Cohort:** Qual a taxa de retenção por mês de aquisição e o tempo médio para a segunda compra?
* **Preferência de Pagamento:** Existe correlação entre o parcelamento e o aumento no ticket médio?

### 🚚 Pilar 3: Eficiência Logística e Custos (Financial Impact)
* **Impacto do Frete na Conversão:** O valor do frete atua como barreira de saída em regiões específicas?
* **Lead Time vs. Satisfação:** Qual a correlação estatística entre o tempo de entrega e as avaliações dos clientes?
* **Otimização Geográfica:** Quais estados apresentam o maior custo logístico em relação à margem de contribuição?

### 🤖 Pilar 4: Predição e Consultas Inteligentes (IA & LLM)
* **Análise de Elasticidade-Preço:** Como variações nos preços impactam o volume de vendas e a receita total?
* **Consulta Semântica:** Como gestores podem identificar anomalias usando linguagem natural sem depender de relatórios estáticos?

---

## 📂 5. Entregáveis do Repositório
* **/data**: Documentação dos metadados e dicionário de dados.
* **/notebooks**: Análise Exploratória (EDA) e modelos de clusterização/estatística.
* **/sql**: Scripts de criação do Data Warehouse e Views analíticas.
* **/powerbi**: Arquivo `.pbix` e capturas de tela do dashboard final.

---

## 📈 6. Principais Descobertas (Insights)
*(Espaço para preencher após a execução - Exemplos abaixo)*
* **Insight 1:** Clientes do cluster "Diamante" possuem um LTV 3x superior à média, mas são sensíveis ao *Lead Time* acima de 5 dias.
* **Insight 2:** A forma de pagamento via Boleto apresenta uma taxa de cancelamento X% superior ao Cartão de Crédito.

---

## 🖼️ 7. Demonstração Visual
*(Insira aqui os prints do seu dashboard e o diagrama da sua arquitetura)*

---

## 🚀 8. Como Reproduzir este Projeto
1.  Clone o repositório.
2.  Importe os arquivos da pasta `/data` para o Google BigQuery.
3.  Execute os scripts na pasta `/sql` para estruturar o Data Warehouse.
4.  Utilize o notebook em `/notebooks` para processar as análises estatísticas.
5.  Abra o relatório em `/powerbi` para visualizar os insights.

---

## 🤝 Contato
* **Felipe** - Economista & Analista de Dados
* [Seu LinkedIn Aqui]
* [Seu E-mail Aqui]
