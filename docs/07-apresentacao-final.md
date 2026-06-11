# 7. Apresentação Final

[← Voltar ao índice](../README.md)

Resumo dos slides da apresentação final do projeto.

> 📥 **Arquivo original (PPTX):** [apresentacao-final.pptx](assets/apresentacao-final.pptx)

---

## Slide 1 — Abertura

**Análise do Sistema de Informação e Proposta de Solução Baseada em Dados**

*Gestão de Estoque em Empresa de Autopeças*

PUC Minas — Sistemas de Informação · Grupo 2 — 2026

**Integrantes:** Gabriel Alves Aredes Moraes · Gabriel Alves Rodrigues · Guilherme Martins Fialho · Jean Gabriel da Silva Lima · Lívia Santos Morais · Vinicius Menezes Gomes

---

## Slide 2 — Auto Peças Inconfidentes Ltda

**Fundada em 1988 · Contagem/MG · 40+ anos de mercado**

Comércio varejista físico e online com diferencial em **atendimento personalizado** e relacionamento próximo com o cliente.

**Contexto de mercado:**

- Alta demanda por manutenção automotiva na região
- Forte concorrência regional e expansão de marketplaces
- Crescente pressão competitiva do comércio online

---

## Slide 3 — O Problema e o Sistema Atual

| Limitação | Impacto |
|---|---|
| **ERP G-Tech** focado em controle básico, cadastro e fiscal — sem capacidade analítica | Sem visão estratégica |
| **Gestão por intuição** | Decisões sem suporte de dados objetivos |
| **Relatórios limitados** | ERP não gera visões estratégicas nem análises de desempenho |
| **Estoque parado** | Alto risco de capital imobilizado em produtos sem giro |

---

## Slide 4 — Objetivo do Projeto

> Desenvolver uma solução de **Business Intelligence** que transforme os dados existentes em **inteligência acionável** para a gestão de estoque.

| Frente | Entrega |
|---|---|
| **Solução de BI** | Plataforma de análise de dados integrada ao ERP existente |
| **Reposição inteligente** | Processos baseados em dados históricos e padrões de venda |
| **Dashboards gerenciais** | Painéis intuitivos e interativos para apoio à decisão |
| **Decisões estratégicas** | Liderança apoiada por dados confiáveis, atualizados e visuais |

---

## Slide 5 — Decisão Estratégica e Oportunidades

**Foco central:** maximizar vendas, reduzir perdas operacionais e otimizar o capital de giro — utilizando os dados já disponíveis no ERP.

| Oportunidade | Ação |
|---|---|
| **Definir critérios de reposição** | Regras claras baseadas em giro, sazonalidade e margem |
| **Reduzir estoque inativo** | Identificar e eliminar produtos sem movimentação que imobilizam capital |
| **Antecipar demanda** | Usar padrões históricos para planejar compras com maior precisão |

---

## Slide 6 — KPIs, KITs e KIQs

Indicadores estruturados em **três dimensões analíticas** para cobrir comportamento de vendas, produtos estratégicos e qualidade da informação.

| | |
|---|---|
| **4** KPIs principais | Giro de estoque, tempo médio em estoque, volume de vendas e margem de lucro por produto |
| **3** dimensões de análise | Comportamento de vendas, produtos mais vendidos e itens com maior giro sazonal |
| **12+** meses históricos | Base para análise de sazonalidade e tendências de consumo |

**Detalhamento dos KPIs:**

- **Giro de Estoque** — velocidade de venda dos produtos armazenados
- **Tempo Médio em Estoque** — dias médios que um item permanece sem venda
- **Volume de Vendas** — quantidade vendida por período e categoria
- **Margem de Lucro** — rentabilidade real por produto e linha

---

## Slide 7 — Estrutura de Dados e Qualidade

**Fontes de dados:** relatórios CSV extraídos do ERP G-Tech, abrangendo vendas, estoque e cadastro de clientes.

**Etapas de tratamento:**

1. **Limpeza de dados** — correção de inconsistências, duplicidades e campos incompletos
2. **Padronização** — unificação de nomenclaturas de produtos e categorias
3. **Curva ABC** — classificação dos itens por relevância (A = alto impacto, C = baixo giro)

---

## Slide 8 — Funcionalidades do Dashboard de BI

| Funcionalidade | Descrição |
|---|---|
| **Filtros dinâmicos** | Navegação interativa por período, categoria e fornecedor |
| **Indicação visual** | Itens sem movimentação e outros problemas sinalizados |
| **Curva ABC** | Visualizações avançadas para identificar padrões de concentração de vendas |
| **Cards executivos** | Visão consolidada dos principais indicadores com gráficos comparativos |

---

## Slide 9 — Segurança, Compliance e LGPD

O projeto garante **conformidade total com a LGPD**, assegurando que todos os dados de clientes e operações sejam tratados com transparência e responsabilidade.

| Pilar | Medida |
|---|---|
| **Controle de Acesso** | Permissões por perfil de usuário com rastreabilidade de ações |
| **Backups Periódicos** | Rotinas automatizadas de backup para garantir continuidade |
| **Proteção de Dados Sensíveis** | Mascaramento e criptografia de informações críticas de clientes e fornecedores |

---

## Slide 10 — Resultados e Conclusão

### Resultados iniciais observados

- **Predominância B2C** — Identificação clara do perfil de cliente majoritário e seus padrões de compra
- **Estoque parado mapeado** — Produtos sem movimentação identificados e prontos para ação corretiva
- **Sazonalidade detectada** — Padrões sazonais revelados, permitindo planejamento antecipado de compras

### Impacto esperado

- Redução drástica de estoque parado e capital imobilizado
- Melhor planejamento de compras com base em dados históricos
- Maior disponibilidade dos produtos certos no momento certo
- Base sólida para expansão e crescimento sustentável

> 💡 O BI transforma dados brutos em **decisões estratégicas**, gerando eficiência operacional e competitividade real.

---

[← 6. Dashboard](06-dashboard.md) · [Voltar ao índice](../README.md) · [Próximo: Referências →](referencias.md)
