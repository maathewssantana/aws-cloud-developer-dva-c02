## Laboratório - Amazon S3 Básico, Avançado e Acesso a Logs ![icons8-bucket-30](https://github.com/user-attachments/assets/279ed93f-0151-49da-8d16-c0d7c9dcd06d)

Neste laboratório prático, você aprenderá a utilizar os principais recursos do Amazon S3 voltados à organização, segurança e gerenciamento eficiente de dados. Serão abordadas práticas recomendadas para criação de buckets com configurações seguras, 
controle de versões de arquivos, automação de regras de ciclo de vida e geração de URLs pré-assinadas para compartilhamento temporário e seguro de objetos. 
Além disso, será demonstrada a ativação e configuração do servidor de logs de acesso, utilizando um segundo bucket dedicado ao armazenamento dos registros de operação.

### Objetivos

- Criar buckets no Amazon S3 com configurações recomendadas de segurança.
- Ativar e utilizar o versionamento para manter múltiplas versões de arquivos.
- Configurar regras de ciclo de vida para transição e expiração de objetos.
- Gerar URLs pré-assinadas para compartilhamento seguro e temporário de arquivos.
- Ativar e consultar logs de acesso utilizando um segundo bucket.

### 📘 **Regra de Negócio:**

> "Armazenar os documentos fiscais enviados pelos clientes de forma segura, garantindo histórico de alterações, controle de acesso e descarte após 5 anos."

### ✅ **Como aplicar os pontos do bucket no dia a dia:**

#### 1. **Criar buckets no Amazon S3 com configurações recomendadas de segurança**

* Criamos um bucket chamado `documentos-fiscais-clientes`.
* Configuramos para **negar acesso público**, **habilitar criptografia automática** (AES-256 ou KMS) e usamos políticas IAM para que só usuários autorizados da empresa acessem.

#### 2. **Ativar e utilizar o versionamento**

* Ativamos o versionamento no bucket.
* Se um cliente reenviar um mesmo arquivo com correções, a versão anterior não é perdida.
* Isso cumpre requisitos legais de auditoria e rastreabilidade.

#### 3. **Configurar regras de ciclo de vida**

* Criamos uma regra que:

  * Move arquivos para a classe de armazenamento **S3 Glacier** após 1 ano (reduz custo).
  * Exclui automaticamente o arquivo após **5 anos** (prazo legal de retenção de documentos fiscais).

#### 4. **Gerar URLs pré-assinadas**

* Ao invés de tornar os arquivos públicos, usamos **URLs pré-assinadas válidas por 24h** para que os clientes acessem seus documentos.
* Isso garante acesso seguro e temporário sem necessidade de login no sistema.

#### 5. **Ativar e consultar logs de acesso**

* Habilitamos o **logging de acesso** e enviamos os logs para um segundo bucket chamado `logs-documentos-fiscais`.
* Periodicamente, analisamos os logs para identificar tentativas de acesso não autorizadas ou comportamento incomum.

---

### 🧩 Resumo

Essa aplicação prática mostra como os recursos do S3 **suportam diretamente** regras de negócio envolvendo **segurança, controle de versões, retenção legal de dados, auditoria e compartilhamento seguro**.


- Criar buckets no Amazon S3 com configurações recomendadas de segurança.
  
![buckets_02](https://github.com/user-attachments/assets/1bcc001d-a9d6-4d0b-856d-fcaca6602b0e)

- Ativar e utilizar o versionamento para manter múltiplas versões de arquivos.

![versionamento_01](https://github.com/user-attachments/assets/bdf7c52a-34dc-4dbf-a727-0473f28b7076)

- Configurar regras de ciclo de vida para transição e expiração de objetos.
  
![glaicer_01](https://github.com/user-attachments/assets/35023999-db1a-4371-bf66-e983f446a136)

- Gerar URLs pré-assinadas para compartilhamento seguro e temporário de arquivos.

![image](https://github.com/user-attachments/assets/a37254f6-dd51-45bf-9008-8dcb8906f2ab)

- Ativar e consultar logs de acesso utilizando um segundo bucket.
- 
![image](https://github.com/user-attachments/assets/2595de43-2c55-4acc-b03c-38d930f1d705)
