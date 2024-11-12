
# Projeto de Extração e Inserção de Dados da Receita Federal

Este projeto realiza a extração de dados públicos da Receita Federal a partir de arquivos CSV, seu tratamento e inserção no banco de dados PostgreSQL. O objetivo é automatizar o carregamento massivo dos dados extraídos para análises e relatórios.

[Arquivos da Receita Federal](https://arquivos.receitafederal.gov.br/cnpj/dados_abertos_cnpj/2024-10/)


## Estrutura do Projeto

### 1. Web Scraping
O processo de web scraping coleta dados sobre estabelecimentos comerciais, empresas, CNAEs e outros itens especificados no dicionário de dados da Receita Federal. Para entender as informações e os campos coletados, consulte o [Dicionário de Dados da Receita Federal](https://www.gov.br/receitafederal/dados/cnpj-metadados.pdf).

### 2. Inserção no Banco de Dados
Após a coleta e tratamento dos dados, o arquivo CSV é carregado no banco de dados PostgreSQL. Esse processo torna os dados acessíveis para consultas e análises mais detalhadas.

#### Carregamento dos Dados
A inserção dos dados é realizada com tratamento para garantir que cada registro seja inserido corretamente e que valores nulos ou inconsistentes sejam processados adequadamente. Em caso de falhas, o script de inserção fornece informações detalhadas para depuração.

### 3. Execução no Jupyter Notebook
Para facilitar a inserção e controle do processo, foi criado um Jupyter Notebook. Esse notebook permite:
- Conectar ao banco de dados PostgreSQL.
- Processar e inserir os dados de maneira interativa.
- Monitorar o status e os erros do processo de inserção para facilitar a depuração e o ajuste de dados.
