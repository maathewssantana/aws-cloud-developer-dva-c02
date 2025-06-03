# Tópico SNS e filas SQS Padrão e DLQ  ![icons8-fila-30](https://github.com/user-attachments/assets/b849ae17-cdc2-4d69-beca-124e81c6c8a3)


### Objetivo 
Neste laboratório, você irá criar um fluxo de mensagens desacoplado utilizando SNS (Simple Notification Service) e SQS (Simple Queue Service) com uma Dead-Letter Queue (DLQ). Esse cenário simula a arquitetura de microsserviços,
onde eventos são publicados e processados de forma assíncrona, com tolerância a falhas.

### Passos para Conclusão do Laboratório:

- Criar uma fila SQS para servir como Dead-Letter Queue (DLQ).
- Criar uma fila SQS principal (Padrão).
- Configurar a fila principal para usar a DLQ (Política de Redirecionamento/Redrive Policy). 
- Criar um tópico SNS Padrão.
- Inscrever a fila SQS principal no tópico SNS.
- Testar o envio de mensagens via SNS e o recebimento na fila SQS. 
- Compreender e simular o envio de mensagens para a DLQ.
