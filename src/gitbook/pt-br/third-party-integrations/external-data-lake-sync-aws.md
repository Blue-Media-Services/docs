# Sincronização com Data Lake Externo (AWS)

A integração entre os Armazenamentos de Eventos e a AWS permite a transferência contínua de dados de eventos para um bucket S3, garantindo arquivamento eficiente, backup e acessibilidade dos dados. Exportar seus dados para um data lake externo oferece mais controle sobre suas informações, levando a insights valiosos.

{% hint style="warning" %}
_Antes de começar, certifique-se de que você tem acesso ao Console de Gerenciamento da AWS com permissões para gerenciar Nuvens Privadas Virtuais (VPC), Grupos de Segurança, funções Lambda e papéis IAM. Além disso, considere que este procedimento pode gerar custos adicionais em sua conta da AWS devido à criação e uso de novos recursos._
{% endhint %}

## Implantando Infraestrutura com AWS CloudFormation <a href="#deploying-infrastructure-with-aws-cloudformation" id="deploying-infrastructure-with-aws-cloudformation"></a>

Dois modelos foram desenvolvidos usando o CloudFormation para simplificar a configuração da integração e fornecer a infraestrutura mínima necessária. Dependendo do seu conhecimento técnico, você pode personalizar esses modelos após a configuração inicial para atender às necessidades do seu negócio.

{% hint style="info" %}
_Para continuar, você precisa de uma Chave de API criada com permissões de leitura para os armazenamentos de eventos. Você pode aprender a criar e recuperar uma Chave de API_ [_neste artigo_](../product-documentation/identity-access-management-iam/api-keys.md)_._
{% endhint %}

### Modelo com VPC <a href="#template-with-vpc" id="template-with-vpc"></a>

Use este modelo se uma Nuvem Privada Virtual (VPC) já estiver configurada em sua conta AWS. Acesse o modelo [aqui](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/with-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1123).png" alt=""><figcaption><p>Modelo com VPC</p></figcaption></figure>

Após acessar o modelo, preencha os detalhes:

* Nome da Stack: Este campo é preenchido automaticamente, mas você pode usá-lo para personalizar o nome da stack.
* Nome do Bucket S3: Informe ou crie um nome para o seu Bucket S3.
* Criar Bucket S3: Escolha 'true' para criar um novo Bucket S3 ou 'false' para usar um já existente.
* ID da Conta: Informe seu ID de Conta BMS.
* ID do Armazenamento de Eventos: Informe o ID do Armazenamento de Eventos; você pode encontrá-lo clicando em <img src="../.gitbook/assets/image (1121).png" alt="edit" data-size="line"> na mesma linha do Armazenamento de Eventos que deseja importar.
* Chave de API: Informe uma Chave de API BMS com a política de acesso "MON - Armazenamento de Eventos - Somente Leitura".

Após preencher todos os campos, no final da página você deve confirmar que o AWS CloudFormation poderá criar recursos IAM para este modelo. Em seguida, clique em 'Criar Stack' para prosseguir com a criação da stack.

### Modelo sem VPC <a href="#template-without-vpc" id="template-without-vpc"></a>

Se sua conta AWS não tiver uma Nuvem Privada Virtual (VPC) configurada, use este modelo, que pode ser acessado [aqui](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/without-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1124).png" alt=""><figcaption><p>Modelo sem VPC</p></figcaption></figure>

Após acessar o modelo, preencha os detalhes:

* Nome da Stack: Este campo é preenchido automaticamente, mas você pode usá-lo para personalizar o nome da stack.
* Nome do Bucket S3: Informe ou crie um nome para o seu Bucket S3.
* Criar Bucket S3: Escolha 'true' para criar um novo Bucket S3 ou 'false' para usar um já existente.
* ID da Conta: Informe seu ID de Conta BMS.
* ID do Armazenamento de Eventos: Informe o ID do Armazenamento de Eventos; você pode encontrá-lo clicando em <img src="../.gitbook/assets/image (1121).png" alt="edit" data-size="line"> na mesma linha do Armazenamento de Eventos que deseja importar.
* Chave de API: Informe uma Chave de API BMS com a política de acesso "MON - Armazenamento de Eventos - Somente Leitura".
* IDs de Sub-rede: Selecione um ID de sub-rede para a função Lambda na lista suspensa.
* IDs do Grupo de Segurança: Selecione um ID de grupo de segurança para a função Lambda na lista suspensa.

Após preencher todos os campos, no final da página você deve confirmar que o AWS CloudFormation poderá criar recursos IAM para este modelo. Em seguida, clique em 'Criar Stack' para prosseguir com a criação da stack.

## Informações Adicionais <a href="#additional-information" id="additional-information"></a>

Agora você integrou seus Armazenamentos de Eventos BMS com a AWS e seus dados começarão a ser enviados assim que a criação da stack for concluída. Você pode acompanhar esse processo no painel das suas stacks. Confira estes artigos para saber mais sobre recursos relacionados da BMS e produtos AWS:

* [Pipelines de Eventos](../product-documentation/monitoring/event-pipes.md)
* [Armazenamento de Eventos](../product-documentation/monitoring/event-stores.md)
* [Chaves de API](../product-documentation/identity-access-management-iam/api-keys.md)
* [AWS CloudFormation](https://docs.aws.amazon.com/pt_br/cloudformation)
