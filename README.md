# World GDP Data ETL

Este projeto é um exemplo de um pipeline ETL (Extração, Transformação e Carregamento) que lida com dados de PIB de vários países. O objetivo principal é criar um script que pode extrair os dados de PIB de uma fonte da web, realizar transformações necessárias e carregar os dados em um arquivo CSV e em um banco de dados SQLite. O código também inclui funcionalidade de registro de progresso em um arquivo de log.

## Funcionalidades

O projeto inclui as seguintes funcionalidades:

1. **Extração de Dados**: O script acessa uma URL que contém os dados de PIB de países e extrai as informações relevantes usando BeautifulSoup.

2. **Transformação de Dados**: Os dados extraídos passam por um processo de transformação, que inclui a conversão dos valores de PIB de milhões para bilhões de dólares.

3. **Carregamento de Dados**: Os dados transformados são carregados em um arquivo CSV e em uma tabela de banco de dados SQLite.

4. **Registro de Progresso**: O script registra mensagens de progresso em um arquivo de log para manter um registro das etapas concluídas.

5. **Consulta SQL**: O script inclui a capacidade de executar consultas SQL no banco de dados e exibir os resultados.

## Estrutura do Repositório

O repositório contém os seguintes arquivos:

- `.gitattributes`: Arquivo de configuração do Git.
- `Countries_by_GDP.csv`: Arquivo CSV com dados de PIB dos países (em bilhões de dólares).
- `etl_project_gdp.py`: Código Python para ETL de dados de PIB.
- `etl_project_log.txt`: Registro de progresso e mensagens do processo ETL.
- `World_Economies.db`: Banco de dados SQLite para armazenar dados de PIB.
- `README.md`: Este arquivo de documentação.


## Pré-requisitos e Instalação

Certifique-se de que você tenha as seguintes bibliotecas Python instaladas:

- `requests`: Para fazer solicitações HTTP para a página da web.
- `beautifulsoup4`: Para fazer a análise HTML da página da web.
- `pandas`: Para manipulação de dados tabulares.
- `numpy`: Para operações matemáticas.
- `sqlite3`: Para trabalhar com o banco de dados SQLite.

Você pode instalar essas bibliotecas usando o pip:

`pip install requests beautifulsoup4 pandas numpy sqlite3`

## Execução do Projeto

Para executar o projeto, siga os passos abaixo:

1. Clone este repositório em sua máquina local.
2. Certifique-se de ter todas as dependências necessárias instaladas.
3. Execute o arquivo `etl_project_gdp.py`.
4. O script executará o pipeline ETL completo e registrará o progresso em um arquivo de log.
