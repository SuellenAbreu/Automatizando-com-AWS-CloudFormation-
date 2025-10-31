# Automatizando-com-AWS-CloudFormation-

Durante o processo de criação da pilha na AWS utilizando CloudFormation, o objetivo foi automatizar o provisionamento de recursos, como buckets S3, usando templates em JSON ou YAML. No início, o template foi criado para configurar todos os recursos necessários, mas logo encontrei desafios relacionados a erros de configuração.

Um dos maiores obstáculos foi o erro InvalidBucketAclWithObjectOwnership, causado pela tentativa de usar ACLs com a configuração BucketOwnerEnforced no bucket S3. A solução foi remover as ACLs ou ajustar a configuração do bucket para BucketOwnerPreferred, permitindo o uso das ACLs.

Além disso, outro erro surgiu devido ao nome de bucket duplicado, com o erro AlreadyExists. Isso exigiu que eu escolhesse um nome de bucket exclusivo, já que o S3 exige que os nomes de buckets sejam globalmente únicos.

Após corrigir esses problemas, a pilha foi atualizada com sucesso e o bucket foi criado corretamente. Esse processo destacou a importância de padronizar e replicar a infraestrutura corretamente para garantir que a criação dos recursos seja consistente e sem erros, além de demonstrar como a infraestrutura como código (IaC) pode agilizar e automatizar o provisionamento de recursos na AWS.
<img width="1247" height="733" alt="Captura de tela 2025-10-30 222955" src="https://github.com/user-attachments/assets/bb580e42-f932-4c4c-8088-048562a1163c" />
