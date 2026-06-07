# 2. Identificação, Análise e Estruturação das Necessidades de IC

[← Voltar ao índice](../README.md)

## 2.1 Mapeamento das decisões estratégicas

A partir da análise do contexto operacional e de mercado da Auto Peças Inconfidentes Ltda, foram identificadas decisões estratégicas que impactam diretamente a competitividade e a sustentabilidade da empresa. Para maior clareza, essas decisões foram agrupadas em quatro áreas principais:

### Gestão de Estoque
A empresa precisa decidir quais produtos devem ser mantidos, ampliados ou retirados do estoque, considerando a rotatividade, demanda e espaço físico disponível.

> **Exemplo prático:** se uma peça de freio tem alta saída em março e abril devido à manutenção preventiva de veículos, é estratégico aumentar a reposição nesse período. Por outro lado, produtos com baixa demanda devem ser avaliados antes de ocupar espaço de estoque.

### Vendas e Preços
Definir preços competitivos e escolher os canais de venda mais vantajosos é fundamental para manter a margem de lucro e atrair clientes.

> **Exemplo prático:** comparar preços praticados por concorrentes locais e online para peças comuns, como filtros de óleo, e decidir se vale a pena ofertar promoções na loja física ou em marketplaces.

### Clientes e Relacionamento
Estratégias para fidelizar clientes e fortalecer relacionamentos com oficinas mecânicas são essenciais para manter a confiança e garantir vendas recorrentes.

> **Exemplo prático:** oferecer condições especiais para oficinas que compram regularmente, criar programas de desconto ou cadastro de clientes frequentes para envio de novidades e promoções.

### Fornecedores e Condições de Compra
Avaliar fornecedores e condições de compra ajuda a reduzir custos e evitar rupturas no estoque.

> **Exemplo prático:** negociar prazos de entrega e descontos com fornecedores de peças de alta rotatividade ou buscar alternativas para produtos com atrasos frequentes.

### 2.1.1 Definição da decisão-chave

Dentre as decisões estratégicas, a empresa definiu como prioridade a **gestão de estoque**:

> 🎯 **Decisão-Chave:** "Estabelecer critérios claros para reposição de produtos no estoque, determinando quais itens devem ser mantidos, em qual quantidade e em que momento, de forma a maximizar vendas, reduzir perdas e garantir o capital de giro eficiente."

Essa decisão foca na melhoria da gestão de estoque, atualmente baseada principalmente na experiência dos vendedores, sem uso estruturado de dados.

### 2.1.2 Definição do KIT (Key Intelligence Topic)

> 🧠 **KIT:** Análise do comportamento de vendas e giro de estoque para otimização da reposição de produtos.

### 2.1.3 Formulação das KIQs (Key Intelligence Questions)

1. Quais são os produtos mais vendidos em determinado período?
2. Quais produtos apresentam maior frequência de venda (giro alto)?
3. Quais produtos permanecem mais tempo em estoque sem venda?
4. Existe sazonalidade na venda de determinados produtos?
5. Qual é o volume médio de vendas por produto ao longo do tempo?
6. Quais produtos geram maior faturamento para a empresa?
7. Há produtos que ocupam espaço no estoque, mas possuem baixa saída?
8. Qual é o tempo médio entre a entrada e a venda de um produto?
9. Existe relação entre preço e volume de vendas?
10. Quais categorias de produtos apresentam melhor desempenho?

### 2.1.4 Justificativa da relevância do KIT e das KIQs

O KIT está diretamente ligado à eficiência da gestão de estoque, um dos principais fatores de sucesso no setor de autopeças. A ausência de análises estruturadas pode levar a:

- Excesso de estoque e capital parado
- Falta de produtos com alta demanda
- Perda de vendas por ruptura

Com as KIQs respondidas, a empresa poderá:

- Reduzir custos com estoque parado
- Melhorar o planejamento de compras
- Aumentar a disponibilidade de produtos com alta demanda
- Otimizar o uso do capital de giro
- Apoiar decisões estratégicas com base em dados concretos

