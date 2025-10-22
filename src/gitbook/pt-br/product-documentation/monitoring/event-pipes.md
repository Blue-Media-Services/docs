# Pipes de Eventos

Nossos _Pipes_ de Eventos são usados para coletar dados de todos os produtos em nossa plataforma. Você pode usar este recurso para acompanhar tudo o que pode causar um evento na BMS, desde campanhas até a criação de uma organização, permitindo que você organize os dados fornecidos como desejar.

Todos os _pipes_ de eventos criados serão enviados para um _Event Store_ ou você pode usar um _webhook_ para enviar esses dados diretamente para sua ferramenta de gerenciamento de dados. Fornecemos modelos para cada evento que podemos rastrear, para que você possa escolher de qual deseja coletar dados.

{% hint style="info" %}
_Temos uma solução que pode ajudá-lo a entender como um webhook funciona._ [_Confira este artigo aqui_](../../third-party-integrations/webhook-tool-zapier.md)_._
{% endhint %}

## Criando um Pipe de Eventos <a href="#creating-an-event-pipe" id="creating-an-event-pipe"></a>

Para criar um _pipe_ de eventos, clique em <img src="../../.gitbook/assets/image (276).png" alt="Create Event Pipe" data-size="line">, e uma tela de criação aparecerá.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 073841.png" alt=""><figcaption><p>Criação de Pipe de Eventos</p></figcaption></figure>

* Nome: Defina um nome para seu _Pipe_ de Eventos.
* Tags: Crie tags para identificar melhor cada _pipe_ de eventos.

### Filtros <a href="#filters" id="filters"></a>

Para começar a configurar seu _pipe_ de eventos, escolha um modelo de sua preferência na nossa aba Filtros, de acordo com suas necessidades.

* Modelo de Evento de Amostra: Neste menu suspenso, serão fornecidos todos os modelos relacionados aos eventos que podemos rastrear.

Neste exemplo, criaremos um _pipe_ de eventos para ADS - Delivered. Este evento rastreia cada Anúncio que está atualmente em uma campanha e entregando impressões. Uma vez que criarmos este _pipe_ de eventos, todos os dados serão enviados para um _Event Store_ ou um _Webhook_.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 074141.png" alt=""><figcaption><p>Pipe de Eventos para ADS - Ad Delivered</p></figcaption></figure>

Uma vez que o modelo esteja selecionado, você pode verificar quais dados serão coletados ao criar o _Pipe_ de Eventos correspondente.

Para coletar os dados, devemos inserir um filtro, clicando em ![Add Filter](<../../.gitbook/assets/image (279).png>).

<figure><img src="../../.gitbook/assets/image (280).png" alt="" width="515"><figcaption><p>Adicionando Filtros</p></figcaption></figure>

* Caminho: Tag específica na qual você pode identificar o evento. Ex: `id`, `type`, `source`, `data.accountId`.
* Operador: Regra que será usada neste filtro.
* Valor: O valor específico que a tag deve conter.

Neste caso, coletaremos dados de eventos de anúncios entregues, então a configuração ficaria assim:

<figure><img src="../../.gitbook/assets/image (281).png" alt="" width="524"><figcaption><p>Configurações de Filtro do Pipe de Eventos</p></figcaption></figure>

Especificamos o **Caminho** usando a tag "Type", escolhemos a opção de **Operador** "Contém" e adicionamos o **Valor** "Ad-delivered". Note que esses campos são sensíveis a maiúsculas e minúsculas, então os campos preenchidos devem corresponder ao modelo.

Depois de preencher todos os campos com as informações correspondentes com base no seu _pipe_ de eventos, o teste de filtro deve ter um sinal de verificação <img src="../../.gitbook/assets/image (282).png" alt="Test Filters Checked" data-size="line"> confirmando que está funcionando corretamente. Se não estiver funcionando corretamente devido a informações ausentes ou um erro de digitação, ele será apresentado com um sinal de aviso <img src="../../.gitbook/assets/image (284).png" alt="Test Filters Warning" data-size="line">.

<figure><img src="../../.gitbook/assets/image (283).png" alt="" width="518"><figcaption><p>Aviso de Teste de Filtro</p></figcaption></figure>

Neste caso, nosso filtro falhou devido à verificação em nosso campo Valor. Esses campos são sensíveis a maiúsculas e minúsculas e devem corresponder às informações correspondentes.

Depois de adicionar seus filtros, clique em <img src="../../.gitbook/assets/image (1113).png" alt="" data-size="line"> para salvar seu _pipe_ de eventos.

### Aba Destinos <a href="#targets-tab" id="targets-tab"></a>

Aqui você decidirá para onde enviar os dados: se serão enviados para um ou múltiplos event stores, um webhook ou uma Planilha Google.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-04 074833.png" alt=""><figcaption><p>Aba de Destinos do Pipe de Eventos</p></figcaption></figure>

Para configurar um destino, clique em ![Add Target](<../../.gitbook/assets/Captura de tela 2024-11-01 083709.png>) e preencha os detalhes de acordo com a opção de destino escolhida:

#### Enviar para Event Store <a href="#send-to-event-store" id="send-to-event-store"></a>

Você deve criar um event store antes de usá-lo como destino para seus pipes de eventos. [Saiba mais sobre Event Stores](event-stores.md).

<figure><img src="../../.gitbook/assets/image (1193).png" alt=""><figcaption><p>Destinar para Event Store</p></figcaption></figure>

Se você decidir enviar seus dados para um event store, basta nomear seu destino e escolher seu event store já criado.

* Nomeie seu destino&#x20;
* Selecione "Enviar para um Event Store"
* Selecione o Event Store que deseja usar.

Uma vez que estiver tudo configurado, clique em <img src="../../.gitbook/assets/image (289).png" alt="Save" data-size="line"> e seu pipe de eventos será listado.

