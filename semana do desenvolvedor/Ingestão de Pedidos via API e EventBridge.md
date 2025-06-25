## Ingestão de Pedidos via API e EventBridge

_Este laboratório marca o início da semana do desenvolvedor AWS da Escola da Nuvem, voltada para alunos do curso AWS Developer Associate. Nesta sessão, construiremos o fluxo inicial para a ingestão de pedidos. 
Nosso objetivo é criar um endpoint de API REST que receberá dados de pedidos, passará por uma Lambda de pré-validação, será enfileirado em uma fila SQS FIFO (First-In, First-Out) para garantir a ordem, e então processado por uma segunda Lambda que validará o pedido mais a fundo e publicará um evento em um barramento de eventos customizado no Amazon EventBridge._


### Objetivos

- Endpoint API funcional para receber pedidos.
- Duas funções Lambda para validação.
- Uma fila SQS FIFO para desacoplar o processamento.
- Um barramento de eventos customizado para notificar sobre novos pedidos validados.

![sqs-semanadev](https://github.com/user-attachments/assets/d526cd3d-09b1-4307-bde1-3414b2c28512)
![sqs-fila](https://github.com/user-attachments/assets/5d65b78b-4494-40b6-8999-4ae793b37be1)
![postman-envio](https://github.com/user-attachments/assets/c6193ebb-4669-4c34-b8a9-beb6726f8461)
![lambda](https://github.com/user-attachments/assets/a21bf46c-cf21-4690-8644-dfca9f3811c6)
![event-bridge](https://github.com/user-attachments/assets/4c7973bf-67a3-4145-bdc4-6297cd21c4e0)
![cloudwatch](https://github.com/user-attachments/assets/0295087a-5af0-473a-9194-ad10e9056f2d)
![api-gateway](https://github.com/user-attachments/assets/13272bad-eada-40eb-9c09-c8e2c7ff1e94)

