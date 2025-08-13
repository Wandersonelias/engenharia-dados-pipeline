# engenharia-dados-pipeline
Projeto de aplicação pratica de conhecimentos adiquiridos curso de Pós Graduação e Engenharia de Dados disciplina Engenharia de Dados na Pratica 

# Descrição detalhada 
Este projeto simulara a contrução de um pipeline de dados usando a Arquitetura de Dados Medalhas (Medallion Architecture), que é divida em três camadas detro do DataLake conforme a figura abaixo:

![alt text](image.png)


### Camada Landing

È uma camada para pré processamento de arquivos, geralmente usado como uma intermediária para tratamento de dados, no caso dados que vem em algum padrão diferente da Camada Bronze

### Camada Bronze
Na camada temos a ingestão dos dados ainda em estado bruto no DataLake estraídos recentemente extraidos da fonte de dados, passando antes por uma camada intermediária de pré tratamento conhecida com Landing que recebe os dados na origem e pode transformar em outros formato antes de inserir na Camada bronze ainda sem tratamento de dados, quando há casos que os dados não podem ser inseridos diretamente na camada bronze sem transformação.

### Camada Silver

Na camada Silver o precesso de refinameto dos dados é inciado, com a transformação dos dados, e aplicação de tradução dos tipos de dados, renomeando colunas e também a aplicação de regras de data e hora, a formatação de textos no caso de impacto nos dados e padronização do formatado de dados, e desduplicação dos dados recebidos entre outras regras que sejam necessarias aplicar, e a preparação das tabelas para visualização de dados 

### Camada Gold

Onde serão disponibilizados as tabelas para visualização de dados, os dados já estarão tratados usando tabelas de fatos e dimensões, usando modelos star schema e snow flake


### O que será realizado neste projeto

Será realizado a simulação de dados importados do SAP, que chegaram na camada Landing em formato CSV, por meio de pastas de arquivos, a seguir eles serão processados e salvos na Camada Bronze, na sequencia os dados serão refinados na Camada Silver onde todas a tranformações serão realizadas para serem disponibildas na Camada Gold como self service BI  
