# Escreva sua Documentação AQUI!!!

## Como executar o projeto
### Requisitos:
- **Docker**
- **Docker-compose**
### Versões testadas:
- **docker**: *Docker version 20.10.12, build 20.10.12-0ubuntu2~20.04.1*
- **docker-compose**: *docker-compose version 1.29.2, build 5becea4c*

Para executar o modo dev `make dev`

Para executar o modo de prod `make dev` [esse modo e ilustrativo nao recomendo utilizar essa estrategia]

Caso queira desligar o server de `CTRL + C`
## Como foi feito o desafio
### Step 1
A princípio eu queria utilizar uma image alpine mas deu incompatibilidade com a lib `psycopg2-binary`
então troquei para uma image slim onde está funcionando como o esperado
### Step 2
Com o `docker-compose` ocorreu do jeito que eu esperava :)
### Step 3
Básico de docker
### Step 4
Nao conheço tanto sobre python mas usei o test padrão dele para fazer validação, apesar de nao ter nem um test automatizado escrito
### Step 5
acho que isso nao deveria esta aqui em sim no na etapa um, rodar o projeto junto com o postgres pois a aplicação nao sobe sem ele
### Step 6
Nao conhecia o nginx tanto assim so ouvir falar dele, mas acabou sendo fácil de ser utilizar
### Step 7
Estamos aqui :)
### Step 8
Esse aqui posso explicar como pensei em como fazer, usando o docker + github action, da para cria a image docker apos o processor de test do ci subir ela para o docker hub e depois automatizar o deploy com algumas action da aws junto com os serviços dela como aws codedeploy service, pensando em um ambiente simples, pensando um pouco maior poderia utilizar ferramentas de cd como Jenkins junto com o action para ter maior automação e segurança + clusters Kubernetes para ter uma escalabilidade e resiliência
