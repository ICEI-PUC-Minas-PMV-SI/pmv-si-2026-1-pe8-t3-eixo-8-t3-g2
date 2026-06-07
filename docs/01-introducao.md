# 1. Introdução

[← Voltar ao índice](README.md)

## 1.1 Apresentação da empresa

A empresa escolhida para o desenvolvimento do projeto é a **Auto Peças Inconfidentes Ltda**, que atua no segmento de comércio varejista de peças e acessórios para veículos automotores. A empresa foi fundada em **1988** e possui sua sede localizada na Avenida Juscelino Kubitschek, nº 402, no bairro Industrial, em **Contagem**, região metropolitana de Belo Horizonte, Minas Gerais. Sua atividade principal é a comercialização de peças automotivas novas, destinadas principalmente à linha leve e utilitários.

A empresa atua há mais de três décadas no mercado de autopeças, oferecendo uma grande variedade de produtos e trabalhando com marcas originais e de reposição. Além da venda presencial, também possui presença digital por meio de loja virtual, permitindo que clientes realizem compras de forma prática e segura. O negócio busca oferecer atendimento especializado e manter um estoque diversificado para atender às diferentes necessidades dos clientes.

A escolha da empresa para o desenvolvimento deste trabalho se justifica pelo fato de ela atuar em um segmento com grande volume de produtos, vendas e relacionamento com clientes, o que gera diversos tipos de dados importantes para análise. Empresas do setor de autopeças frequentemente utilizam sistemas simples para controle de estoque, vendas e clientes, o que abre oportunidades para a aplicação de sistemas de informação, dashboards e análises de dados que possam melhorar a gestão e apoiar a tomada de decisões.

Por ser uma empresa de pequeno porte, o entendimento de seus processos de negócio é facilitado, possibilitando identificar oportunidades de melhoria por meio da implementação ou aprimoramento de sistemas de informação.

## 1.2 Análise de mercado

A Auto Peças Inconfidentes Ltda atua no setor de comércio de autopeças, vendendo produtos utilizados na manutenção e revisão de veículos. Esse mercado possui **demanda constante**, já que veículos precisam de manutenção periódica e substituição de peças ao longo do tempo. Itens relacionados à parte mecânica e revisões gerais costumam ter boa demanda, principalmente em regiões com grande circulação de veículos.

Em Contagem, na região metropolitana de Belo Horizonte, existe um grande número de veículos e oficinas mecânicas, o que gera demanda para lojas de autopeças. Ao mesmo tempo, essa realidade aumenta a concorrência, já que diversas empresas do mesmo segmento atuam na região.

Entre os principais concorrentes da empresa estão outras lojas de autopeças da região e vendedores online. Muitas dessas empresas conseguem oferecer preços mais baixos porque compram em maior quantidade diretamente dos fornecedores. Além disso, atualmente os clientes conseguem comparar preços com facilidade pela internet, o que faz com que o preço se torne um fator muito relevante na decisão de compra.

Mesmo diante dessa concorrência, a Auto Peças Inconfidentes Ltda busca se diferenciar principalmente pelo **atendimento ao cliente**. Por ser uma empresa menor e com muitos anos de atuação no mercado, foi construída uma relação de confiança com diversos clientes e oficinas da região. Esse tipo de atendimento mais próximo contribui para a fidelização.

Outro ponto importante no setor é o crescimento das vendas online. Embora a empresa possua cadastro em plataformas e redes sociais, as altas taxas cobradas acabam reduzindo significativamente as margens de lucro, tornando o atendimento direto ao cliente na loja física mais vantajoso.

### Matriz SWOT

| Forças (S) | Fraquezas (W) |
|---|---|
| Mais de 30 anos de mercado e marca consolidada | ERP com baixa capacidade analítica (sem dashboards) |
| Relacionamento próximo com clientes e oficinas | Decisões de reposição baseadas em intuição/experiência |
| Mix diversificado de produtos (originais e reposição) | Cadastro de produtos com inconsistências |
| Presença em loja física + e-commerce | Dependência de exportação manual de dados |
| **Oportunidades (O)** | **Ameaças (T)** |
| Uso de BI para decisões data-driven | Forte concorrência regional (lojas locais e online) |
| Padronização de cadastros e governança de dados | Marketplaces com altas taxas reduzindo margem |
| Integração automatizada ERP ↔ BI | Pressão de preço de grandes redes/atacadistas |
| Análises preditivas de demanda e sazonalidade | Migração de clientes para canais digitais |

