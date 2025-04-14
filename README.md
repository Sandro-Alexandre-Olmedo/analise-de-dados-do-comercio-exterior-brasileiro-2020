# Projeto de Análise de Dados de Importação do Comércio Exterior Brasileiro 2020 
# Com linguagem de programação Python, SQL e serviços da Amazon Web Services


![swift](https://img.shields.io/badge/Python-FFD438?style=for-the-badge&logo=Python&logoColor=blue)
![swift](https://img.shields.io/badge/SQL-023E8A?style=for-the-badge&logo=sql&logoColor=blue)
![swift](https://img.shields.io/badge/AWS-BE5504?style=for-the-badge&logo=aws&logoColor=blue)

![comex](https://github.com/Sandro-Alexandre-Olmedo/analise-de-dados-de-comercio-exterior/blob/main/images/comex.png)

# Introdução

## Quanto aos dados:

Conhecer os dados, como estão estruturados e como devem ser estruturados é de suma importância no momento de desenvolver projetos de analises de dados, seja para aplicações off-line ou online, entre outras.

Grande parte de um projeto de analise de dados esta em `ETL` (extrair, transformar e carregar), ou seja, arrumar as coisas conforme as necessidades para permitir a geração assertiva de resultados e insights relevantes para as tomadas de decisões.

Este é um projeto simples de analise de dados, mas que exigiu alguns esforços e conhecimentos. As possibilidades de se chegar aos mesmos ou melhores resultados deste projeto são inúmeras por meio de outras ferramentas e linguagens de programação, contudo, fica a critério de cada interessado realizá-lo conforme eventual necessidade. 

## Quanto às importações:

É muito interessante conhecer como as importações evoluem ao longo do tempo em volume, em valor e outras variáveis muito importantes, isso ajuda a entender a economia de um país e as relações internacionais. 

O comércio exterior ou Comex é uma área complexa e que esta em constante evolução, principalmente no que diz respeito à tecnologia, envolve questões tributárias, financeiras, administrativas, comerciais e aduaneiras. 

Sendo assim, saber detalhadamente como tudo ocorre é primordial nesse mundo, pois, dados ou informações erradas podem gerar grandes prejuízos.

# Visão Geral da Solução na AWS

![AWS](https://github.com/Sandro-Alexandre-Olmedo/analise-de-dados-de-comercio-exterior/blob/main/images/visaogeralsolucaoaws.png)
> O Usuário faz o upload de um arquivo para o `bucket` da `Amazon S3`
>
> A `AWS Glue` cataloga a localização, schema e estrutura dos dados
> 
> O catálogo com localização, schema e estrutura dos dados são criados a partir da criação das tabelas do `Athena` no próprio console do `Glue` ou direto via código no console do `Athena`
>
> As consultas do `Athena` acessam o `Glue` para verificar informações sobre os dados e só então acessam o bucket por meio de consultas SQL
>
> Os resultados são exibidos na tela ao usuário, caso o usuário necessite pode fazer o download dos resultados em CSV 
>
> **Observação:** Essa é uma aplicação simples, o S3 e Athena podem interagir com diversas ferramentas da própria AWS, API’s e serviços de terceiros, tanto no recebimento quanto no envio de dados



         

