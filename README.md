# Desafio-Devops

## Descrição do desafio

Considere que você foi contratado para subir uma aplicação (deploy) Api em Django + PostgreSQL, e você chegou a conclusão que a melhor forma de fazer isso é utilizando containers, como por exemplo as ferramentas Docker e Docker Compose. Então este desafio tem como objetivo testar a sua capacidade de fazer o deploy de uma aplicação e mostar noções de DevOps, em especial na parte de CI/CD (Integração contínua e Entrega contínua).

## Instruções

O foco do desafio é no deploy e boas praticas Devops, logo, recomendamos que faça um fork da aplicação Api que disponibilizamos nesse repositório, para poder se concentrar na estrutura da aplicação.

## Requisitos Principais

|**Requisitos**| **Objetivo** | **Detalhes**|
|---------------|----------|----------------|
| Req 1         | Aplicação deverá conter um arquivo Dockerfile para realizar a build (construção da aplicação)|
| Req 2         | O arquivo responsável por subir o container deverá ser o Docker-compose contendo as demais informações (Ex. porta, nome, imagem e etc...) |
| Req 3         | O container deverá rodar em uma porta diferente da 8000, pois a aplicação da API já vem pré-configurada para isso, e queremos que explore e entenda as configurações de porta do Docker|
| Req 4         | Implementar a Pipeline CI no Github actions |
| Req 5         | Implementar conecxão com banco de dados PostgreSQL (Implementar uma nova instancia no docker e fazer a parte de comunicação com a API. | No arquivo .env está disponivel os dados do banco |
| Req 6         | Utilização de NGINX para permitir o acesso através da porta 80 direcionando para a porta do container |
| Req 7        |  Projeto bem documentado no GitHub (Arquivo Readme bem detalhado), incluindo instruções de como executar e testar o desafio | Existe um arquivo chamado yours_readme.md, onde você vai documentar


## Requisitos Extras


|**Requisitos**| Objetivo | Detalhes |
|---------------|----------|-------|
| Req Extra |  Criar um pipeline CD - O principal objetivo é ver como você organiza o arquivo de configuração "deploy.yml", responsável por esse papel | Lembrando que o deploy deverá ser baseado em containers Docker |




