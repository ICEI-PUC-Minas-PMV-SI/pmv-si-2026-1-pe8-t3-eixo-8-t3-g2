# 4. PETI — Plano Estratégico de Tecnologia da Informação

[← Voltar ao índice](../README.md)

## 4.1 Planejamento estratégico de TI

Esta seção apresenta os principais elementos do planejamento estratégico de TI, incluindo sua finalidade, pontos fortes e limitações, diretrizes, objetivos estratégicos e indicadores de acompanhamento.

### 4.1.1 Finalidade do PETI

O **Plano Estratégico de Tecnologia da Informação (PETI)** tem como finalidade orientar a continuidade e a evolução do uso estratégico da TI na Auto Peças Inconfidentes Ltda, garantindo que os sistemas de informação e a solução de Business Intelligence (BI) desenvolvida no projeto sejam utilizados de forma estruturada para apoiar a tomada de decisão — especialmente na gestão de estoque, vendas e desempenho comercial.

O PETI busca consolidar a transformação dos dados operacionais em informações estratégicas, promovendo maior eficiência, redução de custos e melhoria contínua dos processos organizacionais.

### 4.1.2 Pontos fortes e limitações identificadas

#### ✅ Pontos fortes

- ERP em operação garantindo registro estruturado das transações
- Disponibilidade de dados históricos de vendas, estoque e clientes
- Possibilidade de exportação de dados em formato CSV para análise externa
- Implementação inicial de dashboards de BI com indicadores relevantes
- Melhoria na visibilidade de indicadores como faturamento, margem e giro de estoque

#### ⚠️ Limitações identificadas

- Baixa capacidade analítica nativa do ERP (ausência de dashboards avançados)
- Dependência de exportação manual de dados
- Inconsistências no cadastro de produtos (falta de padronização)
- Ausência de integração automatizada entre ERP e ferramentas de BI
- Falta de análises preditivas e alertas automáticos de estoque
- Baixo uso de indicadores estratégicos na rotina de decisão

### 4.1.3 Diretrizes estratégicas de TI

Para evolução da solução de SI/BI, são propostas as seguintes diretrizes:

| Diretriz | Descrição |
|---|---|
| **Automação da integração de dados** | Pipeline automatizado entre ERP e BI, eliminando processos manuais de exportação |
| **Padronização de cadastros** | Regras de governança de dados para produtos, clientes e categorias |
| **Evolução do BI para análise preditiva** | Uso de histórico de vendas para prever demanda e sazonalidade |
| **Integração com fontes externas** | Inclusão de dados de mercado, preços de concorrentes e tendências do setor |
| **Melhoria na governança de dados** | Criação de dicionário de dados e regras de qualidade |
| **Expansão do uso do sistema** | Disponibilização de dashboards para diferentes áreas (vendas, compras, gestão) |

### 4.1.4 Objetivos estratégicos de TI

#### 🚀 Curto prazo (0 a 6 meses)

- Consolidar e estabilizar os dashboards de BI desenvolvidos
- Melhorar a qualidade dos dados (limpeza e padronização)
- Aumentar a confiabilidade dos indicadores apresentados
- Treinar usuários-chave para utilização dos dashboards

#### 📈 Médio prazo (6 a 12 meses)

- Automatizar a integração entre ERP e BI
- Implementar alertas de estoque e relatórios automatizados
- Expandir dashboards com novos indicadores financeiros e operacionais
- Iniciar uso de análises de tendência e sazonalidade

#### 🎯 Longo prazo (1 a 2 anos)

- Implementar modelos preditivos para reposição de estoque
- Integrar dados externos (mercado e concorrência)
- Evoluir para uma arquitetura de dados centralizada (Data Warehouse)
- Ampliar o uso estratégico da TI em toda a organização

### 4.1.5 Indicadores de acompanhamento

| Indicador | O que mede |
|---|---|
| Número de usuários ativos no BI | Adoção da solução pelos setores |
| Frequência de uso do sistema/dashboards | Engajamento com a ferramenta |
| Redução de perdas operacionais | Estoque parado e rupturas |
| Tempo médio de resposta para decisão | Agilidade gerencial |
| Acurácia das previsões de demanda | Quando modelos preditivos forem implementados |
| % de decisões baseadas em dados | Nível de maturidade analítica |

