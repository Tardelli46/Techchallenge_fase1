# Tech Challenge — Fase 1 | Data Analytics 📊

> Pós-Tech FIAP · Turma 2026

![Jupyter](https://img.shields.io/badge/Ferramenta-Jupyter%20Notebook-orange)
![Status](https://img.shields.io/badge/Status-Concluído-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 🎯 Objetivo

O trabalho investiga uma hipótese central: **o crescimento acelerado da Olist entre 2016 e 2018 pressionou a infraestrutura logística da plataforma, gerando aumento nos atrasos e queda direta na satisfação dos clientes.**

A análise parte de dados transacionais reais e constrói uma narrativa executiva — do volume de pedidos à experiência do cliente — com foco em evidências quantitativas e recomendações acionáveis para investidores.

---

## 📦 Dataset

**Brazilian E-Commerce Public Dataset by Olist** — disponível no [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

Conjunto de dados públicos com pedidos reais (anonimizados) realizados em marketplaces brasileiros. A análise cobre o período de **setembro de 2016 a outubro de 2018**, com foco nas tabelas de pedidos, itens, pagamentos, reviews, clientes, vendedores e produtos.

| Tabela | Conteúdo |
|--------|----------|
| `olist_orders_dataset.csv` | Ciclo de vida do pedido: status, datas de compra, aprovação e entrega |
| `olist_order_items_dataset.csv` | Composição dos pedidos: produto, seller, preço e frete por item |
| `olist_order_payments_dataset.csv` | Forma e valor de pagamento, número de parcelas |
| `olist_order_reviews_dataset.csv` | Nota do cliente (1–5) e comentários pós-entrega |
| `olist_customers_dataset.csv` | Identificador único de cliente, localização por CEP e estado |
| `olist_sellers_dataset.csv` | Cadastro de vendedores com estado e cidade |
| `olist_products_dataset.csv` | Categoria, peso e dimensões dos produtos |

---

## 🗂️ Estrutura da Análise

O notebook está organizado em 6 blocos sequenciais:

| Bloco | Foco |
|-------|------|
| **1. Preparação dos dados** | Merge das 7 tabelas, engenharia de features, checagem de qualidade e cobertura |
| **2. KPIs executivos** | Painel de indicadores: receita total, ticket médio, nota média, % atraso, frete |
| **3. Crescimento** | Evolução mensal de receita e pedidos, expansão geográfica, categorias, segmentação RFM e projeção de tendência |
| **4. Logística** | Pipeline de entrega por etapa (aprovação → postagem → transporte), atrasos por estado e meios de pagamento |
| **5. Satisfação** | Correlação entre atraso e nota, impacto por faixa de prazo, desempenho de sellers e mapa de estados |
| **6. Conclusões** | Tabela-resumo de achados e recomendações estratégicas |

---

## 📥 Como executar

### 1. Baixe os dados

Acesse o dataset no [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) e extraia os arquivos CSV dentro de uma pasta chamada `data_sets/` na raiz do projeto:

```
data_sets/
├── olist_orders_dataset.csv
├── olist_order_items_dataset.csv
├── olist_order_payments_dataset.csv
├── olist_order_reviews_dataset.csv
├── olist_customers_dataset.csv
├── olist_sellers_dataset.csv
└── olist_products_dataset.csv
```

### 2. Abra o notebook

```bash
jupyter notebook TECHCHALLENGE.ipynb
```

Execute as células na ordem — cada bloco depende das variáveis geradas pelo anterior.

---

## 🔍 Principais Resultados

- **Crescimento expressivo**: o volume de pedidos cresceu de forma consistente ao longo dos dois anos, com expansão para todos os estados do Brasil.
- **Degradação logística acompanha o crescimento**: o percentual de pedidos com atraso aumentou à medida que o volume escalou.
- **Atraso penaliza fortemente a avaliação**: pedidos atrasados recebem nota média de **2,57**, contra **4,29** para entregas no prazo — uma queda de **1,73 pontos**.
- **Pipeline de entrega longo**: lead time médio total de **12,6 dias**, sendo o transporte a etapa mais demorada.
- **Concentração de receita em poucos sellers**: pequena parcela dos vendedores responde por 80% da receita, criando risco de dependência operacional.
- **Retenção de clientes baixa**: taxa de recompra em torno de 3%, indicando que o crescimento se apoia majoritariamente em aquisição de novos clientes.
- **Qualidade varia significativamente por categoria**: existe um gap relevante de satisfação entre as categorias mais bem e pior avaliadas.

---

## 📌 Entregáveis

- Notebook analítico completo (`TECHCHALLENGE.ipynb`)
- Relatório executivo em formato ABNT
- Apresentação com os principais achados e recomendações

---

## 📚 Referências

- Olist — Brazilian E-Commerce Public Dataset (Kaggle, 2018)
- Documentação Pandas, Matplotlib, Seaborn e NumPy
- E-Commerce Report Brasil — ABComm/Ebit|Nielsen (2017–2018)

---

## 👤 Autor

| Nome | RM |
|------|----|
| **Felipe Lins Prado Tardelli** | 374386 |

---
