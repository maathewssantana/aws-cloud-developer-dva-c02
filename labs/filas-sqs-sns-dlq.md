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


### Criei uma fila SQS para servir como Dead-Letter Queue (DLQ).
![fila-dlq](https://github.com/user-attachments/assets/9a9939da-5254-4b21-9c41-b6b9cdd3f74d)

### Criei uma fila SQS principal (Padrão).
![fila-principal-sqs](https://github.com/user-attachments/assets/650dfb08-50dd-4c19-958c-720025633cb7)

### Configurei a fila principal para usar a DLQ (Política de Redirecionamento/Redrive Policy)
### Criei um tópico SNS Padrão.
![topico-sns](https://github.com/user-attachments/assets/eb5ea036-8dd5-45ba-8598-9c64561378bc)

### Testei o envio de mensagens via SNS e o recebimento na fila SQS. 
![mensagem-sqs](https://github.com/user-attachments/assets/a15206b8-7cf0-409a-b524-bf2abc667de0)

### Simulado o envio de mensagens para a DLQ.
![image](https://github.com/user-attachments/assets/ea476790-a42b-45dc-b418-d2a2fb540f2f)

### Como adicional criei um script em Python que envia uma mensagem para fila principal, e depois faço a leitura da mensagem na fila.
![image](https://github.com/user-attachments/assets/9825c32d-b7ad-4779-9c01-c0bd37e2926c)
