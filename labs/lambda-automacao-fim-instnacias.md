# Automação com Lambda para finalizar instâncias ![image](https://github.com/user-attachments/assets/60b1a3f8-8938-4a10-9bae-d5783d3f4ef0)

## Laborátório 🥼

Criar e gerenciar políticas IAM e funções Lambda na AWS, com foco em automação e integração entre serviços, permitindo a execução automática via EventBridge. 

### Passos para Conclusão do Laboratório:

Crie uma política de IAM que permita terminar instâncias EC2.
Crie uma função Lambda utilizando Python para executar a ação desejada.
Associe a política IAM criada à função Lambda.
Configure um gatilho no EventBridge para que a função Lambda seja executada automaticamente.

Essa automação com AWS Lambda e EventBridge é amplamente utilizada no ambiente corporativo para **gerenciar custos, melhorar a segurança e otimizar recursos de TI**.

### Aplicação no Negócio:

Empresas usam essa abordagem para **automatizar o desligamento de instâncias EC2 não utilizadas**, como servidores de desenvolvimento, testes ou recursos temporários. Isso evita desperdício de recursos e gastos desnecessários, além de manter o ambiente limpo e seguro.

### 3 Benefícios Iniciais:

1. **Redução de custos**
   Instâncias são encerradas automaticamente fora do horário de uso, economizando com uso desnecessário de recursos.

2. **Automação e Eficiência Operacional**
   Elimina tarefas manuais repetitivas de desligamento, liberando tempo da equipe de TI para atividades mais estratégicas.

3. **Segurança e Conformidade**
   Garante que instâncias não fiquem ativas além do necessário, reduzindo riscos de exposição e facilitando a conformidade com políticas internas.

**Configurei uma politica de IAM que permite terminar instâncias EC2.**

![PoliticaTerminarEC2-MatheusFelipedeSantana](https://github.com/user-attachments/assets/c98b5402-ca29-4187-8fb3-75bfa970fc37)

✅ Política IAM
Sua política está correta para permitir que a função Lambda registre logs e encerre instâncias EC2:

![image](https://github.com/user-attachments/assets/496b543e-f5e5-4c81-885d-4696c83e77c5)

**Criado uma função lambda para executar essa ação.**

✅ Código

![image](https://github.com/user-attachments/assets/bebbf624-5139-46aa-b974-443064c6955b)


**Associei a politica IAM criada para função Lambda**

![RoleTerminarEC2-MatheusFelipedeSantana](https://github.com/user-attachments/assets/a62a7c0d-1840-49e3-9648-a634b16aee3b)

**Por fim, criei um gatilho utilizando o EventBridge para execução.**

![EventBridge](https://github.com/user-attachments/assets/a5c76ef3-f32d-4e6d-8f65-f992fd42e754)




