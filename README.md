# Análise vendas online empresa Contoso
Utilizado a base de dados ContosorRetailDW, é um banco de dados de data warehouse, criado pela Microsoft para demonstração e aprendizado. Ele simula um cenário de varejo, contendo dados de uma empresa fictícia chamada Contoso, que vende produtos em diversas lojas ao redor do mundo.

<br>

## Sobre o Projeto Desenvolvido
Objetivo de monitorar e analisar o desempenho de vendas de uma empresa fictícia, a Contoso. O foco principal foi traduzir dados brutos em insights acionáveis, utilizando o Power BI para construir uma interface intuitiva e interativa.

## Principais Respostas que o Projeto Responde
O dashboard foi construído para responder a perguntas-chave de negócio, como:<br>

- Desempenho Geral: Qual é o nosso faturamento total, margem de lucro e volume de vendas.<br>
- Rentabilidade: Onde está a maior parte da nossa margem de lucro? As vendas online estão sendo lucrativas.<br>
- Vendas e Custo por Período: Como as Vendas Online, Custo de Produtos e Margem Bruta variaram a cada mês.<br>
- Melhores Produtos e Categorias: Quais são os Top 5 Produtos Mais Vendidos e quais categorias de produtos têm a maior receita e margem de lucro.<br>
- Impacto de Promoções: Qual é a diferença no desempenho de vendas em meses com Seasonal Discount versus meses sem desconto (No Discount).<br>
- Detalhes de Vendas: Ao selecionar um mês ou uma categoria, quais são os KPIs de vendas para esse período ou categoria específica, e quais produtos se destacaram.<br>

## Cronograma da Criação do Projeto
O projeto foi dividido em etapas lógicas, desde a modelagem dos dados até a finalização do dashboard interativo.

Etapa de Modelagem de Dados:
- O que foi feito: O relacionamento entre as tabelas de fato (FactOnlineSales) e as tabelas de dimensão (DimProduct, DimCustomer, Dim_Calendario, etc.) foi estabelecido. Uma tabela de calendário (Dim_Calendario) foi criada para facilitar a análise temporal.<br>
 Por que foi feito: Para garantir que os dados de vendas, produtos, clientes e tempo se conectassem corretamente, permitindo análises precisas e a criação de medidas e visuais sem erros.<br>

- Etapa de Criação de Medidas (DAX):
O que foi feito: Foram criadas as medidas-chave para os KPIs, como Vendas Online, Margem Bruta, Quantidade Vendida, Custo Produtos e Valor Médio do Pedido. Também foram criadas medidas de variação percentual anual (YoY) para contextualizar o desempenho.<br>
 Por que foi feito: As medidas transformam os dados brutos em métricas de negócio relevantes, que são a base para a tomada de decisões.<br>

- Etapa de Design e Layout do Dashboard:
O que foi feito: O dashboard foi projetado com um tema escuro e uma paleta de cores vibrantes, mas consistentes (azul para vendas, verde para margem, laranja para custo). O layout foi organizado para que os KPIs principais ficassem no topo, seguidos por gráficos que detalham o desempenho por categoria, promoções e tempo.<br>
 Por que foi feito: Um design limpo e organizado facilita a leitura e a interpretação das informações, tornando a experiência do usuário mais eficiente.<br>

- Etapa de Interatividade e Funcionalidades Avançadas:
O que foi feito: Foram implementados filtros dinâmicos que se escondem através de um menu de botões, e two tooltips personalizadas foram criadas e aplicadas a visuais específicos. A primeira tooltip é um sumário de KPIs com um gráfico temporal, e a segunda é um sumário de KPIs com uma desagregação por categorias.<br>
 Por que foi feito: Essa interatividade permite que o usuário explore os dados de forma aprofundada, respondendo a perguntas específicas sem sobrecarregar a visualização principal.<br>

## Explicação Resumida das para o Portfolio
<img align="right" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Relacionamento%20Tabelas.JPG?raw=true">
Relacionamento das tabelas:  Ela mostra como a tabela central de fatos (FactOnlineSales) está conectada às tabelas de dimensão de produto, cliente e tempo, garantindo a integridade dos dados e o funcionamento correto de todas as análises.<br><br><br><br><br><br>

#


<img align="left" width="100"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Medidas_Criadas.JPG?raw=true">
Criação de medidas DAX: As medidas são fórmulas de cálculo dinâmicas em que os resultados mudam dependendo do contexto. gerando suporte à combinação e filtragem de dados de modelo usando vários atributos
<br><br><br><br><br><br>

#

<img align="right" width="300"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/TabelaCriada_Dimens%C3%A3o_de_Tempo.JPG?raw=true">
Criação da tabela Dim_Calendario: teve como objetivo fundamental centralizar e padronizar todas as informações relacionadas a tempo em um único lugar.

