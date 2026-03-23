📊 Dashboard de Performance: Marketplace de Produtos (Olist)

📌 Sobre o Projeto
Este projeto apresenta uma análise profunda de performance de vendas de um marketplace, utilizando o dataset público da Olist. O objetivo foi transformar dados brutos de e-commerce em insights estratégicos para gestão de faturamento, logística e comportamento do consumidor.

O grande diferencial deste trabalho foi a resolução de inconsistências críticas de dados (ETL) e a modelagem estruturada para permitir análises temporais precisas de 2016 a 2018.

🛠️ Tecnologias e Ferramentas
Power BI: Visualização de dados e criação de dashboards interativos.

DAX (Data Analysis Expressions): Criação de medidas de inteligência de tempo e KPIs complexos.

SQL: Extração e manipulação prévia dos dados para análise.

Power Query: Processo de ETL (Extração, Transformação e Carga) e limpeza de dados.

🏗️ Desafios Técnicos & Soluções (O "Pulo do Gato")
Durante o desenvolvimento, identifiquei que o Power BI não reconhecia os dados de 2016 e parte de 2017 devido ao formato internacional dos arquivos CSV.

Tratamento de Dados (ETL): Utilizei a técnica de Alterar Tipo por Localidade (Inglês EUA) no Power Query para converter os timestamps corretamente. Sem isso, o faturamento estaria subestimado em milhões.

Modelagem Star Schema: Implementei uma tabela Calendário customizada via DAX para conectar as tabelas de pedidos e itens, permitindo filtros de data consistentes em todo o relatório.

Limpeza de Dados: Apliquei filtros e substituições para remover erros de valores vazios (nulls) que distorciam o Ticket Médio.

📈 Principais Indicadores (KPIs)
Faturamento Total: Visualização clara do montante de R$ 13,59 Milhões.

Evolução Mensal: Gráfico de áreas mostrando o crescimento histórico e picos de vendas (Black Friday).

Ticket Médio por Estado: Identificação de regiões com maior valor de compra por pedido.

Ranking de Categorias: Visão detalhada de quais produtos (Equipamentos, Beleza, Relógios) trazem mais receita.

📂 Estrutura do Repositório
Projeto_Analise_de_E-Commerce.pbix: Arquivo fonte do Power BI.

Projeto_Analise_de_E-Commerce.sql: Scripts utilizados para extração/tratamento no banco de dados.

Apresentação PowerBI.png: Screenshot do dashboard finalizado.

README.md: Documentação completa do projeto.

👨‍🎓 Conclusão


Este projeto foi uma excelente oportunidade para aplicar técnicas avançadas de BI. A maior lição foi entender que um gráfico bonito não serve para nada se os dados por trás não forem confiáveis. A correção das datas foi o que transformou um erro técnico em uma análise de negócio real de 3 anos de história.