## 2.2 Mapeamento de dados e identificação das necessidades de informação

### 2.2.1 Mapeamento das informações necessárias

| KIQ | Dados necessários | Classificação | Fonte |
|---|---|---|---|
| Produtos mais vendidos no período | Código do produto, qtd. vendida, data da venda | Desempenho operacional | ERP |
| Produtos com maior frequência de venda | Histórico de vendas, qtd. vendida, datas | Desempenho operacional | ERP |
| Produtos parados no estoque | Data de entrada, data da última venda | Controle de estoque | ERP |
| Sazonalidade nas vendas | Datas e qtd. vendida por período | Análise temporal | ERP |
| Volume médio de vendas por produto | Qtd. vendida por período, histórico | Desempenho operacional | ERP |
| Produtos de maior faturamento | Valor de venda, qtd. vendida, produto | Financeiro | ERP |
| Produtos com baixa saída ocupando estoque | Qtd. em estoque, data de entrada, última venda | Controle de estoque | ERP |
| Tempo médio entre entrada e venda | Data de entrada, data de saída/venda | Eficiência operacional | ERP |
| Relação preço × volume | Preço, qtd. vendida, histórico | Análise de mercado | ERP |
| Desempenho por categoria | Categoria, qtd. vendida, faturamento | Por categoria | ERP |

### 2.2.2 Priorização das informações

Foram priorizadas as informações mais diretamente ligadas ao desempenho do estoque e ao impacto nos resultados:

- Volume de vendas por produto
- Giro de estoque
- Tempo de permanência no estoque
- Produtos com baixa rotatividade
- Produtos com maior impacto no faturamento

### 2.2.3 Fontes de dados

Fontes internas — todas do ERP:

- Registros de vendas (produto, quantidade, valor e data)
- Movimentações de estoque (entradas e saídas)
- Cadastro de produtos (código, descrição e categoria)
- Informações de preços

### 2.2.4 Avaliação da disponibilidade e confiabilidade

| Aspecto | Avaliação |
|---|---|
| Disponibilidade | ✅ Boa — dados gerados continuamente pelas operações |
| Confiabilidade | ⚠️ Afetada por erros de cadastro, registros manuais incorretos e falta de padronização |
| Limitação típica | Mesmo produto cadastrado com nomes diferentes dificulta análise consolidada |

Mesmo com essas limitações, os dados são adequados para o estudo desde que passem por **organização e validação** antes da análise.

## 2.3 Especificação de requisitos informacionais

### 2.3.1 Requisitos informacionais

O sistema de informação deverá transformar os dados operacionais em informações estratégicas que apoiem a decisão de reposição de estoque. Principais requisitos:

- Produtos mais vendidos por período
- Produtos com maior e menor giro de estoque
- Tempo médio de permanência dos produtos no estoque
- Volume de vendas por produto
- Faturamento por produto e por categoria
- Identificação de produtos com alta quantidade em estoque e baixa saída

### 2.3.2 Indicadores-chave (KPIs)

| KPI | O que mede |
|---|---|
| **Giro de estoque** | Frequência de venda dos produtos em determinado período |
| **Tempo médio em estoque** | Quantos dias um item permanece sem venda |
| **Volume de vendas** | Base para decisões de reposição de produtos |
| **Faturamento por produto** | Itens com maior impacto financeiro |

### 2.3.3 Funcionalidades da solução

- Dashboards gerenciais com visão geral de vendas e estoque
- Relatórios analíticos por produto, categoria e período
- Filtros dinâmicos (data, produto, categoria)
- Alertas para estoque baixo e produtos sem saída

### 2.3.4 Justificativa

A definição dos requisitos e KPIs está diretamente relacionada à necessidade da empresa de tornar a gestão de estoque mais eficiente e baseada em dados. Atualmente, muitas decisões são tomadas com base na experiência, o que pode gerar falhas como excesso ou falta de produtos. Com a solução proposta, a empresa poderá identificar padrões de venda, reduzir estoque parado, melhorar o planejamento de compras e aumentar a disponibilidade dos itens de maior demanda.

