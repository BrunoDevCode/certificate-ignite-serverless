<h1>Certificate Ignite - Serverless</h1>

<h3>Tecnologias</h3>

- [Node.js](https://nodejs.org/en/)
- [Typescript](https://www.typescriptlang.org/)
- [Serverless Framework](https://www.serverless.com/)
- [Puppeteer](https://puppeteer.github.io/puppeteer/)
- [Lambda AWS](https://aws.amazon.com/pt/lambda/)

<h3>Códigos</h3>

<p>Aqui descrevo todos os códigos necessário para criação até o deploy da aplicação.</p>

Criar projeto:

``
serverless create --template aws-nodejs-typescript --path nomeDaPasta
``

Instalar a lib para rodar na maquina local

``
yarn add serverless-offline -D
``

Rodar o serverless na maquina local

``
serverless offline
``

Instalar o DynamoDB

``
serverless dynamodb install
``

Para rodar o dynamo localmente é necessário

``
yarn add serverless-dynamodb-local -D
``

Iniciar o DynamoDB

``
serverless dynamodb start
``

Para o deploy é necessário criar um usuário IAM: AdministratorAccess

``
serverless config credentials --provider aws --key=UserID --secret userPass
``

Comando de deploy

``
serverless deploy --verbose
``