Os principais motivos para a sua criação foram:
Simplificar a Análise Temporal: A tabela fornece colunas pré-calculadas como Ano, Mês, Trimestre e Nome do Mês, o que facilita a criação de gráficos de tendência, como o de Vendas Online | Custo Produtos | Margem Bruta no dashboard principal.
<br><br><br><br><br><br>

#


<img align="left" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Cards.JPG?raw=true">
Os cartões (cards): localizados na parte superior do dashboard têm o objetivo de fornecer um resumo instantâneo e de alto nível do desempenho do negócio. De forma resumida, eles:
- Apresentam os KPIs principais: Exibem o valor total das cinco métricas mais importantes do e-commerce: Vendas Online, Margem Bruta, Quantidade Vendida, Custo Produtos e Valor Médio do Pedido.<br>
- Contextualizam o Desempenho: Além do valor absoluto, a maioria dos cartões inclui a variação percentual anual (YoY), permitindo ao usuário saber rapidamente se o desempenho está crescendo ou diminuindo em relação ao ano anterior.
<br><br><br><br><br><br>

#

<img align="right" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Imagem_01.JPG?raw=true">

- Variação YoY vendas por categoria: Objetivo principal mostrar o crescimento percentual do faturamento de cada categoria de produtos em relação ao mesmo período do ano anterior. Ele permite identificar rapidamente quais categorias estão se expandindo de forma mais acelerada e onde o negócio está obtendo o maior crescimento de vendas ano após ano.<br>

- Categorias: Função de detalhar o desempenho absoluto de cada categoria. Ele mostra, lado a lado, o total de Vendas Online e a Margem Bruta por categoria de produto. O visual é crucial para entender não apenas quais categorias vendem mais, mas também quais são as mais rentáveis, permitindo focar os esforços em produtos com maior margem.<br>

- TOP 5 produtos mais vendidos: Focado em um nível mais granular, identificando os produtos individuais que mais contribuíram para a receita total. Ele lista os cinco produtos com o maior volume de vendas, permitindo que a gestão identifique rapidamente os best-sellers do e-commerce.
<br><br><br><br><br><br>

#

<img align="left" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Imagem_02.JPG?raw=true">

- No Discount | Seasonal Discount: Objetivo de analisar o impacto das promoções nas vendas. Ele compara, mês a mês, o total de vendas realizadas Sem Desconto com as vendas feitas durante uma Promoção Sazonal. Permite identificar o efeito das campanhas promocionais na receita e se elas estão sendo eficazes em impulsionar as vendas.<br>

- Vendas Online | Custo Produtos | Margem Bruta: Mostra a tendência temporal das três métricas financeiras mais importantes do projeto. Ele permite visualizar a evolução mensal de Vendas Online. O objetivo é entender a relação entre essas métricas, como os custos se comportam em relação às vendas e como a margem de lucro varia ao longo do ano.<br>
<br><br><br><br><br><br>

#

<img align="right" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Intera%C3%A7%C3%A3o.JPG?raw=true">

- Filtros de Interação: O dashboard possui um painel de filtros que pode ser exibido ou ocultado, contendo opções de segmentação de dados como Ano - Mês, Categoria do Produto e Promoção (NOME - TIPO).<br>

- Botões de Ação: A funcionalidade de mostrar/esconder o painel de filtros é controlada por botões. O botão de "abrir menu" (ícone de três barras) exibe o painel de filtros, e o botão de "voltar" (ícone de seta) o esconde, mantendo a tela principal limpa e livre de informações desnecessárias.<br>
<br><br><br><br><br><br>

#

<img align="left" width="500"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Contoso%20E-Commerce.JPG?raw=true">

Esta é a visão geral do dashboard final. Ela mostra os principais KPIs de negócio no topo (Vendas Online, Margem Bruta, etc.) e os gráficos que detalham o desempenho por categoria, variação anual, promoções e tendências temporais.<br>
O projeto visa monitorar os principais indicadores de desempenho (KPIs), como Vendas Online, Margem Bruta e Variação YoY, e permitir uma exploração profunda dos dados através de filtros e tooltips personalizadas. A meta final é capacitar a tomada de decisões estratégicas sobre o desempenho de vendas, lucratividade, categorias de produtos e o impacto das promoções.
<br><br><br><br><br><br>

#

# Resumo do Projeto
Este projeto foi desenvolvido com o objetivo de demonstrar habilidades em Business Intelligence, utilizando o Power BI. Todos os dados e análises são baseados no conjunto de dados fictício da Contoso
<br><br><br><br><br><br>

#

# Ferramenta utilizada:
Power BI
