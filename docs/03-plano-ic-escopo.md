# 3. Conexão com o Plano de IC e Definição do Escopo

[← Voltar ao índice](../README.md)

Este projeto tem como objetivo estruturar uma solução de **Business Intelligence** que transforme dados operacionais da empresa em informações estratégicas para tomada de decisão. A proposta consiste na construção de dashboards interativos que possibilitem a análise de desempenho de vendas, comportamento de clientes, lucratividade e sazonalidade, utilizando dados extraídos do sistema ERP.

A abordagem é orientada por indicadores-chave de inteligência (KIQs), garantindo que os painéis desenvolvidos respondam diretamente às principais necessidades do negócio — gerando insights relevantes que apoiem decisões mais assertivas e estratégicas.

## 3.1 KIQs respondidas com dashboards

A partir da análise dos relatórios disponíveis, foram identificadas KIQs precisas, diretamente alinhadas com os dados reais existentes:

1. Quais são os produtos mais vendidos ao longo do ano? *(quantidade vendida e distribuição mensal)*
2. Quais produtos apresentam maior faturamento? *(valor total por período)*
3. Como as vendas se comportam ao longo dos meses? *(análise de sazonalidade)*
4. Qual é o volume médio de vendas por produto?
5. Quais produtos apresentam maior margem de lucro? *(comparação custo × faturamento)*
6. Existe relação entre preço, custo e volume de vendas?
7. Quais são os clientes com maior volume de compras, considerando valor e frequência?
8. Como evoluem as vendas por cliente ao longo do tempo?

### 3.1.1 Fontes de dados

A solução foi construída com base em **três fontes internas** extraídas do ERP, todas em formato CSV:

- Relatório de Análise de Vendas e Custos
- Curva ABC de Venda por Produto
- Análise de Venda por Cliente

### 3.1.2 Relacionamento de métricas e indicadores com os objetivos de negócio

| Objetivo | Métricas | Indicadores |
|---|---|---|
| **Analisar o desempenho de produtos** | Quantidade vendida, faturamento total, preço de custo | Ranking de produtos por volume; Classificação ABC; Margem estimada; Produtos com alto faturamento e baixa rentabilidade; Média mensal por produto; Alta rotatividade vs. esporádicos |
| **Entender o comportamento de clientes** | Volume de compras, número de transações, data da última compra | Ranking de clientes; Clientes mais frequentes; Evolução de compras ao longo do tempo |
| **Identificar padrões e sazonalidade das vendas** | Vendas mensais (jan a dez) | Meses com maior/menor volume; Produtos sazonais; Tendência de crescimento ou queda |

## 3.2 Organização e modelagem de dados

Os dados da base foram organizados em múltiplas abas temáticas no arquivo Excel, permitindo separação lógica e melhor estruturação para análise em BI. A modelagem foi dividida em áreas de negócio: indicadores executivos, clientes, produtos, vendas, custos e consumo via cupom fiscal.

### Estruturas identificadas

| Estrutura | Conteúdo |
|---|---|
| **Resumo Executivo** | Consolidação do faturamento total entre NFe e Cupom Fiscal, indicadores gerais |
| **Clientes NFe** | Vendas por cliente, número de notas, última compra, recência, segmentação, % acumulado |
| **Curva ABC Produtos** | Classificação de produtos por faturamento e quantidade vendida mensal |
| **Vendas e Custos NFe** | Detalhamento financeiro — preço de custo, faturamento, margem bruta e percentual |
| **Consumidor – Cupom Fiscal** | Vendas sem identificação de cliente, categorias, estoque estimado, margem |
| **Ranking de Clientes** | Visão consolidada de NFe + consumidor final |

### Variáveis mapeadas

- Faturamento total
- Quantidade vendida
- Margem bruta e margem percentual
- Segmentação de clientes
- Data de compra
- Participação percentual nas vendas
- Categoria de produtos
- Estoque
- Fornecedor
- Período / mês de venda

### Filtros analíticos

- Tipo de venda (NFe ou Cupom Fiscal)
- Cliente
- Produto
- Categoria
- Fornecedor
- Segmento
- Período
- Curva ABC