#### Chamar Webhook <a href="#call-webhook" id="call-webhook"></a>

É possível enviar seus dados para um webhook fornecido por sua ferramenta de gerenciamento de dados. Selecione esta opção para usar a ferramenta de gerenciamento de dados de sua preferência e preencha os detalhes.

<figure><img src="../../.gitbook/assets/image (1066).png" alt=""><figcaption><p>Destinar para Webhook</p></figcaption></figure>

* Dê um nome ao seu destino.
* Selecione "Chamar Webhook".
* Insira a URL do webhook da sua ferramenta de gerenciamento de dados.

Depois de configurar sua URL de _webhook_, use nossa aba Testar Webhook para confirmar a usabilidade. Selecione um dos modelos de evento de amostra e clique em ![Test Webhook](<../../.gitbook/assets/image (1067).png>).

Se o teste do seu _webhook_ for bem-sucedido, o ícone será apresentado como ![Test Webhook Successful](<../../.gitbook/assets/image (1068).png>) e as abas do seu teste serão preenchidas:

* _Payload:_ Informação que será enviada para o seu _webhook_.
* Resultado: Status retornado e a latência.
* Requisição: Requisição usada pela BMS para enviar as informações para este teste.
* Resposta: Resposta recebida do seu _webhook_.

Após finalizar todas as configurações e testes, clique em <img src="../../.gitbook/assets/image (1065).png" alt="" data-size="line"> para salvar seu destino.

#### Google Sheets

Você também pode enviar seus dados para o Google Sheets. Selecione esta opção e preencha os detalhes.

<figure><img src="../../.gitbook/assets/image (1194).png" alt=""><figcaption><p>Destinar para Google Sheets</p></figcaption></figure>

* Dê um nome ao seu destino.
* Selecione "Google Sheets".
* Conecte-se com sua Conta Google para poder acessar a planilha.

Uma vez que estiver tudo configurado, clique em <img src="../../.gitbook/assets/image (289).png" alt="Save" data-size="line"> e seu pipe de eventos será listado.

### Habilitando seu Pipe de Eventos <a href="#enabling-your-event-pipe" id="enabling-your-event-pipe"></a>

Para habilitar um _pipe_ de eventos, simplesmente acione a chave seletora <img src="../../.gitbook/assets/image (510).png" alt="Toggle" data-size="line"> e ele será habilitado.

<figure><img src="../../.gitbook/assets/image (265).png" alt=""><figcaption><p>Pipe de Eventos Habilitado</p></figcaption></figure>

### Editando seu Pipe de Eventos <a href="#editing-your-event-pipe" id="editing-your-event-pipe"></a>

Para editar seu _pipe_ de eventos, clique em <img src="../../.gitbook/assets/image (512).png" alt="Edit" data-size="line">. Uma tela de edição aparecerá. Faça as alterações necessárias e clique em <img src="../../.gitbook/assets/image (509).png" alt="Save" data-size="line">.

<figure><img src="../../.gitbook/assets/image (271).png" alt="" width="527"><figcaption><p>Tela de Edição de Pipes de Eventos</p></figcaption></figure>

### Ações em Massa <a href="#bulk-actions" id="bulk-actions"></a>

Ao selecionar dois ou mais _pipes_ de eventos, as Ações em Massa serão habilitadas, permitindo que você realize ações em lote, como Arquivar e Excluir.

<figure><img src="../../.gitbook/assets/image (267).png" alt=""><figcaption><p>Ações em Massa - Pipes de Eventos</p></figcaption></figure>

### Arquivando e Desarquivando seu Pipe de Eventos <a href="#archiving-and-unarchiving-your-event-pipe" id="archiving-and-unarchiving-your-event-pipe"></a>

Para arquivar seu pipe de eventos, clique em <img src="../../.gitbook/assets/image (514).png" alt="Archive" data-size="line"> e ele será enviado para a lista de arquivados. Para desarquivar seu pipe de eventos, alterne a visualização para eventos arquivados clicando no botão de alternância <img src="../../.gitbook/assets/image (515).png" alt="Archived Toggle" data-size="line">. Você verá a lista de eventos arquivados. Clique em <img src="../../.gitbook/assets/image (962).png" alt="Unarchive" data-size="line"> para desarquivar um pipe de eventos.

### Excluindo seu Pipe de Eventos <a href="#deleting-your-event-pipe" id="deleting-your-event-pipe"></a>

Para excluir um _pipe_ de eventos, clique em ![](<../../.gitbook/assets/image (975).png>) e uma confirmação será necessária.

<figure><img src="../../.gitbook/assets/image (968).png" alt=""><figcaption><p>Exclusão de Pipes de Eventos</p></figcaption></figure>

Após clicar em <img src="../../.gitbook/assets/image (977).png" alt="Delete" data-size="line">, seu _pipe_ de eventos será excluído.

{% hint style="warning" %}
_Aconselhamos os usuários a arquivar em vez de excluir. Exclua apenas se tiver certeza, pois a ação não pode ser desfeita._
{% endhint %}

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Selecione um _pipe_ de eventos para acessar suas métricas. Selecionar mais de um mostrará uma comparação entre eles. As métricas são preenchidas assim que você cria os _pipes_ de eventos e eles estão habilitados e coletando dados.

Estas são todas as métricas para pipes de eventos:

* [Contagem de Eventos Correspondentes](monitoring-metrics.md#contagem-de-eventos-correspondentes)
* [Contagem de Chamadas de Execução de Destino](monitoring-metrics.md#contagem-de-chamadas-de-execucao-de-destino)
* [Taxa de Falha na Execução de Destino](monitoring-metrics.md#taxa-de-falha-na-execucao-de-destino)
