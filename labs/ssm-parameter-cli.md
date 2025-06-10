# SSM Parameter Store Hands on (CLI) ![image](https://github.com/user-attachments/assets/ebd15aca-78f7-4e24-85a3-20df053e62e4)


## Laborátório 🥼

Neste laboratório prático, você aprenderá a criar e gerenciar parâmetros utilizando o AWS Systems Manager Parameter Store, incluindo parâmetros seguros criptografados com chaves do KMS (AWS Key Management Service), 
além de acessar os valores por meio da AWS CLI no CloudShell.

### Objetivos do laboratório

- Criar parâmetros do tipo String e SecureString no Parameter Store.
- Criar uma chave de criptografia (CMK) no KMS para proteger os parâmetros sensíveis.
- Recuperar os parâmetros por meio da AWS CLI, utilizando comandos com e sem a opção de descriptografia.
- Navegar e visualizar os parâmetros diretamente no console do AWS Systems Manager.


### Criar parâmetros do tipo String e SecureString no Parameter Store.
Criamos chaves dentro do SSM para salvar em parâmetros. 2 Tipo Strig e 2 Security String.
![ssm-strings](https://github.com/user-attachments/assets/654bc368-56a8-416f-bb90-7621c81c13ee)

###  Criar uma chave de criptografia (CMK) no KMS para proteger os parâmetros sensíveis.
Criado uma chave KMS para criptografar os dados.
![kms](https://github.com/user-attachments/assets/65b1cd6b-86ed-471e-97a3-9330b4a745d5)

### Recuperar os parâmetros por meio da AWS CLI, utilizando comandos com e sem a opção de descriptografia.
![cli-ssm](https://github.com/user-attachments/assets/f81bc9b1-1070-424f-bdcd-f2297a133532)

### Utilizando --with-decryption
![image](https://github.com/user-attachments/assets/38e42fdf-811b-4f74-aeee-c4073b0a14e7)