A consistência dos dados foi validada a partir da conferência entre faturamento consolidado, totais por aba e distribuição percentual dos indicadores. Foi realizada padronização das estruturas para facilitar integração com a ferramenta de BI.

## 3.3 Planejamento dos dashboards

### KPIs definidos

- Faturamento total
- Faturamento por cliente
- Faturamento por produto
- Margem bruta
- Margem percentual
- Produtos mais vendidos
- Curva ABC de produtos
- Participação percentual dos clientes
- Recência de compra
- Giro e cobertura de estoque
- Comparativo entre vendas NFe e Cupom Fiscal

### Visualizações planejadas

- Cards executivos com KPIs principais
- Gráficos de barras para ranking de clientes e produtos
- Gráficos de linha para evolução mensal das vendas
- Gráficos de pizza ou rosca para participação percentual
- Tabelas analíticas detalhadas
- Heatmaps ou indicadores visuais para estoque e giro
- Curva ABC para priorização comercial

### Filtros interativos

Período, Cliente, Produto, Categoria, Fornecedor, Tipo de venda, Segmento de cliente.

A estrutura proposta atende aos objetivos de inteligência comercial (IC), permitindo identificar oportunidades de vendas, produtos de maior relevância, clientes estratégicos, comportamento de consumo e desempenho financeiro da operação.

## 3.4 Versionamento e controle do projeto

Durante o desenvolvimento da solução foi utilizado o **GitHub** como ferramenta de versionamento e gerenciamento, permitindo controle das alterações, organização colaborativa e rastreabilidade das implementações realizadas.

O repositório contém os arquivos do projeto, estrutura de dados, documentação técnica e histórico de evolução das funcionalidades implementadas.

🔗 **Repositório oficial:** <https://github.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2026-1-pe8-t3-eixo-8-t3-g2>

Benefícios da utilização do GitHub:

- Organização do desenvolvimento em equipe
- Registro histórico das alterações realizadas
- Facilidade de manutenção e evolução
- Compartilhamento centralizado dos arquivos

## 3.5 Início da construção e automação

A construção do dashboard foi iniciada a partir da integração da base de dados estruturada com a ferramenta de Business Intelligence, permitindo automatizar a consolidação das informações comerciais, financeiras e operacionais da empresa.

Foi desenvolvida uma estrutura inicial de navegação com foco em visualização executiva e análise estratégica, centralizando os principais indicadores de desempenho em um painel interativo.

### Primeiras visualizações implementadas

- Indicadores gerais de faturamento
- Comparativo entre vendas NFe (B2B) e Cupom Fiscal (B2C)
- Margem bruta
- Valor total em estoque
- Produtos parados
- Quantidade de SKUs cadastrados
- Produtos com vendas
- Clientes ativos
- Custos totais (CMV)

### Gráficos analíticos criados

- Composição da receita entre NFe e Cupom Fiscal
- Evolução mensal do faturamento por canal de venda
- Indicadores visuais de estoque e desempenho comercial

### Testes iniciais

Durante a construção foram realizados testes de consistência e validação visual:

- Correspondência entre os valores do dashboard e da base original
- Funcionamento correto dos indicadores
- Coerência dos cálculos financeiros
- Distribuição adequada das informações nos gráficos
- Clareza visual para interpretação gerencial

### Insights iniciais identificados

- 📊 **Forte predominância das vendas via Cupom Fiscal (B2C)** em relação às vendas NFe
- 💰 **Alto volume financeiro imobilizado em estoque**
- 📦 Existência de **produtos sem movimentação** no período
- 📅 **Concentração de faturamento** em determinados períodos do ano
- 🎯 Oportunidades de otimização de reposição e gestão de estoque

> Para ver o dashboard completo, consulte a [seção 5 — Dashboard de BI](05-dashboard.md).

---

[← 2. Necessidades de IC](02-necessidades-ic.md) · [Voltar ao índice](../README.md) · [Próximo: 4. PETI →](04-peti.md)
