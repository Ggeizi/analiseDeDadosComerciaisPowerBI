# Relatório de Vendas Anual — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-01B8AA?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-376C60?style=for-the-badge)

Dashboard interativo de **análise de vendas anuais** de uma rede de varejo de moda, desenvolvido no **Power BI**. O relatório acompanha faturamento, lucro e desempenho por marca, tipo de produto e período, transformando a base de vendas em indicadores prontos para apoiar decisões.

>  Projeto de estudo desenvolvido com base em uma base de dados fictícia, para praticar tratamento de dados, modelagem, medidas DAX e visualização no Power BI.

---

## Perguntas de negócio

O dashboard foi construído para responder:

- Qual o **faturamento** e o **lucro** total no período?
- Quais **marcas** mais faturam e qual a participação de cada uma?
- Quais **tipos de produto** têm maior presença nas vendas?
- Como o desempenho se comporta ao longo do **período (2013–2014)**?

## Sobre os dados

- **Fonte:** base de vendas (dados fictícios para fins de estudo).
- **Tabela `Vendas`** com ~720 registros e os campos: `SKU`, `Dia`, `Mês`, `Ano`, `Tipo`, `Marca`, `Faturamento` e `Lucro`.
- **Período analisado:** 2013 a 2014.

## O que foi feito

- **Tratamento e limpeza** dos dados no **Power Query** (ajuste de tipos, datas e padronização).
- Criação de **medidas DAX** para os principais indicadores.
- Construção de **visuais interativos**: cartões de KPI, gráfico de rosca (faturamento por marca), gráfico de pizza (por tipo de produto) e gráfico de funil (ranking de marcas).
- **Segmentações (slicers)** por período (intervalo de datas) e por tipo de produto, permitindo análise dinâmica.
- Aplicação de **tema escuro** e organização do layout para facilitar a leitura.

### Exemplos de medidas (DAX)

```dax
Soma de Faturamento = SUM( Vendas[Faturamento] )

Soma de Lucro = SUM( Vendas[Lucro] )

Margem de Lucro % = DIVIDE( [Soma de Lucro], [Soma de Faturamento] )
```

## Visão geral do dashboard

![Dashboard de Vendas Anual](./assets/dashboard.png)

## Principais insights

- **Faturamento total de ~R$ 57,24 mil** e **lucro de ~R$ 25,07 mil** no período — uma **margem de lucro de aproximadamente 44%**.
- A marca **Reserva lidera o faturamento (~48%)**, seguida por **Hashtag (~28%)** e **Osklen (~23%)**.
- O mix de produtos é diversificado, com destaque para **camisas, casacos e camisetas** entre os tipos mais presentes.
- Os filtros de período e de tipo permitem isolar rapidamente o desempenho de cada marca ou categoria.

## Estrutura do repositório

```
.
├── Relatorio_Vendas_Anual.pbix   # arquivo do Power BI
├── assets/
│   └── dashboard.png             # print do relatório
└── README.md
```

## Como visualizar

1. Baixe o arquivo `Relatorio_Vendas_Anual.pbix`.
2. Abra no **[Power BI Desktop](https://www.microsoft.com/pt-br/power-platform/products/power-bi/desktop)** (gratuito).
3. Para uma prévia rápida, veja a imagem na pasta `assets/`.

---
**Geiziane Rocha** — Estudante de Engenharia de Software | Desenvolvedora & Análise de Dados/BI

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/geizi)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:geizirocha586@gmail.com)
