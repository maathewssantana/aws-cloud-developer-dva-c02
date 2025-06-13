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
