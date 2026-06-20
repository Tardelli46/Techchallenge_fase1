# TECH CHALLENGE 1 - PÓS TECH FIAP 📊

> **TECH CHALLENGE 1 - Data Analytics** > Universidade FIAP - 2026

![Jupyter](https://img.shields.io/badge/Aplicação-Jupyter%20Notebook%20-orange)
![Status](https://img.shields.io/badge/Status-Concluído-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 Sobre o Projeto

**Case E-commerce Olist**
Este desafio propõe a construção de um relatório executivo voltado a investidores e acionistas do setor de e-commerce, baseado no Brazilian E-Commerce Public Dataset by Olist. O objetivo é transformar dados transacionais em uma narrativa clara sobre desempenho comercial, eficiência logística e/ou satisfação do cliente, culminando em recomendações acionáveis e, quando possível, previsões fundamentadas.

---

## 📈 Sobre o Dataset

O dataset reúne aproximadamente 100 mil pedidos entre 2016 e 2018, cobrindo múltiplos marketplaces no Brasil. Inclui tabelas interconectadas de clientes, pedidos, itens, produtos, vendedores, pagamentos, avaliações e geolocalização por CEP. Os dados são reais e foram anonimizados. Há possibilidade de análises multidimensionais, como status do pedido, preço, meios de pagamento, desempenho de frete, localização, atributos de produto e reviews. 

O dataset pode ser acessado aqui (https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

**Período**: Setembro de 2016 - Agosto de 2018  
**Formato**: CSV  
**Total de tabelas**: 8

## 🔎 Estrutura dos Dados e Dicionário

| Tabela | Descrição | Registros |
|--------|-----------|-----------|
| `olist_orders_dataset`: order_id, customer_id, status, timestamps de compra/aprovação/entrega | Informações dos pedidos | ~100k |
| `olist_order_items_dataset`: order_id, item_id, product_id, seller_id, shipping_limit_date, price, freight_value | Itens de cada pedido | ~112k |
| `olist_order_payments_dataset`: order_id, payment_type, installments, payment_value | Dados de pagamento | ~103k |
| `olist_order_reviews_dataset`: order_id, review_score, timestamps, review_comment_title/text | Avaliações dos clientes | ~99k |
| `olist_customers_dataset`: customer_id, customer_unique_id, zip_code_prefix, cidade, estado | Informações dos clientes | ~99k |
| `olist_sellers_dataset`: seller_id, zip_code_prefix, cidade, estado | Dados dos vendedores | ~3k |
| `olist_products_dataset`: product_id, category_name, pesos/medidas, descrição | Catálogo de produtos | ~32k |
| `olist_geolocation_dataset`: zip_code_prefix, latitude, longitude, cidade, estado | Dados geográficos | ~1M |
| `category_translation`: tradução de nomes de categorias para inglês |  |  |

---

## 📥 Como reproduzir a análise

### 1. Baixe o dataset
Download diretamente do Kaggle:

🔗 [Brazilian E-Commerce Public Dataset by Olist — Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Após baixar, extraia os arquivos CSV na pasta `dataset/`. Os arquivos esperados são:

```
data/
├── olist_orders_dataset.csv
├── olist_customers_dataset.csv
├── olist_order_items_dataset.csv
├── olist_order_payments_dataset.csv
├── olist_order_reviews_dataset.csv
├── olist_products_dataset.csv
└── olist_sellers_dataset.csv
```

### 2. Execute o notebook
Abra `notebook/TechChallenge1_Datanalytics_Postech_FIAP.ipynb` no Google Colab ou Jupyter e execute as células sequencialmente.

```bash
# Ou via terminal com Jupyter
jupyter notebook notebook/TechChallenge1_Datanalytics_Postech_FIAP.ipynb
```
---

## 📊 Principais Insights
- Crescimento consistente de receita entre 2016–2018.  
- Dependência de poucos sellers e regiões (SP concentra maior parte da receita).  
- Logística crítica em estados do Norte, impactando satisfação.  
- Baixa taxa de recompra (3,12%), indicando necessidade de fidelização.  
- Preferência cultural pelo parcelamento no cartão de crédito.  
- Polarização das avaliações (muitos 5, mas também muitos 1).  

---

## 📌 Entregáveis

- Relatório executivo em formato ABNT.
- Apresentação executiva com principais análises e destaques.
- Notebook completo, comentado e organizado trilha por trilha.  
- Documentação dos dados (premissas, qualidade, reprodutibilidade).  

---

## 📚 Referências

- Olist Dataset – Brazilian E-Commerce Public Dataset by Olist.  
- Relatórios de mercado de e-commerce no Brasil (2016–2018).  
- Estudos sobre comportamento de consumo e parcelamento no Brasil.  

---

## 👥 Integrantes do Grupo

| Nome | RM |
|------|----|
| **Emerson Henrique de Lima e Sousa** | 373751 |
| **Moacyr Souza Barros** | 373412 |

---
