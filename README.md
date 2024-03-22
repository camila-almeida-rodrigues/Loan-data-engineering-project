# Loan-data-engineering-project
Loan-data-engineering-project

A arquitetura medalhão visa fornecer diferentes níveis de serviço e desempenho, dependendo das necessidades específicas de cada área. Cada camada oferece um conjunto diferente de funcionalidades e tratamento de dados.

Camada Bronze:
  - Representa a base da arquitetura, onde os dados brutos são inicialmente armazenados e processados.
 
Camada Silver:
  - Esta camada intermediária é responsável pelo tratamento e limpeza dos dados

Camada Gold:
  - É a camada de maior refinamento, pronta para alimentar projetos de Business Intelligence (BI) com dados de alta qualidade e confiabilidade.

No projeto em questão, foram utilizados dados abertos de empréstimos, incluindo informações dos clientes como gênero, escolaridade, renda, entre outros. Para a implementação da arquitetura, optou-se pelo Azure, fazendo uso dos seguintes recursos:

![image](https://github.com/camila-almeida-rodrigues/Loan-data-engineering-project/assets/139059782/38a2aad0-108b-4a94-811a-995a429fbc20)


A arquitetura é representada de forma visual abaixo:
![Arquitetura](https://github.com/camila-almeida-rodrigues/Loan-data-engineering-project/assets/139059782/49ff22b5-7e6c-477a-9802-e8d8674da2e4)


Data Factory - É responsável por criar um pipeline que carrega os dados brutos e os insere no container da Camada Bronze. Posteriormente, após o tratamento no Azure Databricks, os dados são inseridos no pipeline para garantir a automatização do processo.

![image](https://github.com/camila-almeida-rodrigues/Loan-data-engineering-project/assets/139059782/4a42e2a2-e834-43e7-a32b-831053b2b373)


Azure Databricks - Esta ferramenta é utilizada para o tratamento dos dados, seguindo os princípios da arquitetura Medalhão.

 Data Lake Storage Gen2 - Serve como armazenamento para os dados, tanto estruturados quanto não estruturados.

 Azure Synapse - Cria visualizações do armazenamento da Camada Gold, permitindo que sejam utilizadas pelo Power BI para a criação de dashboards e análises.

 Power BI - Utilizado para a criação de dashboards e análises a partir dos dados disponíveis na Camada Gold.
