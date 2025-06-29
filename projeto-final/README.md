## Projeto Final 

_Uma arquitetura orientada a eventos, serverless e
desacoplada, capaz de lidar com múltiplas fontes de dados e diferentes
operações de negócio. Ela utiliza serviços essenciais da AWS_

- Compute: AWS Lambda
- Integração: Amazon API Gateway, Amazon SQS (Standard e FIFO), Amazon EventBridge, Amazon SNS
- Armazenamento: Amazon S3, Amazon DynamoDB
- Gerenciamento e Governança: AWS IAM, AWS CloudWatch (Logs e Métricas)

######
![image](https://github.com/user-attachments/assets/63553682-2d02-451a-80ab-7d899ee6a995)

#### Utilizando dessa estrutura para criação de pedidos por API, criei um frontend, deixo em anexo os arquivos do projeto.
![frontendp-api](https://github.com/user-attachments/assets/ad2aa28e-2ec9-46c7-a84a-345343fcba6a)

#### Primeiro rode npm install e depois npm run dev, e logo abre no navegador o projeto.
![image](https://github.com/user-attachments/assets/21274b69-dfe8-44c2-87c1-d9fe744b8fc3)

#### Tive que realizar algumas liberações, implantando na API REST a liberação ao CORS.
![image](https://github.com/user-attachments/assets/eadf7d16-5e73-4432-aa3d-db4dddba0f55)

# Cabeçalhos CORS globais
cors_headers = {
    'Content-Type': 'application/json',
    'Access-Control-Allow-Origin': '*',  # ou 'http://localhost:5173' se preferir
    'Access-Control-Allow-Headers': 'Content-Type,Authorization',
    'Access-Control-Allow-Methods': 'OPTIONS,POST,GET'
}

### Também realizei um ajuste no lambda de pre-validacao que processa os dados vindos do API Gateway. inserindo a liberação.
![image](https://github.com/user-attachments/assets/748325aa-f06a-47f9-909c-9d4a8806e46e)

### Abaixo após o produto cadastrado no FrontEnd criado, analisando o fluxo seguido.
![valida-pedido](https://github.com/user-attachments/assets/75e106e1-d178-4749-96fe-bee6c4d732c3)
![processa-pedido](https://github.com/user-attachments/assets/98575204-0ba3-4e03-a171-baa97725066c)
![pre-processa](https://github.com/user-attachments/assets/7b4caf1d-2be1-4b32-822f-bd9500abf257)
![pedido-processado-dynamo](https://github.com/user-attachments/assets/5766a936-46aa-44b2-8af5-1528c1007d93)

