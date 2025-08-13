# engenharia-dados-pipeline
Projeto de aplicação pratica de conhecimentos adiquiridos curso de Pós Graduação e Engenharia de Dados disciplina Engenharia de Dados na Pratica 

# Descrição detalhada 
Este projeto simulara a contrução de um pipeline de dados usando a Arquitetura de Dados Medalhas (Medallion Arch), que é divida em três camadas detro do DataLake conforme a figura abaixo:

![alt text](image.png)

### Camada Bronze
Na camada temos a ingestão dos dados ainda em estado bruto no DataLake estraídos recentemento da fonte de dados, passando antes por uma camada intermediária de pré tratamento conhecida com Landing Layer