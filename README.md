# 🛒 E-commerce Data Simulator & Analytics

Este projeto simula um cenário real de varejo para análise de dados, focando em Engenharia de Dados, SQL Avançado e Storytelling.

## 🛠 Tecnologias Utilizadas
- **Linguagem:** Python 3.9+
- **Bibliotecas:** Pandas, Seaborn, Faker, SQLAlchemy
- **Banco de Dados:** SQLite (In-memory/File)
- **Conceitos:** ETL, Window Functions, Data Modeling

## 🎯 Destaques do Projeto

### 1. Engenharia de Dados (ETL)
Em vez de usar datasets estáticos, desenvolvi um pipeline que gera dados sintéticos baseados em **regras de negócio reais**:
- Pesos demográficos customizados (Gen Z, Millennials, etc).
- Geração de transações e produtos com faixas de preço lógicas.

### 2. SQL Avançado
Utilização de **Window Functions** para análises complexas, superando agregações simples:
```sql
-- Exemplo: Ranking de melhores clientes (Whales) por Estado
DENSE_RANK() OVER (PARTITION BY estado ORDER BY total_investido DESC)