## 1.3 Análise de processos e sistemas

### 1.3.1 Processos e fluxo de informações

A empresa realiza suas atividades comerciais principalmente por meio de **vendas diretas no balcão**. O fluxo operacional inicia quando o cliente chega ao estabelecimento e solicita uma peça automotiva específica para seu veículo. Nesse momento, o vendedor realiza a consulta no sistema de gestão empresarial para verificar a disponibilidade do produto em estoque.

Caso o item esteja disponível, o vendedor informa o preço e procede com a separação. Em algumas situações, o cliente verifica fisicamente o produto antes da conclusão da compra, para confirmar compatibilidade com o veículo. Após o pagamento (cartão de crédito, débito, PIX ou dinheiro), a venda é registrada no sistema, que automaticamente atualiza o estoque e armazena as informações da transação.

Além do processo de venda, a empresa realiza um acompanhamento constante do nível de estoque dos produtos. Durante o atendimento ou em momentos de verificação interna, os vendedores observam quais itens apresentam níveis reduzidos ou estão esgotados. A decisão de realizar novas compras considera fatores como a **frequência de venda**, a **demanda dos clientes** e a **relevância do produto no portfólio**. Itens de alta rotatividade tendem a ser repostos com maior prioridade, enquanto produtos com baixa demanda podem deixar de ser adquiridos novamente.

#### Diagrama BPMN — Processo de venda de peças

> Atendimento → Consulta ao ERP → Disponibilidade? → Informa preço / Separação / Verificação física → Pagamento → Registro da venda → Atualização automática do estoque.

### 1.3.2 Sistema de informação existente e oportunidades de melhoria

A empresa utiliza um sistema de gestão fornecido pela **G-Tech Sistemas**, que funciona como ERP — responsável por integrar e registrar diversas atividades operacionais:

- Controle de estoque
- Registro de vendas
- Cadastro de produtos e fornecedores
- Emissão de documentos fiscais eletrônicos (NFe)

**Limitações identificadas:**

- Relatórios disponíveis são restritos e oferecem poucas possibilidades de análise aprofundada.
- Ausência de dashboards ou painéis visuais.
- Dificuldade para visualizar rapidamente indicadores como desempenho de vendas, giro de estoque ou lucratividade por categoria.

**Oportunidade:** o ERP possibilita a geração de relatórios operacionais que podem ser exportados em **formato CSV**. Esse recurso permite extrair os dados para tratamento e análise em ferramentas externas (planilhas eletrônicas ou plataformas de BI), abrindo espaço para construir indicadores de desempenho que apoiem a tomada de decisão sobre reposição de mercadorias.

### 1.3.3 Avaliação da maturidade do sistema de informação

O sistema atual pode ser classificado como **adequado para o suporte das atividades operacionais básicas**:

- Registro de vendas, atualização automática do estoque, emissão de NFe e armazenamento de histórico funcionam bem.
- Integração com a Secretaria da Fazenda para documentos fiscais eletrônicos.
- Informações registradas podem ser utilizadas pelo setor contábil.

Entretanto, a maturidade em relação ao **suporte à gestão estratégica** ainda é limitada. A ausência de recursos avançados de análise de dados, visualização de indicadores e geração de relatórios gerenciais detalhados restringe o potencial de utilização das informações disponíveis.

### 1.3.4 Levantamento de informações técnicas do sistema

Dados armazenados no banco do ERP:

- Cadastro de produtos e peças automotivas
- Controle de estoque e movimentação de mercadorias
- Registro das vendas realizadas
- Cadastro de clientes e fornecedores
- Informações fiscais utilizadas para emissão de documentos eletrônicos

> Informações técnicas mais específicas (linguagens, SGBD, APIs de integração) foram solicitadas à empresa desenvolvedora do software e, no momento da elaboração deste trabalho, ainda aguardavam retorno.

Quanto às funcionalidades de análise, o sistema disponibiliza relatórios operacionais relacionados a vendas e movimentação de estoque, com limitações em relação à geração de indicadores gerenciais e visualizações gráficas mais avançadas.

---

[← Voltar ao índice](README.md) · [Próximo: 2. Necessidades de IC →](02-necessidades-ic.md)
