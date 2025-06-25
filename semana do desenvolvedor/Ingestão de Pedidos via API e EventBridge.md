## Ingestão de Pedidos via API e EventBridge

_Este laboratório marca o início da semana do desenvolvedor AWS da Escola da Nuvem, voltada para alunos do curso AWS Developer Associate. Nesta sessão, construiremos o fluxo inicial para a ingestão de pedidos. 
Nosso objetivo é criar um endpoint de API REST que receberá dados de pedidos, passará por uma Lambda de pré-validação, será enfileirado em uma fila SQS FIFO (First-In, First-Out) para garantir a ordem, e então processado por uma segunda Lambda que validará o pedido mais a fundo e publicará um evento em um barramento de eventos customizado no Amazon EventBridge._


### Objetivos

- Endpoint API funcional para receber pedidos.
- Duas funções Lambda para validação.
- Uma fila SQS FIFO para desacoplar o processamento.
- Um barramento de eventos customizado para notificar sobre novos pedidos validados.
