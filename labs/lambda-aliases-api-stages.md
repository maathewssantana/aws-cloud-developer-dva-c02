# AWS Lambda  com Aliases e API Gateway com Stages ![icons8-configurações-de-api-30](https://github.com/user-attachments/assets/5d305bf0-c044-41f2-8df4-ea2d8f145ca5)


## Laborátório 🥼

Neste laboratório, você irá configurar uma arquitetura serverless organizada por ambientes (como desenvolvimento e produção), utilizando e . Essa abordagem permite controlar o ciclo de vida da aplicação com segurança e agilidade.

- Criar uma função AWS Lambda compatível com a integração Proxy do API Gateway.
- Publicar pelo menos duas versões da função Lambda para representar diferentes estados do código.
- Criar Aliases no Lambda (ex: dev, prod) apontando para versões específicas da função.
- Criar uma API REST no API Gateway.
- Configurar a integração do tipo Proxy entre a API Gateway e a função Lambda.
- Criar Stages no API Gateway (ex: Desenvolvimento, Producao) representando os ambientes.
- Integrar cada Stage com o Alias correspondente da função Lambda.
- Testar os endpoints dos Stages (/dev, /prod) para garantir que cada um acione a versão correta da função Lambda.
- Compreender os benefícios do uso combinado de Aliases (Lambda) e Stages (API Gateway) para o gerenciamento do ciclo de vida e implantação controlada de aplicações serverless


### Versões do lambda
![lambda-versoes](https://github.com/user-attachments/assets/6c7430e9-ef27-4ebd-acb1-0466496ecece)

### Aliases lambda
![versao-aliases-lambda](https://github.com/user-attachments/assets/b24055dc-31ca-410d-baf8-32eea25af345)

### Stages API Gateway (Prod e Dev) Metódo (GET)
![stages-api-gateway](https://github.com/user-attachments/assets/7880ddc7-70f1-49df-b657-928e2cea9abe)

### Teste API Postman
/Prod

![get-postman-prod](https://github.com/user-attachments/assets/777eb6a3-6b49-4c9b-9835-600652440db9)

/Dev
![get-postman-dev](https://github.com/user-attachments/assets/7e5c2563-4a2b-43fa-b5b3-8070ef84d830)

