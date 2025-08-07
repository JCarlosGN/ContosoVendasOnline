# Análise vendas online empresa Contoso
Utilizado a base de dados ContosoretailDW, é um banco de dados de data warehouse de exemplo, criado pela Microsoft para demonstração e aprendizado. Ele simula um cenário de varejo, contendo dados de uma empresa fictícia chamada Contoso, que vende produtos em diversas lojas ao redor do mundo.

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
Relacionamento das tabelas:  Ela mostra como a tabela central de fatos (FactOnlineSales) está conectada às tabelas de dimensão de produto, cliente e tempo, garantindo a integridade dos dados e o funcionamento correto de todas as análises.<br><br>
<br><br>



<img align="left" width="200"  src="https://github.com/JCarlosGN/ContosoVendasOnline/blob/main/Imagens/Medidas_Criadas.JPG?raw=true">
Criação de medidas DAX: As medidas são fórmulas de cálculo dinâmicas em que os resultados mudam dependendo do contexto. gerando suporte à combinação e filtragem de dados de modelo usando vários atributos

# Ferramenta utilizada:
Power BI
<br>

##
