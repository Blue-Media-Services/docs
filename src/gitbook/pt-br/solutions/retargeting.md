# Criando uma Campanha de Retargeting

_Retargeting_ é uma estratégia de publicidade online projetada para reengajar usuários que já visitaram seu website ou aplicativo móvel mas não completaram uma ação desejada, como comprar um produto, cadastrar-se ou preencher um formulário. O principal objetivo do retargeting é trazer esses usuários de volta ao seu website ou app e motivá-los a completar a ação que inicialmente pretendiam.

Para ajudá-lo a criar uma campanha de retargeting do início ao fim, desenvolvemos este artigo. Aqui está o que vamos abordar para este propósito:

* [Criando e Instalando um Cookie Pool](retargeting.md#criando-um-cookie-pool)
* [Criando um Catálogo e Canais de Importação](retargeting.md#criando-um-catalogo)
* [Criando, Configurando e Instalando um Rastreador](retargeting.md#criando-rastreadores)
* [Criando Modelos de Recomendação](retargeting.md#criando-um-modelo-de-recomendacao)
* [Usando o Construtor de Criativos para Criar Builds e Blueprints](retargeting.md#construtor-de-criativos)
* [Criando Grupos Criativos](retargeting.md#criando-um-grupo-de-criativos)
* [Criando Anúncios e Anúncios em Lote](retargeting.md#criando-um-anuncio)
* [Configurando Regras para Anúncios](retargeting.md#criando-uma-regra)
* [Criando uma Campanha de Retargeting](retargeting.md#criando-uma-campanha)

## Cookie Pool

Começamos criando e instalando um _cookie pool_ em seu website. Um cookie pool é um banco de dados construído sobre cookies armazenados de usuários. Cookies são pequenos arquivos armazenados no navegador web de um usuário que contêm dados sobre seu comportamento na internet.

O recurso de cookie pool coleta dados adicionais sobre segmentação de audiência e melhora o desempenho da campanha.

### Criando um Cookie Pool <a href="#creating-a-cookie-pool" id="creating-a-cookie-pool"></a>

1. Na página inicial da BMS, no serviço de DMP, clique em Cookie Pools.
2. Clique em <img src="../.gitbook/assets/image (49).png" alt="" data-size="line"> para criar um Cookie Pool.
3. Defina um Nome e Tags para ele.
4. Insira seu domínio e selecione as ad exchanges desejadas.
5. Defina o período e o tamanho máximo do cookie pool.
6. Clique em <img src="../.gitbook/assets/image (50).png" alt="" data-size="line"> para salvar seu cookie pool.

### Instalando um Cookie Pool <a href="#installing-a-cookie-pool" id="installing-a-cookie-pool"></a>

1. Na página Cookie Pools, selecione a aba de Instruções de Instalação.
2. Clique no botão <img src="../.gitbook/assets/image (422).png" alt="Copy button" data-size="line"> para copiar a tag do cookie pool.
3. Adicione este código à tag \<head> das páginas onde deseja que seus usuários sejam adicionados ao pool.
   * Recomendamos pedir ao desenvolvedor do seu website para realizar esta ação.
   * Alternativamente, você pode instalar esta tag usando Google Tag Manager (GTM).

## Serviço de Armazenamento de Catálogo (CS2) <a href="#catalog-storage-service-cs2" id="catalog-storage-service-cs2"></a>

Se deseja promover produtos do seu website em seus banners publicitários, use o catálogo. Se este não for seu objetivo, pule esta etapa e prossiga com a configuração dos [rastreadores](retargeting.md#rastreadores).

Uma vez criado um cookie pool, é hora de criar seu catálogo de produtos. Isso permitirá que você use modelos de recomendação que aumentam as conversões de anúncios apresentando seus produtos em banners dinâmicos.

### Criando um Catálogo <a href="#creating-a-catalog" id="creating-a-catalog"></a>

1. Na página inicial da BMS, clique em Catálogos, na seção CS2.
2. Clique em <img src="../.gitbook/assets/image (423).png" alt="Create Catalog Button" data-size="line"> para criar um novo catálogo.
3. Defina um nome e tags para o catálogo.
4. Clique em <img src="../.gitbook/assets/image (419).png" alt="Save Button" data-size="line"> para salvar seu catálogo.
5. Siga as instruções na aba de instruções de instalação para instalar o pixel do catálogo em seu website:
   * Na aba  instruções de instalação, você terá acesso às tags de imagem necessárias para rastrear interações em seu website com os produtos do catálogo. Cada tag rastreia diferentes ações em seu website
   * É necessário substituir a seção indicada em vermelho pelo seu ID da oferta, o mesmo ID usado para importação para que as métricas possam ser sincronizadas.

{% hint style="danger" %}
Atenção! Você deve instalá-los com muito cuidado nas páginas corretas para garantir que sejam renderizados apenas 1 vez por evento, pois para a plataforma cada renderização é contada como 1 evento.
{% endhint %}

### Criando um Canal de Importação <a href="#creating-an-import-channel" id="creating-an-import-channel"></a>

1. No menu à direita, clique em Canais de Importação.
2. Clique em <img src="../.gitbook/assets/image (424).png" alt="+ import channel button" data-size="line"> para começar.
3. Aqui precisamos configurar as três abas disponíveis para que o canal funcione corretamente.
   * Aba Geral
     1. Defina um nome e tags para seu Canais de Importação.
     2. Selecione o catálogo para onde importará os dados de produtos.
     3. Selecione com que frequência seu catálogo deve ser atualizado para adicionar ou editar seus produtos.
     4. Selecione com que frequência seus produtos devem ser removidos de seu catálogo.
   * Aba Fonte
     1. Selecione o protocolo usado na URL de onde os produtos serão importados.
     2. Informe a URL de onde os produtos serão importados.
     3. Selecione o formato do seu catálogo entre as opções disponíveis.
   * Aba Mapeamento
     1. Informe o modelo do seu catálogo, esta etapa pode requerer ajuda de nossa equipe técnica.
     2. Clique em <img src="../.gitbook/assets/image (420).png" alt="Save Button" data-size="line"> para salvar suas mudanças![](<../.gitbook/assets/image (52).png>).

Após completar os passos acima, ative o canal de importação para começar a trabalhar com ele. Você também pode realizar um teste para confirmar que está funcionando corretamente. Para realizar este teste, siga os passos abaixo:

1. Selecione o canal de importação que deseja testar.
2. Clique em ![](<../.gitbook/assets/image (53).png>) para iniciar uma importação manual.
3. Marque a opção 'Modo de Teste'.
4. Selecione quantos produtos devem ser importados no teste.
5. Defina se deseja usar as configurações do canal para deletar produtos ou se deseja removê-los antes do teste começar.
6. Clique em <img src="../.gitbook/assets/image (426).png" alt="Start Button" data-size="line"> para começar o teste.
7. Selecione o canal de importação que você testou e, na aba tarefas, você pode confirmar se o canal está funcionando corretamente ou não. Caso haja algum problema, ele será exibido na coluna "Problemas".

### Produtos <a href="#products" id="products"></a>

Nesta seção, você poderá visualizar todos os seus produtos. Marque a caixa de seleção dos produtos e vá para a aba detalhes para ver informações mais detalhadas sobre ele, como o ID da Oferta, por exemplo.

## Rastreadores <a href="#trackers" id="trackers"></a>

Rastreie atividades do website de sua audiência usando rastreadores e utilize os dados para criar um modelo de recomendação de produtos baseado em seu catálogo.

### Criando Rastreadores <a href="#creating-trackers" id="creating-trackers"></a>

1. Na página inicial da BMS, clique em Rastreadores
2. Clique em <img src="../.gitbook/assets/image (54).png" alt="" data-size="line"> para adicionar um novo rastreador
3. Defina o nome para seu rastreador.
4. Configurar tags ajudará você a encontrar este rastreador mais facilmente.
5. Defina o número máximo de usuários. Novos usuários não poderão ser adicionados uma vez que o limite for atingido, mas as ações de usuários existentes continuarão sendo rastreadas.
6. Defina a quantidade máxima de eventos rastreados por usuário. Uma vez que o limite for atingido, o sistema automaticamente deletará os eventos mais antigos para dar espaço para novos.
7. Defina por quanto tempo deseja usar estes rastreadores . Após este período, as atividades do seu rastreador serão deletadas.

### Configurando Rastreadores <a href="#configuring-trackers" id="configuring-trackers"></a>

Configure eventos para rastrear ações específicas de sua audiência.

1. Na página Rastreadores, selecione um rastreador.
2. Na aba configuração, clique em <img src="../.gitbook/assets/image (55).png" alt="" data-size="line"> para criar um evento.
3. Definir um nome para seu evento automaticamente definirá um ID para ele.
4. Defina os Campos de Dados Personalizados com as informações que deseja rastrear, por exemplo: "offerid".
5. Clique em <img src="../.gitbook/assets/image (56).png" alt="" data-size="line"> para criar uma ação a ser executada após o evento ser rastreado.
6. Defina um nome para a ação.
7. Escolha entre uma ação 'Chamar um Webhook' ou 'Rastrear no Catálogo':
   * Para uma ação 'Chamar um Webhook', informe a URL para onde os dados devem ser enviados. Aqui você também pode escolher atividades padrão e personalizadas para serem rastreadas.
   * Para uma ação 'Rastrear no Catálogo', escolha o catálogo desejado, depois a atividade que deseja rastrear. Também é possível rastrear uma atividade personalizada.
8. Clique em <img src="../.gitbook/assets/image (58).png" alt="" data-size="line"> para salvar a ação que criou.
9. Sinta-se à vontade para adicionar mais ações a este evento, depois clique em <img src="../.gitbook/assets/image (59).png" alt="" data-size="line"> novamente para salvar seu evento.

### Instalando um Rastreador <a href="#installing-a-tracker-on-your-website" id="installing-a-tracker-on-your-website"></a>

Após criar seus rastreadores, eventos e ações, você deve instalá-los em seu website para começar a usá-los. Há 3 métodos de instalação disponíveis: Script, Pixel e Redirecionamento.

* Script
  1. Na página Rastreadores, selecione o rastreador desejado.
  2. Clique na aba 'Instruções de Instalação' e escolha o evento que deseja rastrear.
  3. Selecione a opção Script.
  4.  Se você configurou campos de dados personalizados, por favor use as seções indicadas para informar os valores.

      Aqui está um exemplo de como a seção indicada para seus campos de dados personalizados pode parecer para você: ![](<../.gitbook/assets/image (60).png>)

      _**Exemplo**: Você precisa rastrear qual cor de produto seus usuários estão mais interessados, você poderá usar este campo para coletar dados sobre a cor do produto_.
  5. Clique em <img src="../.gitbook/assets/image (61).png" alt="" data-size="line"> para copiar o script.
  6. Adicione este script ao código do seu website, na página onde o evento será rastreado
* Pixel
  1. Após escolher um evento na aba 'Instruções de Instalação', selecione a opção Pixel.
  2. Se você configurou campos de dados personalizados, por favor use as seções indicadas para informar os valores.
  3. Clique em <img src="../.gitbook/assets/image (62).png" alt="" data-size="line"> para copiar a tag Pixel
  4. Adicione a tag Pixel ao código do seu website, na página onde o evento será rastreado.
  5. Você também pode usar um gerenciador de tags, como Google Tag Manager, para adicionar este script ao seu website.
* Redirecionamento
  1. Após escolher um evento na aba 'Instruções de Instalação', selecione a opção Redirecionamento.
  2. Forneça a URL para onde o usuário deve ser redirecionado após o evento ser capturado.
  3. Se você configurou campos de dados personalizados, por favor use as seções indicadas para informar os valores.
  4. Clique em <img src="../.gitbook/assets/image (63).png" alt="" data-size="line"> para copiar a URL gerada e use-a como se fosse a URL que você forneceu anteriormente.

### Métricas de Rastreadores <a href="#trackers-metrics-tab" id="trackers-metrics-tab"></a>

A aba métricas permite visualizar como seus rastreadores, eventos e ações estão performando. Na aba métricas da página de rastreadores, é possível filtrar os dados que são exibidos de acordo com sua preferência. Aqui estão os filtros disponíveis no momento:

* "Agrupar por": Selecione como deseja agrupar os dados exibidos, por rastreador ou por evento
* "Visualização": Selecione como deseja exibir seus dados, cartões de métrica ou tabela de dados
* "Período": Selecione o período que contém os dados que você precisa

Os dados coletados pelos rastreadores tornam possível a exibição anúncios dinâmicos personalizados para seu público.

## Modelos de Recomendação <a href="#recommendation-models" id="recommendation-models"></a>

Modelos de recomendação são usados para preencher seus banners dinâmicos com dados sobre seus produtos baseados em seus catálogos e na atividade rastreada de seu website.

### Criando um Modelo de Recomendação <a href="#creating-a-recommendation-model" id="creating-a-recommendation-model"></a>

1. Na página inicial da BMS, clique em Modelos de Recomendação, na seção de CS2.
2. Clique em <img src="../.gitbook/assets/image (64).png" alt="" data-size="line"> para criar um novo modelo de recomendação.
3. Defina um Nome e Tags para o modelo.
4. Selecione o catálogo de onde o modelo coletará dados e interações de leads.
5. Clique em <img src="../.gitbook/assets/image (65).png" alt="" data-size="line"> para salvar suas alterações.

Se você parar de usar um modelo de recomendação, recomendamos desativá-lo ao invés de deletá-lo, pois deletar um modelo também deleta os dados coletados por este modelo de recomendação.

### Configurando uma Fonte <a href="#setting-up-a-source" id="setting-up-a-source"></a>

Agora que criamos nosso modelo de recomendação, precisamos configurar algumas fontes para alimentá-lo. Há 2 tipos de fontes disponíveis: Rastreadores (DMP) e Catálogos (CS2). Usar rastreadores como fonte relacionará seu modelo de recomendação aos dados coletados pelos rastreadores instalados em seu website. A opção catálogos relacionará seu modelo de recomendação aos dados do catálogo, estabelecendo um ranking de produtos. Abaixo estão os passos para realizar a configuração baseados no tipo de fonte desejado:

* DMP Rastreadores
  1. Selecione os modelos de recomendação para os quais deseja usar esta fonte.
  2. Na aba Configuração, clique em <img src="../.gitbook/assets/image (66).png" alt="" data-size="line"> para adicionar uma nova fonte.
  3. Defina um Nome.
  4. Defina um limite de produtos do catálogo de onde os dados serão coletados.
  5. Escolha DMP Rastreador como o tipo da fonte.
  6. Selecione o Rastreador de onde você coletará os dados.
  7. Selecione o evento configurado no rastreador de onde você coletará dados.
  8. Informe o campo contendo seus IDs da Oferta.
  9. Clique em <img src="../.gitbook/assets/image (67).png" alt="" data-size="line"> para salvar suas alterações.
* Ranking de Produtos CS2
  1. Realize os passos 1-4 acima.
  2. Escolha Ranking de Produtos CS2 como o tipo da fonte.
  3. Selecione a ação que deseja usar para ranquear produtos para esta fonte.
  4. Informe o período em que as métricas serão verificadas e coletadas.
  5. Clique em para salvar suas alterações.

Fontes trazem seus dados de produtos para seu banner dinâmico. Você deve ter pelo menos uma fonte para cada espaço disponível em seu banner dinâmico. Cada fonte preenche apenas um espaço por vez, então se você tiver mais espaços que fontes, alguns espaços ficarão vazios em seus banners dinâmicos. Também recomendamos configurar pelo menos 3 fontes por modelo de recomendação.

## Construtor de Criativos <a href="#creative-builder" id="creative-builder"></a>

Use o Construtor de Criativos para criar blueprints e builds que ajudarão você a criar seus anúncios mais rapidamente.

### Blueprints

Blueprints são modelos para criação de anúncios de forma rápida e eficiente. Estes modelos pré-feitos permitem que você construa anúncios que atendam às necessidades de seu negócio com facilidade.

Construídos em linguagens de desenvolvimento web, Blueprints podem oferecer a flexibilidade de criar banners dinâmicos. Também possuímos modelos de blueprints públicas para facilitar o uso por quem não possui conhecimento nas linguagens de desenvolvimento.

#### Como usar blueprints <a href="#how-to-use-blueprints" id="how-to-use-blueprints"></a>

Primeiro, você precisará escolher entre criar um blueprint por conta própria ou usar um blueprint já existente.

* **Criando um modelo de blueprint**
  1. Localize e clique em Blueprints na página inicial da BMS.
  2. Clique em <img src="../.gitbook/assets/image (68).png" alt="" data-size="line"> para começar.
  3. Defina um nome para sua Blueprint
  4. Defina tags para facilitar encontrá-lo depois
  5. Escolha a disponibilidade de acordo com sua preferência. Selecionar público tornará seu blueprint disponível para todos usando a plataforma BMS, e privado o manterá disponível apenas para você e aqueles com acesso à sua conta.
  6. Selecione os tamanhos de banner desejados.
  7. Clique em ![](<../.gitbook/assets/image (69).png>) para adicionar um novo grupo de parâmetros e começar a codificar seu banner.
  8. Sinta-se à vontade para usar os parâmetros do sistema de acordo com suas necessidades.
  9. Você também pode usar nossos Macros para melhor interação com o público de seus anúncios.
* **Usando um modelo de Blueprint existente**
  1. Localize e clique em Blueprints na página inicial da BMS.
  2. Desligue a opção 'Próprias', isso mostrará todos as Blueprints públicos disponíveis no momento.
  3. Escolha a Blueprint de acordo com as necessidades de seu negócio entre as opções disponíveis.
  4. Clique em <img src="../.gitbook/assets/image (70).png" alt="" data-size="line"> para duplicar a blueprint para sua conta.
  5. Clique em <img src="../.gitbook/assets/image (71).png" alt="" data-size="line"> para começar a editar sua cópia da blueprint. Aqui você pode fazer alterações na blueprint, ajustando-a para melhor refletir as necessidades de seu negócio.

### Builds

Crie builds usando seus modelos de blueprint. Builds ajudam você a criar banners dinâmicos mostrando produtos de seu catálogo, usados para suas campanhas de retargeting.

#### Criando Banners Dinâmicos com Builds <a href="#creating-dynamic-banners-using-builds" id="creating-dynamic-banners-using-builds"></a>

1. Na página inicial da BMS, localize e clique em Builds.
2. Clique em <img src="../.gitbook/assets/image (72).png" alt="" data-size="line"> para começar a criar uma nova build.
3. Defina um Nome para ela. Você também pode definir tags para facilitar seu rastreamento
4. Informe seu domínio.
5. Agora selecione um modelo de blueprint.
6. Selecione os tamanhos para seus banners. É recomendado usar tamanhos com proporções iguais para cada build. Por exemplo, use uma build para banners verticais e então crie outra para banners horizontais. Isso manterá as proporções dos logos, imagens e produtos mostrados
7. Use os Parâmetros no lado esquerdo para configurar e customizar seus logos, imagens, grades de produtos e mais.
8. Conforme você muda os parâmetros, pode ver uma prévia ao vivo de como seu banner será mostrado para ajudá-lo a encontrar o ajuste perfeito para as necessidades de seu negócio
9. Marque a caixa "Enviar criativos para revisão" e clique em <img src="../.gitbook/assets/image (73).png" alt="" data-size="line"> para salvar sua build e enviá-la para revisão dos Ad Exchanges.

## Grupos de Criativos <a href="#creative-groups" id="creative-groups"></a>

Agrupe vários criativos como uma única unidade para aplicar diferentes pesos e comparar performance entre variantes. Esta comparação é conhecida como teste A/B e é muito útil para descobrir quais tipos de criativos são mais interessantes para sua audiência.

### Criando um Grupo de Criativos <a href="#creating-a-creative-group" id="creating-a-creative-group"></a>

1. Na página inicial da BMS, clique em Grupos de Criativos, na Seção de Ad Server
2. Clique em <img src="../.gitbook/assets/image (74).png" alt="" data-size="line"> para criar um novo grupo criativo.
3. Defina um Nome e Tags para ele.
4. Selecione seu domínio.
5. Selecione o formato dos criativos no grupo.
6. Selecione os criativos que devem estar neste grupo. Clique em <img src="../.gitbook/assets/image (75).png" alt="" data-size="line"> para adicionar mais campos e selecionar seus criativos.
7. Defina o peso para cada criativo que adicionou.
8. Este peso será usado para definir quais criativos você deseja que sejam exibidos com mais frequência para seu target. Quanto maior o peso de um criativo, mais ele será exibido.
9. Você pode obter uma prévia de seu grupo após terminar esta configuração. Clique em <img src="../.gitbook/assets/image (76).png" alt="" data-size="line"> para ver a prévia.
10. Clique em <img src="../.gitbook/assets/image (77).png" alt="" data-size="line"> para salvar suas alterações.

## Anúncios <a href="#a-ds" id="a-ds"></a>

Aqui é onde você cria seus anúncios usando seus grupos criativos e os envia para revisão dos AdExchanges. Você também pode criar regras para controlar como seus anúncios serão entregues, e acompanhar o status e métricas de seus anúncios.

### Criando um Anúncio <a href="#creating-an-a-d" id="creating-an-a-d"></a>

1. Na página inicial da BMS, clique em Anúncios, na seção de Ad Server.
2. Clique em <img src="../.gitbook/assets/image (78).png" alt="" data-size="line"> para criar seu anúncio.
3. Nomeie-o e defina tags para ele.
4. Selecione seu domínio.
5. Escolha um formato para seu anúncio.
6. Selecione o grupo criativo que deseja usar.
7. Se você não tiver um grupo criativo ou precisar de um novo, pode rapidamente criar um clicando em ![](<../.gitbook/assets/image (79).png>).
8. Marque a caixa de seleção para enviar seu anúncio para revisão em todos os ad exchanges suportados.
9. Clique em <img src="../.gitbook/assets/image (81).png" alt="" data-size="line"> para salvar seu anúncio

### Anúncios em Lote <a href="#bulk-a-ds" id="bulk-a-ds"></a>

Você pode usar esta opção para criar anúncios de forma rápida e massiva.

1. Clique em <img src="../.gitbook/assets/image (82).png" alt="" data-size="line"> para começar.
2. Defina um Nome e Tags para seus anúncios.
3. Selecione seu domínio.
4. Informe a URL para onde o anúncio deve redirecionar quando clicado. Parametrização é permitida (UTM, por exemplo)
5. Clique em <img src="../.gitbook/assets/image (83).png" alt="" data-size="line"> para adicionar as imagens de seus criativos de acordo com as opções abaixo:
   * **Usar existente**
     1. Selecione todas as imagens que deseja entre as que já enviou para a plataforma.
     2. Clique em <img src="../.gitbook/assets/image (85).png" alt="" data-size="line"> para confirmar sua seleção.
   * **Enviar nova**
     1. Envie novas imagens para a plataforma arrastando-as para a caixa ou clicando em <img src="../.gitbook/assets/image (87).png" alt="" data-size="line"> e selecionando-as no armazenamento de seu dispositivo.
     2. Clique em <img src="../.gitbook/assets/image (84).png" alt="" data-size="line"> para confirmar sua seleção.
   * **Usar endereço Web (URL)**
     1. Adicione um URL de imagem por linha.
     2. Clique em para confirmar sua seleção.
     3. Marque a opção para agrupar criativos do mesmo formato para poder realizar um teste A/B.
     4. Marque a opção para enviar seus anúncios para revisão dos Ad Exchanges.
     5. Clique em <img src="../.gitbook/assets/image (88).png" alt="" data-size="line"> para salvar seus anúncios e enviá-los para revisão.

### Regras <a href="#rules" id="rules"></a>

Nesta aba, você pode configurar regras para que seus anúncios rodem apenas em horários e dias específicos.&#x20;

#### Criando uma Regra <a href="#creating-a-rule" id="creating-a-rule"></a>

1. Selecione o anúncio para o qual deseja configurar uma regra.
2. Na aba Regra, clique em <img src="../.gitbook/assets/image (89).png" alt="" data-size="line"> para adicionar uma nova regra.
3. Defina um Nome para ela e selecione qual Grupo Criativo deve ser afetado.
4. Mude a opção Agendamento para "ligado" ![](<../.gitbook/assets/image (90).png>).
5. Selecione os horários em que deseja que seus anúncios sejam exibidos em cada dia. Se houver dias em que não precisa que este anúncio rode, desmarque todos os horários nestes dias, e ele não rodará nestes dias.
6. Clique em <img src="../.gitbook/assets/image (91).png" alt="" data-size="line"> para salvar sua regra.

### Revisão por Ad Exchanges <a href="#a-d-exchange-reviews" id="a-d-exchange-reviews"></a>

Na aba Revisão das Exchanges, após criar seu anúncio, selecione-o para monitorar se as Ad Exchanges aprovarão ou rejeitarão seus anúncios. Em caso de recusa, você pode verificar o motivo na coluna comentários. Após fazer os ajustes necessários, você pode reenviar os anúncios para uma nova revisão.

## Campanhas <a href="#campaigns" id="campaigns"></a>

Aqui é onde você encontrará e poderá monitorar suas campanhas.

Neste artigo, estamos abordando a criação de campanhas de retargeting. Para ver uma descrição completa de todas as funções nesta página, por favor consulte nossa documentação de [campanhas](../product-documentation/demand-side-platform-dsp/campaigns.md).

### Criando uma Campanha <a href="#creating-a-campaign" id="creating-a-campaign"></a>

1. Na página inicial da BMS, clique em Campanhas, na seção de DSP.
2. Clique em <img src="../.gitbook/assets/image (92).png" alt="" data-size="line"> para começar a criar sua campanha.
3. Defina um nome e tags para ela.
4. Selecione seu domínio e fuso horário.
5. Defina quando a campanha deve começar e terminar.
6. Defina um valor para seus lances:
   * Fixo: Esta opção usará o valor configurado para o lance. Insira seu valor objetivo de CPM aqui.
   * Variável: Esta opção otimizará o valor de seu lance em um intervalo definido, buscando os menores lances possíveis. Insira o menor e o maior valor objetivo de CPM.
7. Defina o limite de frequência, que é o número de vezes que um anúncio da mesma campanha será exibido para o mesmo usuário.
8. Defina quantos lances você deseja solicitar por segundo.
9. Clique em <img src="../.gitbook/assets/image (93).png" alt="" data-size="line"> para salvar sua campanha.

### Público <a href="#target" id="target"></a>

Após criar sua campanha, você precisará definir um público para ela. Para campanhas de retargeting, você deve usar cookie pools como uma das opções de público, pois o objetivo é reengajar usuários que interagiram com seu website e o cookie pool é o recurso que coleta estes dados. Você tem algumas outras opções para ajudá-lo a construir seu público-alvo ideal, incluindo localização geográfica, idioma, categorias de domínios, domínios, palavras-chave e ad exchanges.&#x20;

Nossos públicos trabalham em um sistema '&', o que significa que cada público adicionado a uma campanha trabalhará com os outros para trazer a você uma audiência mais específica e qualificada.

#### Configurando um Público <a href="#creating-a-target" id="creating-a-target"></a>

1. Selecione a campanha que receberá este público.
2. Na aba Configuração, encontre a seção Público e clique em <img src="../.gitbook/assets/image (94).png" alt="" data-size="line"> para criar seu público.
3. Defina um nome para seu público.
4. Na aba Localizações, você pode definir a localização de seu público:
   * Geografias: Use isto para incluir ou excluir países e regiões onde sua campanha deve ser entregue
   * Geofences: Defina uma localização e o raio de distância de onde deseja que sua campanha seja entregue
5. Na aba Conteúdo, estão algumas configurações importantes para seu público:
   * Idiomas: selecione o idioma dos websites onde seus anúncios serão exibidos. Você também pode excluir idiomas que não deseja.
   * Categorias: inclua categorias específicas para que seus anúncios apareçam apenas em websites com conteúdo nessas categorias. Você também pode excluir categorias, para que seus anúncios não sejam exibidos em websites com conteúdo nas categorias excluídas.
   * Domínios: inclua domínios específicos para que seus anúncios apareçam apenas nos websites especificados. Você também pode excluir domínios para que seus anúncios não sejam exibidos nos websites excluídos.
   * Palavras-Chave na URL: inclua ou exclua palavras-chave para refinar onde seus anúncios aparecem baseados no conteúdo da URL.
6. Na aba Dispositivos, você pode definir parâmetros para os dispositivos de seus público:
   * Sistemas Operacionais: selecione sistemas operacionais para que seus anúncios sejam exibidos para usuários navegando na web nesses sistemas. Você também pode excluir sistemas operacionais para que seus anúncios não sejam exibidos para usuários nos sistemas excluídos.
   * Navegadores: selecione navegadores para que seus anúncios sejam exibidos para usuários navegando através desses navegadores. Você também pode excluir navegadores para que seus anúncios não sejam exibidos para usuários nos navegadores excluídos
   * Tipo de Dispositivo: selecione tipos de dispositivos para que seus anúncios sejam exibidos para usuários navegando nesses dispositivos. Você também pode excluir tipos de dispositivos para que seus anúncios não sejam exibidos para usuários nos dispositivos excluídos
   * Palavras-Chave em URLs Visitadas: ao configurar palavras-chave neste filtro, você está personalizando quais dispositivos verão seus anúncios baseados em seu histórico de navegação recente. Rastreamos as URLs que um dispositivo acessou nas últimas 24 horas
   * Domínios Visitados: Ao configurar domínios visitados, você está personalizando quais dispositivos verão seus anúncios baseados em seu histórico de navegação recente. Rastreamos os domínios que um dispositivo acessou nas últimas 24 horas
   * Cookie Pools: selecione cookie pools para que seus anúncios atinjam apenas usuários que foram adicionados aos pools selecionados. Você também pode excluir certos cookie pools para que seus anúncios não atinjam usuários dos pools excluídos. Esta é uma configuração necessária para campanhas de retargeting
7. Na aba Inventário, você pode definir seus exchanges, visibilidade e posição dos anúncios:
   * Exchanges: selecione ad exchanges para exibir seus anúncios através dessas plataformas. Você também pode excluir ad exchanges para que seus anúncios não apareçam nas plataformas excluídas.
   * Posições: selecione posições de inventário para posicionar estrategicamente seus anúncios para melhor visibilidade e engajamento. Você também pode excluir posições para colocar seus anúncios em todas as opções não excluídas.
   * Visibilidade: ajuste o controle deslizante para definir o limite mínimo de visibilidade para espaços de anúncio. Seus anúncios só serão pareados com posições de inventário onde a porcentagem de visibilidade é maior que o limite selecionado.
8. Clique em <img src="../.gitbook/assets/image (95).png" alt="" data-size="line"> para salvar seu público.

### Orçamento

Aqui você define o orçamento diário de sua campanha em USD. Você também pode rastrear quanto do orçamento já foi gasto, quanto ainda tem disponível e o objetivo de orçamento atual.

1. Na aba Configuração, na seção Orçamento, informe seu valor de orçamento em USD.
2. Clique em <img src="../.gitbook/assets/image (96).png" alt="" data-size="line"> para salvar suas alterações.

Agora sua campanha de retargeting está pronta para rodar. Você só precisa ativá-la e acompanhar como está indo nas abas métricas e tempo real. Aqui está um artigo sobre como as [métricas funcionam na plataforma BMS](../product-documentation/metrics.md).

{% hint style="info" %}
_Nosso leilão (bidding) funciona cruzando as informações das configurações de sua campanha e lances, então você receberá impressões baseadas apenas na configuração de sua campanha._
{% endhint %}