## 2.4 Levantamento de fontes de dados existentes

### 2.4.1 Objetivo

Identificar os dados disponíveis atualmente na empresa que podem alimentar a solução proposta, garantindo a viabilidade do projeto e a integração com o sistema de Business Intelligence (BI) a ser desenvolvido.

### 2.4.2 Inventário de dados disponíveis

| Base / Relatório | Formato | Tipo de dados | Responsável |
|---|---|---|---|
| Curva ABC de vendas por produto | CSV | Produto, volume de vendas, classificação ABC | Sistema ERP |
| Análise de vendas por cliente | CSV | Cliente, produtos comprados, volume e frequência | Sistema ERP |
| Análise de venda e custo | CSV | Produto, preço de venda, custo, margem | Sistema ERP |
| Relatório de estoque | CSV | Produto, quantidade em estoque, movimentações | Sistema ERP |

### 2.4.3 Avaliação da estrutura e qualidade dos dados

**Pontos positivos:**
- Dados estruturados em formato CSV (importação e análise facilitadas)
- Informações diretamente relacionadas às operações
- Atualização frequente (geradas pelas vendas/movimentações diárias)

**Pontos de atenção:**
- Possível inconsistência no cadastro de produtos (nomes diferentes para o mesmo item)
- Falta de padronização em alguns campos
- Dependência de exportação manual
- Ausência de integração automática entre os dados

### 2.4.4 Avaliação da prontidão dos dados para uso

Os dados disponíveis **não estão totalmente prontos** para uso direto. Etapas necessárias:

1. Limpeza de dados (remoção de duplicidades e inconsistências)
2. Padronização de nomes e categorias de produtos
3. Organização em modelo estruturado (tabelas relacionais ou data warehouse)
4. Integração entre diferentes relatórios

### 2.4.5 Lacunas identificadas

- Ausência de dados detalhados sobre tempo de permanência em estoque
- Falta de histórico consolidado em uma única base
- Ausência de dados externos (preços de concorrentes, tendências de mercado)
- Falta de identificação clara de sazonalidade estruturada

**Recomendações futuras:**
- Implementar coleta automatizada de dados do ERP
- Padronizar o cadastro de produtos
- Avaliar integração com fontes externas de mercado

### 2.4.6 Conclusão do levantamento

A empresa já possui uma base relevante de dados capaz de sustentar a implementação inicial da solução de BI. Para alcançar maior maturidade analítica, será necessário investir em **organização, integração e padronização** dos dados — transformando dados operacionais em informações estratégicas para fortalecer a tomada de decisão.

## 2.5 Compliance de TI e segurança da informação

### 2.5.1 Mapeamento de requisitos regulatórios

| Norma | Escopo |
|---|---|
| **LGPD** (Lei 13.709/2018) | Diretrizes para coleta, tratamento e armazenamento de dados pessoais |
| **GDPR** | Referência internacional para boas práticas de proteção de dados |
| **ISO 27001** | Gestão da segurança da informação |

### 2.5.2 Políticas de segurança da informação

- Controle de acesso aos dados com base no perfil do usuário
- Definição de níveis de permissão conforme função
- Uso de senhas seguras e mecanismos de autenticação
- Armazenamento seguro das informações
- Realização de backups periódicos

### 2.5.3 Diretrizes para proteção de dados

- Utilização de dados anonimizados sempre que possível
- Limitação do uso de dados pessoais ao necessário
- Restrição de acesso a informações sensíveis
- Não compartilhamento de dados sem autorização

### 2.5.4 Monitoramento e conformidade

- Registro de acessos aos sistemas (logs)
- Auditorias periódicas
- Revisão de permissões de usuários
- Atualização das políticas de segurança
- Orientação básica aos usuários sobre boas práticas

---

[← 1. Introdução](01-introducao.md) · [Voltar ao índice](../README.md) · [Próximo: 3. Plano de IC →](03-plano-ic-escopo.md)
