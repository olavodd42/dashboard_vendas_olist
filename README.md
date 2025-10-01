\# 📊 Dashboard de Vendas — Olist (Power BI)



Projeto de Business Intelligence desenvolvido em \*\*Power BI\*\* usando o dataset público da \[Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).



\## 🎯 Objetivo

Demonstrar habilidades em:

\- Preparação e modelagem de dados.

\- Construção de modelo estrela (Orders, Customers, Items, Payments, Reviews, Dimensões).

\- Criação de KPIs e storytelling com dashboards executivos.

\- Comunicação de insights de negócio.



\## 🗂️ Dataset

\- Fonte: \[Kaggle Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

\- Período: 2016 a 2018

\- Principais tabelas:

&nbsp; - \*\*Orders\*\* — pedidos e datas.

&nbsp; - \*\*Order Items\*\* — produtos, preço, frete.

&nbsp; - \*\*Payments\*\* — métodos e valores pagos.

&nbsp; - \*\*Customers\*\* — clientes e geografia.

&nbsp; - \*\*Sellers\*\* — vendedores.

&nbsp; - \*\*Reviews\*\* — avaliações.



\## 🏗️ Modelagem

Modelo estrela com as seguintes dimensões e fatos:

\- \*\*dim\_date\*\* — calendário (Ano, Mês, Trimestre, AnoMês).

\- \*\*dim\_customer\*\* — cliente (UF, cidade, first\_purchase).

\- \*\*dim\_payment\_type\*\* — métodos de pagamento.

\- \*\*orders\*\* — pedidos (datas, atraso, tempo\_entrega).

\- \*\*order\_items\_agg\*\* — valores agregados por pedido (itens + frete).

\- \*\*payment\_summary\*\* — agregação de pagamentos por pedido.



!\[Modelo Estrela](docs/model.png) <!-- opcional: adicione print do Model View -->



\## 📈 KPIs implementados

\- \*\*Receita\*\* = soma de preços + frete dos pedidos entregues.

\- \*\*Pedidos\*\* = contagem de pedidos únicos entregues.

\- \*\*Ticket Médio\*\* = Receita ÷ Pedidos.

\- \*\*p50 Entrega (dias)\*\* = Mediana do tempo entre compra e entrega.

\- \*\*p90 Entrega (dias)\*\* = 90% dos pedidos entregues até esse tempo.

\- \*\*% No Prazo\*\* = Pedidos entregues até a data estimada ÷ total.

\- \*\*% Reviews Boas\*\* = Reviews nota ≥ 4 ÷ total.

\- \*\*% Receita por Tipo\*\* = Receita de cada método ÷ receita total.



\## 📊 Principais Visuais

\- \*\*Página 1 — Visão Executiva\*\*

&nbsp; - KPIs de Receita, Pedidos, Ticket Médio, SLA (p50/p90, % No Prazo).

&nbsp; - Evolução mensal de Receita e Pedidos.

&nbsp; - Receita por UF (mapa).

&nbsp; - Receita por método de pagamento.



\## 📂 Arquivos no repositório

\- `/olist\_dashboard.pbix` — arquivo do Power BI.

\- `/docs/olist\_report.pdf` — relatório exportado em PDF.

\- `/README.md` — documentação do projeto.



\## 📌 Resultados

\- Receita total analisada: \*\*~R$ 1 Bi\*\* (2016–2018).

\- SLA global: \*\*91%\*\* dos pedidos entregues no prazo.

\- Ticket Médio: \*\*R$ 15,7 mil\*\*.

\- Método mais usado: \*\*Cartão de Crédito\*\* (>70% da receita).



\## 🚀 Como abrir

1\. Clone este repositório.

2\. Abra `olist\_dashboard.pbix` no \*\*Power BI Desktop\*\*.

3\. Explore os visuais e filtros.



\## 🧑‍💻 Autor

Projeto desenvolvido por \*\*Olavo Dalberto\*\*, como parte do portfólio em \*\*Data Analytics / BI\*\*.



