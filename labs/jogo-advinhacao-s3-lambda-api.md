# Jogo de Adivinhação com AWS Lambda, API Gateway e S3 ![image](https://github.com/user-attachments/assets/e784c26b-b784-42b3-b932-557ec88cfaad)

### Objetivo 
Criar e gerenciar uma aplicação serverless na AWS, integrando múltiplos serviços para desenvolver um jogo de adivinhação simples, onde o usuário tenta adivinhar um número entre 1 e 10.

### Passo a Passo

- Desenvolver uma função Lambda em Python para implementar a lógica do jogo.
- Criar uma API RESTful com Amazon API Gateway para expor a função Lambda
- Publicar um frontend estático no Amazon S3 para interação com o usuário
- Conectar o frontend à API Gateway, permitindo chamadas à função Lambda.

1. Criação de uma função do Lambda

Criado uma função lambda.
![lambda_1](https://github.com/user-attachments/assets/345ac771-3439-4a0c-9fde-36caae3872c4)

2. Script lambda
Realizado um upload com o Scripti em Python.

3. Criando API comAmazon API Gateway
![api_2](https://github.com/user-attachments/assets/5b8453ab-ad8a-4ba9-9a68-baa64a5a598e)

Criado um API Gateway com metodo GET apenas. Ele faz a utilização do metodo HTTP buscando integrações no Lambda.

![image](https://github.com/user-attachments/assets/35e94293-77ef-47c5-8ce0-9fb4638f9320)

4. Website estático S3
Utilizamos um index.hmtl estático no S3, que faz a requisição da API.
Configuramos no bucket para ativar hospedagem de site estático.
Fixamos um documento no índice
Desbloqueamos o acesso para o público, fazendo com que as pessoas consigam ver o site na web.

![s3_1](https://github.com/user-attachments/assets/9d39b5e2-a755-443b-9065-239190c108b4)

Deixamos ativos:
Bloquear acesso
público a buckets e objetos concedidos por meio de novas listas de controle
de acesso (ACLs)" e "Bloquear acesso público a buckets e objetos
concedidos por meio de qualquer lista de controle de acesso (ACLs)", você
impede que permissões de acesso sejam concedidas via ACLs, garantindo que o
controle de acesso seja feito exclusivamente por meio de políticas de bucket.

![image](https://github.com/user-attachments/assets/c4f8b015-668c-4ff1-852a-a829d7684ce5)

5. Controle de políticas do Bucket

política do bucket para definir quem pode acessar o conteúdo e quais permissões serão concedidas.
![image](https://github.com/user-attachments/assets/cecd94dd-a7da-483d-8820-0ce54764b49e)

Teste de Site:
Funcionando:
![jogo_ok](https://github.com/user-attachments/assets/35ff3067-a9fe-4199-85cf-d94d6a4e63a4)

Possíveis Erros
Durante os testes recebi um erro 404 quando digitado o número, esse erro foi porque ele não conseguiu fazer a requisição na API.
![erro_404](https://github.com/user-attachments/assets/a01de784-b8ab-4ce1-9da5-cb92d0dac864)

Fazendo a requisição da API no Postman o erro no endpoint ocorria o mesmo.

![image](https://github.com/user-attachments/assets/4e63eebe-d44a-4ef9-a94b-95a96ae84e79)

Fiz um Troubleshooting dos passos, idenfiquei que o endpoint informado esatava faltando um /jogo, após o ajuste normalizou.
![image](https://github.com/user-attachments/assets/9cad3fcd-cf38-49b4-8d5c-f8ec6342f08a)







