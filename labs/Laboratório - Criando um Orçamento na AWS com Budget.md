# Criando um Orçamento na AWS com Budget ![icons8-saco-de-dinheiro-30](https://github.com/user-attachments/assets/ef130703-01f3-4a05-9a40-859412d180a0)

## Laborátório 🥼
Este laboratório orienta passo a passo como configurar um
orçamento de gastos na AWS utilizando o serviço AWS Budgets. A atividade inclui
a criação do orçamento, configuração de alertas por e-mail e verificação das
definições aplicadas.

### Objetivos do laboratório
- Este laboratório ensina como:Acessar o serviço AWS Budgets pelo Console de Gerenciamento da AWS.
- Criar  um orçamento com limite personalizado.
- Configurar alertas por e-mail baseados em percentuais de uso.
- Validar a criação do orçamento e testar notificações automáticas.

### Cenário

Você é um desenvolvedor iniciante ou estudante que está utilizando a AWS para
aprender e realizar testes. Para evitar surpresas na fatura e manter seus
gastos sob controle, é essencial configurar um orçamento com alertas
automáticos. Este laboratório simula a criação de um orçamento simples, com
limite de US$ 10, e notificação por e-mail quando 10% do valor for utilizado.


1 - Crie um nome para o orçamento e também os destinatários que receberam notificações.

![image](https://github.com/user-attachments/assets/151e374a-7cff-43e6-afa8-0ac065aef796)

2 - Configuramos para que sejamos notiicados assim que Quando o custo real for maior que 10% (US$ 0,10) do valor orçado (US$ 1,00), o limite de alerta será excedido.
![image](https://github.com/user-attachments/assets/a81c3415-e9b6-4bf8-a955-7421cc6efc87)

3 - Notificação E-mail
![image](https://github.com/user-attachments/assets/82e465f3-c5d1-418e-a13a-d72e5e279e6f)


Configurar um Budget como este que você acabou de criar é uma prática fundamental
na gestão de custos na AWS. Ele não é apenas um número definido, mas sim uma
ferramenta proativa essencial.
A importância do AWS Budgets reside precisamente em sua capacidade de oferecer
visibilidade sobre seus gastos e, crucialmente, de alertar você antes que seus
custos ultrapassem limites definidos. Ao ser notificado quando atinge um percentual
(como os 10% configurados) ou um valor absoluto do seu orçamento, você ganha a
oportunidade de:

• Investigar a origem dos custos.
• Tomar ações corretivas a tempo (desligar recursos não utilizados, otimizar
serviços, etc.).
• Evitar surpresas desagradáveis e contas elevadas ao final do ciclo de
faturamento.

É uma camada essencial de controle financeiro que transforma o gerenciamento de
custos de reativo (descobrir o gasto no final do mês) para proativo (monitorar e agir
enquanto o gasto acontece). Portanto, utilize essa ferramenta e fique sempre atento
aos alertas para manter seus custos na nuvem sob controle!