## 4.2 Auditoria e governança de TI

A Auto Peças Inconfidentes Ltda é uma empresa de pequeno porte e, por isso, não necessita de estruturas complexas de governança de TI. No entanto, é importante adotar **práticas simples** que garantam a segurança das informações, a continuidade das operações e o uso adequado dos sistemas.

### 4.2.1 Segurança e proteção de dados

A empresa armazena informações relacionadas a clientes, fornecedores, produtos e operações comerciais por meio do ERP e dos relatórios utilizados na solução de BI. É necessário garantir que esses dados sejam utilizados apenas para fins relacionados às atividades da empresa.

**Recomendações:**

- Acesso ao sistema controlado por usuário e senha
- Cada colaborador visualiza apenas as informações necessárias para sua função
- Senhas seguras (letras + números + caracteres especiais) com troca periódica
- Evitar compartilhamento de credenciais entre funcionários
- Manter computadores protegidos com antivírus atualizado e bloqueio automático de tela

### 4.2.2 Práticas recomendadas

Para reduzir riscos e garantir maior confiabilidade dos dados:

- Realização de **backup semanal** dos dados do ERP e dos arquivos utilizados no BI
- Armazenamento das cópias em locais confiáveis (Google Drive, OneDrive ou outro serviço seguro de nuvem)
- Verificação periódica da integridade dos arquivos de backup
- Utilização apenas de softwares e ferramentas confiáveis e devidamente licenciados
- Atualização periódica dos sistemas utilizados pela empresa

### 4.2.3 Continuidade e controle

Caso ocorra perda de dados, falha no sistema ou indisponibilidade do ERP, a empresa deve possuir um procedimento simples para recuperação das informações.

**Plano básico de contingência:**

- Manter backups atualizados e armazenados em local seguro
- Definir o responsável pela restauração dos dados em caso de necessidade
- Registrar alterações importantes realizadas no sistema ou nos dashboards do BI
- Manter documentação básica sobre a estrutura dos relatórios e indicadores utilizados

### 4.2.4 Responsabilidades

A manutenção dos relatórios, dashboards e demais recursos tecnológicos deve ser atribuída a um **responsável principal**, preferencialmente um colaborador com conhecimento básico do sistema ERP e da solução de BI.

Recomenda-se a existência de pelo menos um **responsável secundário** com acesso administrativo, garantindo continuidade em casos de férias, afastamentos e desligamentos.

**Responsabilidades definidas:**

- Monitorar a atualização dos dados
- Verificar a realização dos backups
- Controlar permissões de acesso aos sistemas
- Apoiar usuários na utilização dos dashboards e relatórios
- Registrar eventuais problemas e melhorias identificadas

### 4.2.5 Governança simplificada

A governança de TI da empresa deve ser baseada em regras simples e de fácil aplicação:

- Definir regras básicas de utilização do ERP e dos dashboards de BI
- Criar um manual simplificado ou vídeo demonstrativo para treinamento de novos colaboradores
- Padronizar procedimentos para exportação, atualização e análise dos dados
- Realizar avaliações periódicas para verificar se os dashboards e indicadores continuam atendendo às necessidades do negócio
- Revisar, pelo menos semestralmente, os indicadores utilizados na gestão de estoque, vendas e desempenho comercial
- Realizar auditorias simplificadas e periódicas — verificando permissões de acesso, realização dos backups, integridade dos dados exportados, atualização dos dashboards e registro de inconsistências identificadas nos relatórios

Com essas práticas, a empresa poderá manter a organização dos seus dados, aumentar a confiabilidade das informações, reduzir riscos operacionais e garantir que a tecnologia continue apoiando a tomada de decisão de forma eficiente e alinhada aos objetivos do negócio.

---

[← 3. Plano de IC](03-plano-ic-escopo.md) · [Voltar ao índice](../README.md) · [Próximo: 5. Dashboard →](05-dashboard.md)
