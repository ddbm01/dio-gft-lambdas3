# Desafio: Automação de Tarefas com AWS Lambda e S3

## 📝 Descrição do Desafio
Este repositório contém a documentação e os insights adquiridos durante o laboratório prático de automação na AWS. O objetivo principal foi consolidar os conhecimentos integrando o Amazon S3 com o AWS Lambda, acionando funções automaticamente após o upload de arquivos.

## 🎯 Objetivos de Aprendizagem Alcançados
- Aplicação prática de conceitos de Cloud Computing.
- Configuração de Triggers (Gatilhos) entre S3 e Lambda.
- Gerenciamento básico de permissões (IAM Roles).
- Documentação técnica e versionamento de código via GitHub.

## 🛠️ Tecnologias e Serviços Utilizados
- **Amazon S3:** Armazenamento de objetos.
- **AWS Lambda:** Computação Serverless.
- **AWS CloudWatch:** Monitoramento e Logs.
- **Linguagem:** Python (ou Node.js) para o script da Lambda.

## 🚀 Passo a Passo da Implementação

1. **Criação do Bucket S3:** 
   Foi criado um bucket com o nome `[SEU_NOME_DE_BUCKET]`.
   ![Bucket S3](images/print-bucket-s3.png)

2. **Criação da Função Lambda:** 
   Desenvolvimento de uma função Serverless para processar o evento.
   ![Função Lambda](images/print-lambda.png)

3. **Configuração do Gatilho (Trigger):** 
   O bucket S3 foi configurado para disparar um evento `s3:ObjectCreated:*` para a função Lambda.

4. **Teste e Validação:** 
   Ao fazer o upload de um arquivo de teste no S3, a Lambda foi executada com sucesso, conforme logs no CloudWatch.
   ![Logs CloudWatch](images/print-cloudwatch.png)

## 💡 Insights e Anotações
- **IAM é fundamental:** Aprendi que sem a Role correta, a Lambda não consegue ler os dados do S3 ou escrever logs no CloudWatch.
- **Custos:** O modelo Serverless é excelente pois só há cobrança quando o código é executado.
- (Adicione aqui outras coisas que você achou interessante ou dificuldades que teve).
