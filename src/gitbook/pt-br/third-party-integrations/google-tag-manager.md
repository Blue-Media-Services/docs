# Google Tag Manager

Os gerenciadores de tags são uma ferramenta gratuita que facilita a adição, o gerenciamento e a atualização de códigos de rastreamento (ou “tags”) no seu site. Neste artigo, vamos falar sobre um deles, o mais popular e acessível, o Google Tag Manager, ou GTM. No entanto, todos funcionam de maneira semelhante, então fique à vontade para usar o gerenciador de tags que for mais conveniente para você.

Estes são os tópicos abordados neste artigo:

* [Instalando o Google Tag Manager](google-tag-manager.md#instalando-google-tag-manager)
* [Gatilhos](google-tag-manager.md#gatilhos)
* [Variáveis](google-tag-manager.md#variaveis)
* [Tags](google-tag-manager.md#tags)
* [Modelos](google-tag-manager.md#modelos)
* [Informações Adicionais](google-tag-manager.md#informacoes-adicionais)

## Instalando o Google Tag Manager <a href="#installing-google-tag-manager" id="installing-google-tag-manager"></a>

Após criar uma conta no GTM, você deve instalar o código do GTM nas páginas do seu site. Esse código pode ser encontrado na página inicial do seu contêiner.

<figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 105747.png" alt=""><figcaption><p>Página Inicial do Contêiner do GTM</p></figcaption></figure>

Clique no ID do contêiner para abrir as instruções de instalação do GTM. Há dois trechos de código que devem ser instalados no seu site: o primeiro deve ser inserido dentro da tag `<head>`, e o segundo dentro da tag `<body>`.

<figure><img src="../.gitbook/assets/image (894).png" alt=""><figcaption><p>Instruções de Instalação do GTM</p></figcaption></figure>

Após instalar os códigos do GTM, você poderá testar seu site para garantir que a instalação foi feita corretamente.

## Gatilhos <a href="#triggers" id="triggers"></a>

Configurar gatilhos é essencial para monitorar ações ou eventos específicos em seu site. Os gatilhos determinam quando e onde suas tags devem ser ativadas, permitindo que você gerencie os dados coletados para cada interação do usuário.

Você pode configurar gatilhos na página Gatilhos ou durante a criação ou edição de uma tag.

<figure><img src="../.gitbook/assets/image (895).png" alt=""><figcaption><p>Página de Gatilhos</p></figcaption></figure>

O GTM oferece diversos tipos de gatilhos para capturar diferentes ações dos usuários. Abaixo estão os mais utilizados no rastreamento de e-commerce:

1. **Visualização de Página:** Ativa quando uma página é carregada.
2. **Clique:** Ativa quando um elemento específico em uma página é clicado, como um botão "Adicionar ao carrinho".
3. **Envio de Formulário:** Ativa quando um formulário na página é enviado.
4. **Evento Personalizado:** Ativa com base em eventos JavaScript personalizados, sendo útil para interações complexas que não possuem gatilhos diretos no GTM.
5. **Pronto pra DOM:** Ativa quando o HTML da página é carregado (antes de imagens e outros elementos de mídia).

Você pode aprender mais sobre todos os tipos de gatilhos [neste artigo](https://support.google.com/tagmanager/topic/7679108?sjid=9288738402311135972-SA) do GTM.

### Configurando Gatilhos <a href="#setting-up-triggers" id="setting-up-triggers"></a>

Agora, vamos ver alguns exemplos para ajudar você a entender como configurar gatilhos:

_**Exemplo 1:** Configurando um gatilho de “Adicionar ao carrinho”_

**Objetivo:** Ativar uma tag quando um usuário clicar no botão "Adicionar ao carrinho".

1. Identifique o seletor CSS ou ID do botão:
   * Clique com o botão direito no botão "Adicionar ao carrinho" no seu site e selecione “Inspecionar”. Encontre o seletor CSS, ID ou classe única do botão (como .exemplo ou #exemplo).
2.  Crie o gatilho no GTM:

    <figure><img src="../.gitbook/assets/image (906).png" alt=""><figcaption><p>Configuração de Gatilho</p></figcaption></figure>

    * Clique em <img src="../.gitbook/assets/image (896).png" alt="" data-size="line"> e depois em <img src="../.gitbook/assets/image (897).png" alt="" data-size="original"> para começar a configurar seu gatilho.
    * Selecione Clique – Todos os Elementos se o botão não for um link, ou Clique – Apenas Links se for um link.
    * Em Tipo de Gatilho, escolha Alguns Cliques.
    * Defina as condições para corresponder ao seletor ou ID do botão. Por exemplo:
      * Elemento do Clique > Seletor CSS > .example.
    * Salve o gatilho e dê um nome descritivo, como Gatilho de **Clique em Adicionar ao Carrinho**.
3. Atribuir o Gatilho a uma Tag:

* Anexe este gatilho à tag de **Adicionar ao Carrinho** que você criou, para que ela seja ativada somente quando esse botão for clicado.

_**Exemplo 2:** Configurando um gatilho de Compra_

**Objetivo:** Ativar uma tag quando um usuário concluir uma compra (geralmente na página de “Obrigado” ou “Confirmação de Pedido”).

1. Use a URL da Página de Obrigado:
   * Encontre a URL única ou o padrão de URL da página de confirmação do pedido (por exemplo, /obrigado ou /confirmacao-de-pedido).
2.  Crie um gatilho de Visualização de Página:

    <figure><img src="../.gitbook/assets/image (907).png" alt=""><figcaption><p>Configuração de Gatilho</p></figcaption></figure>

    * Clique em <img src="../.gitbook/assets/image (896).png" alt="" data-size="line"> e depois em <img src="../.gitbook/assets/image (897).png" alt="" data-size="original"> para começar a configurar seu gatilho.
    * Escolha Visualização de Página como tipo de gatilho.
    * Selecione Algumas Visualizações de Página.
    * Defina a condição para corresponder à URL da página de Obrigado:
      * Caminho da Página > contém > /obrigado.
    * Salve o gatilho como Gatilho de Confirmação de Compra.
3. Anexar o gatilho à tag de Compra:
   * Atribua este gatilho à sua tag de Produto Pedido para acompanhar as compras concluídas.

_**Exemplo 3:** Usando um gatilho de Evento Personalizado para ações avançadas_

**Objetivo:** Ativar uma tag para ações que não correspondem aos gatilhos padrão, como eventos personalizados em JavaScript.

1. Implemente um Evento Personalizado:
   *   Se sua plataforma de e-commerce ou desenvolvedor puder adicionar eventos personalizados em JavaScript, você pode usar um evento `dataLayer.push` do JavaScript. Por exemplo:

       ```javascript
       dataLayer.push({
         event: 'addToCart',
         productID: '12345',
         productName: 'Sample Product'
       });
       ```
2.  Crie um gatilho de Evento Personalizado:

    <figure><img src="../.gitbook/assets/Captura de tela 2024-11-05 121903.png" alt=""><figcaption><p>Gatilho de Evento Customizado</p></figcaption></figure>

    * Clique em <img src="../.gitbook/assets/image (896).png" alt="" data-size="line"> e depois em <img src="../.gitbook/assets/image (897).png" alt="" data-size="original"> para começar a configurar seu gatilho.
    * Selecione Evento Personalizado como tipo de gatilho.
    * No campo Nome do Evento, insira o nome do evento usado no `dataLayer.push`, como `addToCart`.
    * Salve este gatilho como Gatilho de Evento Personalizado de Adicionar ao Carrinho.

## Variáveis <a href="#variables" id="variables"></a>

No GTM, variáveis são usadas para armazenar informações que podem ser utilizadas em tags, gatilhos e outras variáveis. Elas aumentam a funcionalidade das suas tags e gatilhos ao permitir que se ajustem dinamicamente com base nas ações do usuário ou nos dados presentes na página.

<figure><img src="../.gitbook/assets/image (898).png" alt=""><figcaption><p>Página de Variáveis</p></figcaption></figure>

### Entendendo Tipos de Variáveis <a href="#understanding-variable-types" id="understanding-variable-types"></a>

Existem dois tipos de variáveis disponíveis no GTM:

1. **Variáveis Internas:** O GTM oferece variáveis internas para ações comuns, como URL da Página, Clique em URL e ID do Formulário. Você pode ativá-las diretamente no GTM.
2. **Variáveis Definidas pelo Usuário:** São variáveis personalizadas que você cria para capturar dados específicos, como um ID de produto ou a classe de um botão clicado. Os tipos de variáveis definidas pelo usuário incluem:
   * **Variáveis da Camada de Dados:** Recuperam valores enviados para o `dataLayer` (por exemplo, o ID de um produto a partir do código do seu site).
   * **Variáveis de URL:** Capturam dados da URL da página, como parâmetros (por exemplo, parâmetros como `utm_campaign`).
   * **Variáveis JavaScript:** Recuperam valores diretamente de expressões JavaScript (por exemplo, propriedades do objeto _document_).
   * **Variáveis Constantes:** Armazenam valores fixos (por exemplo, um ID de rastreamento estático usado em várias tags).

### Configurando Variáveis <a href="#setting-up-variables" id="setting-up-variables"></a>

1. **Variáveis Internas**
   * Na seção **Variáveis Internas**, clique em <img src="../.gitbook/assets/image (900).png" alt="" data-size="line">.
   * Selecione as variáveis que deseja ativar marcando suas caixas (por exemplo, URL da Página, Clique em URL, Clique em Texto, ID do Formulário).
2.  **Variáveis Definidas pelo Usuário**

    *   _**Exemplo 1:** Criando uma Variável da Camada de Dados_

        _Variáveis da Camada de Dados recuperam dados que foram enviados para o `dataLayer`. Isso é útil ao rastrear ações ou valores específicos, como um ID de produto ou categoria._

        1.  **Envie dados para a Camada de Dados** (se ainda não tiver sido feito):\
            No seu site, certifique-se de que os dados necessários estão sendo enviados para o `dataLayer`. Aqui está um exemplo para uma página de produto:

            ```javascript
            dataLayer.push({
                event: 'productViewed',
                productID: '12345'  // Unique identifier for the product
            });
            ```
        2.  **Crie a Variável da Camada de Dados no GTM:**

            <figure><img src="../.gitbook/assets/image (901).png" alt=""><figcaption><p>Configuração da Variável – Exemplo da Camada de Dados</p></figcaption></figure>

            * Na seção Variáveis Definidas pelo Usuário, clique em <img src="../.gitbook/assets/image (902).png" alt="" data-size="line">.
            * Selecione Configuração da Variável e escolha Variável da Camada de Dados.
            * Em Nome da Variável da Camada de Dados, insira o nome usado no push da sua Camada de Dados (por exemplo, `productID`).
            * Opcionalmente, defina um valor padrão caso a variável esteja vazia (por exemplo, `desconhecido`).
            * Dê um nome e salve a variável (por exemplo, DL - ID do Produto).
        3. **Teste:** Use o modo de Visualização do GTM para testar se a variável captura corretamente o ID do produto.
    * _**Exemplo 2:** Criando uma Variável de URL_

    <figure><img src="../.gitbook/assets/image (903).png" alt=""><figcaption><p>Configuração de Variável – Exemplo de URL</p></figcaption></figure>

Variáveis de URL permitem capturar dados da URL da página, como parâmetros de rastreamento (`utm_campaign`) ou caminhos específicos da página.

1. Na seção Variáveis Definidas pelo Usuário, clique em <img src="../.gitbook/assets/image (902).png" alt="" data-size="line">.
2. Escolha Configuração da Variável e selecione URL.
3. No menu suspenso Tipo de Componente, escolha a parte da URL que você precisa:
   * Caminho: Captura o caminho depois do domínio (por exemplo, `/produtos/sapatos`).
   * Consulta: Captura parâmetros de URL específicos como `utm_campaign`.
4. Se você escolher Parâmetro de Consulta, insira a Chave do Parâmetro de Consulta (por exemplo, `utm_campaign`).
5. Salve a variável com um nome descritivo, como URL - Campanha UTM.

### Utilizando Variáveis <a href="#using-variables" id="using-variables"></a>

Após criar variáveis, você pode usá-las para tornar as tags e os acionadores mais dinâmicos.

1. **Em Tags:** Ao configurar uma tag, você pode inserir variáveis selecionando o símbolo \{{\}} ou digitando \{{nome da variável\}}. Por exemplo:
   * Use \{{ID de Rastreamento GA\}} em uma tag do Google Analytics no campo ID de Rastreamento.
   * Use \{{DL - ID do Produto\}} para passar dinamicamente o ID do produto em uma tag de conversão.
2. **Em Gatilhos:** Variáveis podem ser usadas em gatilhos para especificar condições de ativação. Por exemplo:
   * Crie um gatilho para disparar em páginas onde \{{URL - Caminho da Página\}} contenha /checkout

## Tags

Tags são trechos de código usados para coletar dados e monitorar interações dos usuários para plataformas de marketing e análise. Em vez de inserir manualmente cada tag no código do seu site, o GTM funciona como um hub central, permitindo que você gerencie todas as suas tags em um só lugar.

<figure><img src="../.gitbook/assets/image (908).png" alt=""><figcaption><p>Página de Tags</p></figcaption></figure>

### Criando Tags <a href="#creating-tags" id="creating-tags"></a>

Há muitas coisas que você pode realizar usando tags. O GTM oferece diversos tipos de tags. Aqui está um exemplo de como criar uma tag utilizando os códigos de pixel da BMS.

<figure><img src="../.gitbook/assets/image (912).png" alt=""><figcaption><p>Configuração de Tag</p></figcaption></figure>

1. Na página de Tags, clique em <img src="../.gitbook/assets/image (909).png" alt="" data-size="line"> para adicionar uma nova tag e depois em <img src="../.gitbook/assets/image (913).png" alt="" data-size="line"> para começar a configurá-la.
2. Selecione HTML Personalizado na lista.
3. No campo HTML, cole o código do pixel que você precisa instalar; no exemplo, foi usado um pixel de produto adicionado ao carrinho.
4. Lembre-se de substituir o ID da Oferta pelo identificador do produto usado em seu site ou usar uma variável do GTM previamente configurada vinculada a ele. Você pode saber mais sobre como o ID da Oferta da BMS funciona no nosso artigo sobre [Catálogos](../product-documentation/catalog-storage-service-cs2/catalogs.md#instalando-catalogos).
5.  Selecione os gatilhos que irão controlar quando esta tag será ativada.<br>

    <figure><img src="../.gitbook/assets/image (915).png" alt=""><figcaption></figcaption></figure>
6. Dê um nome e salve sua tag.
7. Clique em <img src="../.gitbook/assets/image (916).png" alt="" data-size="line"> para acessar uma pré-visualização da sua página com as tags instaladas e faça a depuração, se necessário. (Esta etapa é opcional)
8. Clique em <img src="../.gitbook/assets/Captura de tela 2025-04-24 103600.png" alt="" data-size="line"> para enviar suas alterações para a versão ao vivo do seu site.

## Modelos <a href="#templates" id="templates"></a>

Como alternativa, você pode usar nosso modelo de Tag Universal BMS para instalar os componentes da BMS no seu site de forma fácil. Este modelo único contém a maioria das nossas tags de produto, e vamos detalhar as ações disponíveis a seguir.

### Configurando a Tag Universal da BMS <a href="#configuring-bms-universal-tag" id="configuring-bms-universal-tag"></a>

Ao criar uma nova tag, você precisará escolher o tipo da sua tag; é aqui que você encontrará nosso modelo após pesquisá-lo como "BMS Universal Tag".

<figure><img src="../.gitbook/assets/image (1178).png" alt=""><figcaption><p>Escolha o tipo de tag – Pesquisando por BMS Universal Tag</p></figcaption></figure>

Após selecionar este modelo, você precisará preencher alguns detalhes de acordo com a ação que deseja executar. Estas são algumas das ações disponíveis:

* [Rastrear Página Carregada](google-tag-manager.md#rastrear-pagina-carregada)
* [Adicionar usuário a um Cookie Pool](google-tag-manager.md#adicionar-usuario-a-um-cookie-pool)
* [Registrar Atividade do Usuário em um Rastreador](google-tag-manager.md#registrar-atividade-do-usuario-em-um-rastreador)
* [Contar Evento no Catálogo](google-tag-manager.md#contar-evento-no-catalogo)
* [Contêiner de Tag](google-tag-manager.md#conteiner-de-tag)

#### Rastrear Página Carregada <a href="#track-page-loaded" id="track-page-loaded"></a>

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103042.png" alt=""><figcaption><p>Rastreamento de Carregamento de Página</p></figcaption></figure>

Quando acionada, esta ação executará a [Tag de Rastreio de Carregamento de Página](/broken/pages/gES7bgs4KZWs0wg6OGvy). Para configurá-la, você precisará preencher os seguintes detalhes:

* **ID da Conta BMS:** Seu número de conta BMS de 12 dígitos.

#### Adicionar usuário a um Cookie Pool <a href="#add-user-to-a-cookie-pool" id="add-user-to-a-cookie-pool"></a>

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103323.png" alt=""><figcaption><p>Adicionar usuário a um Cookie Pool</p></figcaption></figure>

Quando acionada, esta ação adicionará usuários a um [Cookie Pool](../product-documentation/data-management-platform-dmp/cookie-pools.md). Para configurá-la, você precisará preencher os seguintes detalhes:

* **ID da Conta BMS:** Seu número de conta BMS de 12 dígitos.
* **ID do Cookie Pool:** Insira seu ID do Cookie Pool; ele está disponível ao criar ou editar um cookie pool no editor de cookie pools.

#### Registrar Atividade do Usuário em um Rastreador <a href="#record-user-activity-in-a-tracker" id="record-user-activity-in-a-tracker"></a>

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103424.png" alt=""><figcaption><p>Registrar Atividade do Usuário em um Rastreador</p></figcaption></figure>

Quando acionada, esta ação executará as ações do seu [Rastreador](../product-documentation/data-management-platform-dmp/trackers/). Para configurá-la, você precisará preencher os seguintes detalhes:

* **ID da Conta BMS:** Seu número de conta BMS de 12 dígitos.
* **ID do Rastreador:** Insira seu ID do Rastreador; ele está disponível ao criar ou editar um rastreador no editor de rastreadores. Você também pode usar uma variável do seu site que forneça seu ID do Rastreador quando chamada.
* **ID do Evento:** Insira a variável que você identificou como o ID do Evento que deseja capturar.
* **Dados Personalizados:** Se você configurou campos de dados personalizados no seu Rastreador BMS, adicione-os aqui.

#### Contar Evento no Catálogo <a href="#count-event-in-a-catalog" id="count-event-in-a-catalog"></a>

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-24 103516.png" alt=""><figcaption><p>Contar Evento no Catálogo</p></figcaption></figure>

Quando acionada, esta ação carregará o pixel do seu [Catálogo](../product-documentation/catalog-storage-service-cs2/catalogs.md) no seu site. Para configurá-la, você precisará preencher os seguintes detalhes:

* **ID da Conta BMS:** Seu número de conta BMS de 12 dígitos.
* **Evento:** Selecione o evento que você deseja capturar no menu suspenso.
* **ID do Catálogo:** Você pode inserir o ID do seu catálogo ou usar uma variável do seu site que forneça o ID quando chamada.
* **ID do Produto:** Insira uma variável do seu site que forneça o ID do produto quando chamada.

#### Contêiner de Tag <a href="#include-tag-container" id="include-tag-container"></a>

<figure><img src="../.gitbook/assets/Captura de tela 2025-04-22 102738.png" alt=""><figcaption><p>Ação de Contêiner de Tag</p></figcaption></figure>

Quando acionada, esta ação carregará um [Contêiner de Tag](../product-documentation/tag-container/) no seu site. Para configurá-la, você precisará preencher os seguintes detalhes:

* **ID da Conta BMS:** Seu número de conta BMS de 12 dígitos.
* **ID do Contêiner de Tag:** Insira o ID do Contêiner de Tag da BMS.
* **Dados Personalizados:** Se você configurou campos de dados personalizados para este contêiner de tag, adicione-os aqui.

## Informações Adicionais <a href="#additional-information" id="additional-information"></a>

Cada site de comércio eletrônico ou website tem suas próprias particularidades. Para configurar o Google Tag Manager corretamente, é importante estar atento a esses detalhes. Você pode saber mais sobre algumas dessas plataformas de comércio eletrônico nos links abaixo:

* [Como usar o GTM na Nuvemshop](https://atendimento.nuvemshop.com.br/pt_BR/12313-codigos-externos/como-instalar-google-tag-manager-gtm-na-nuvemshop)
* [Como usar o GTM no Shopify](https://help.shopify.com/pt-BR/manual/promoting-marketing/pixels/custom-pixels/gtm-tutorial)
* [Como usar o GTM no Wix](https://support.wix.com/pt/article/adicionando-o-id-da-sua-conta-do-gerenciador-de-tags-do-google-ao-seu-site-wix)

Confira estes artigos para saber mais sobre como seu site ou plataforma de comércio eletrônico funciona, e os nomes que eles usam para eventos, identificadores de produto, etc.
