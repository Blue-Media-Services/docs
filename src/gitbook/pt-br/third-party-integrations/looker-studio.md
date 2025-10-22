# Looker  Studio

Looker Studio é uma plataforma de inteligência empresarial e visualização de dados que permite aos usuários transformar dados brutos em relatórios personalizados. Ela se integra a múltiplas fontes de dados, permitindo a criação de dashboards em tempo real para acompanhar o desempenho e analisar dados.

{% hint style="warning" %}
_Atenção! Antes de continuar, é necessário criar uma Chave de API com permissão para ler os dados de métricas da sua conta. Você pode aprender como fazer isso em nosso artigo sobre_ [_Chaves de API_](../product-documentation/identity-access-management-iam/api-keys.md)_._
{% endhint %}

## Conectando a BMS ao Looker Studio <a href="#connecting-bms-with-looker-studio" id="connecting-bms-with-looker-studio"></a>

Se você ainda não tem uma conta BMS, cadastre-se [aqui](https://console.bluems.com/#signUp).

A BMS possui um conector parceiro no Looker Studio para a API de métricas. Esse conector permite enviar dados das suas campanhas BMS para um relatório personalizado no Looker Studio. Abaixo estão os passos para configurar a BMS como Fonte de Dados.

<figure><img src="../.gitbook/assets/image (1110).png" alt=""><figcaption><p>Página inicial do Looker Studio</p></figcaption></figure>

1. Acesse o Looker Studio. Pode ser necessário criar uma conta caso você ainda não tenha uma.
2. Vá para a guia Fontes de Dados, localizada logo abaixo da barra de pesquisa.
3. Clique em "+ Criar Nova Fonte de Dados"
4. Para renomear sua fonte de dados, clique no nome padrão no canto superior esquerdo da página.
5.  Pesquise por "BMS" na barra de pesquisa.\


    <figure><img src="../.gitbook/assets/image (1111).png" alt=""><figcaption><p>Localizando o Conector BMS</p></figcaption></figure>


6. Clique em _BMS Monitoring_ para selecioná-la como fonte de dados.
7.  Preencha com os parâmetros corretos:\


    <figure><img src="../.gitbook/assets/image (1112).png" alt=""><figcaption><p>Parâmetros do Conector BMS</p></figcaption></figure>



    * **ID da Conta BMS:** Insira o ID da conta BMS que será conectada ao Looker Studio, no formato XXXX-XXXX-XXXX.
    * **Chave de API BMS:** Forneça uma Chave de API BMS com permissão para ler os dados de métricas da sua conta BMS.
    * **Período de Agregação:** Defina o intervalo de tempo padrão para agregar as estatísticas métricas ao consultar dados por carimbos de data/hora.
    * **Deslocamento de Fuso Horário:** Configure o deslocamento UTC para determinar o início do dia ao agrupar dados por dia.
    * **Permitir que o “Período de Agregação” seja modificado nos relatórios:** Marque esta opção se desejar permitir que o período de agregação seja alterado nos relatórios.
8. Após preencher todos os parâmetros corretamente, clique em "Conectar" no canto superior direito da página para concluir a conexão.

## Informações Adicionais <a href="#additional-information" id="additional-information"></a>

Agora os dados de métricas da sua conta BMS estão disponíveis como fonte de dados para relatórios no Looker Studio. Você pode usá-los para criar relatórios personalizados que fornecerão insights valiosos para o seu negócio. Aqui estão alguns artigos do Looker Studio para ajudar nesse processo:

* [Crie um Relatório](https://cloud.google.com/looker/docs/studio/create-a-report?hl=pt-br)
* [Sobre Conectores, Fontes de dados e Credenciais](https://cloud.google.com/looker/docs/studio/about-connectors-data-sources-and-credentials?hl=pt-br)
* [Nossas Políticas de Privacidade](https://bluems.com/privacy.html)
* [Nossos Termos de Uso](https://console.bluems.com/assets/docs/signup-terms-and-conditions-20240404.pdf)
