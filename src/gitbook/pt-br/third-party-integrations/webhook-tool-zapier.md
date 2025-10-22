# Ferramenta de Webhook (Zapier)

## O que é um Webhook <a href="#what-is-a-webhook" id="what-is-a-webhook"></a>

Webhooks são normalmente usados para conectar dois aplicativos diferentes. Quando um evento ocorre no aplicativo de _trigger_ (gatilho), ele serializa os dados sobre esse evento e os envia para uma URL de webhook do aplicativo de _action_ (ação) — ou seja, o aplicativo que realizará alguma atividade com base nos dados do primeiro aplicativo. O aplicativo de ação então pode enviar uma mensagem de retorno (_callback_).

Colocando de outra forma: ao usar um Webhook, todos os dados fornecidos pelo primeiro aplicativo serão enviados automaticamente para um segundo aplicativo. Assim que os dados chegam ao segundo aplicativo, você pode definir quanto desses dados será utilizado, como eles serão utilizados e onde serão inseridos, criando uma gestão de dados totalmente personalizada.

Nesta solução, usaremos um caso em que queremos coletar dados relacionados a um evento _Ad-Delivered_. De todos os dados coletados a partir desse evento, utilizaremos apenas: **Timestamp**, **Domínio**, **ID da Campanha** e **ID do Anúncio**. Assim que obtivermos esses dados, criaremos uma ação para enviá-los a uma planilha do Google (_Google Sheet_).

O principal motivo para coletar esses dados específicos é que queremos saber exatamente em qual domínio o usuário está recebendo nossos banners, e verificar se esses domínios são relevantes para o público-alvo da nossa campanha.

## Requisitos <a href="#requirements" id="requirements"></a>

* Canal de eventos ou outro recurso que utilize Webhook
* Zapier ou qualquer ferramenta que possua recurso de Webhook
* Google Sheets
* Campanha Ativa

Siga os passos abaixo para gerenciar seus dados com sucesso por meio de um webhook.

* [Criando um Canal de Eventos](webhook-tool-zapier.md#criando-um-canal-de-eventos)
* [Configurando sua Ferramenta de Webhook](webhook-tool-zapier.md#configurando-sua-ferramenta-de-webhook) (Zapier)
* [Gatilho](webhook-tool-zapier.md#gatilho)
* [Ação](webhook-tool-zapier.md#acao)
* [Comece a Receber Dados!](webhook-tool-zapier.md#comece-a-receber-dados)

## Criando um Pipe de Eventos <a href="#creating-an-event-pipe" id="creating-an-event-pipe"></a>

Para usar um webhook, utilizaremos o recurso Canal de Eventos para coletar dados de uma campanha em andamento.

Ao usar o **Webhook do Zapier**, vá primeiro para a etapa do gatilho para obter o link do Webhook necessário para concluir a configuração do seu canal de eventos.\
\
Acesse a aba Monitoramento e clique em _**Event Pipes**_.

<div align="center"><figure><img src="../.gitbook/assets/image (491).png" alt=""><figcaption><p>Monitoramento</p></figcaption></figure></div>

Lá, criaremos um _event pipe_ clicando em <img src="../.gitbook/assets/image (492).png" alt="Create Event Pipe" data-size="line">, neste caso, criaremos um evento _ADS - Delivered_, então dentro de _Sample Event Template_ selecione o modelo de evento _ADS - Delivered_.

<figure><img src="../.gitbook/assets/image (493).png" alt="" width="538"><figcaption><p>Tela de Canal de Eventos</p></figcaption></figure>

Em seguida, clique em <img src="../.gitbook/assets/image (495).png" alt="Add Filter" data-size="line"> para adicionar um filtro e coletar dados de eventos _ad-delivered_, buscando por eventos que contenham _ad-delivered_ no campo Tipo.

<figure><img src="../.gitbook/assets/image (496).png" alt="" width="529"><figcaption><p>Filtro de Canal de Eventos</p></figcaption></figure>

Vá para a aba Alvos, é lá que configuramos o link do webhook. Clique em <img src="../.gitbook/assets/image (498).png" alt="Add Target" data-size="line"> e depois selecione Chamar Webhook.

<figure><img src="../.gitbook/assets/image (499).png" alt="" width="543"><figcaption><p>Tela de Criação de Alvo</p></figcaption></figure>

Insira a URL fornecida pelo Zapier ou pela sua ferramenta de gerenciamento de dados e, em seguida, salve seu Alvo e seu Canal de Eventos.

{% hint style="warning" %}
Em algumas ferramentas, o link do webhook **pode** já estar disponível. Se você estiver usando o **Zapier**, será necessário começar configurando seu webhook primeiro para obter o link.
{% endhint %}

<figure><img src="../.gitbook/assets/image (637).png" alt="" width="542"><figcaption><p>Webhook do Zapier Configurado</p></figcaption></figure>

Certifique-se de que seu Canal de Eventos esteja ativado e que haja uma campanha ativa para coletar dados e enviá-los para sua ferramenta de webhook.

<figure><img src="../.gitbook/assets/image (638).png" alt=""><figcaption><p>Canal de Eventos Habilitado</p></figcaption></figure>

## Configurando sua Ferramenta de Webhook <a href="#configuring-your-webhook-tool" id="configuring-your-webhook-tool"></a>

Para esta solução, usaremos o Zapier como exemplo, mas fique à vontade para usar sua ferramenta de gerenciamento de dados favorita, sendo o único requisito que ela possua recurso de Webhook.

O Zapier é uma ferramenta que oferece múltiplas integrações capazes de automatizar suas tarefas diárias. É uma ferramenta paga que disponibiliza um período de teste para que você possa verificar sua utilidade. Será necessário criar uma conta para começar a usar, mesmo durante o período de teste.

Se você também for usar o Zapier, este é o link para acesso: [Zapier](https://zapier.com/).

No Zapier, clique em <img src="../.gitbook/assets/image (270).png" alt="Create" data-size="line">, depois em Zaps.

<figure><img src="../.gitbook/assets/image (501).png" alt="" width="221"><figcaption><p>Menu de Criação do Zapier</p></figcaption></figure>

Em seguida, configuraremos nosso gatilho e ação, com base em Webhook + Canal de Eventos + Google Sheets.

<figure><img src="../.gitbook/assets/image (502).png" alt="" width="489"><figcaption><p>Gatilhos e Ações no Zapier</p></figcaption></figure>

### Gatilho <a href="#trigger" id="trigger"></a>

Este é o passo mais importante, pois aqui você obterá a URL do Webhook para começar a coletar dados da BMS.

Para configurar nosso gatilho, clique em _Trigger_ e depois pesquise por Webhooks by Zapier.

<figure><img src="../.gitbook/assets/image (503).png" alt=""><figcaption><p>Funcionalidade de Webhook</p></figcaption></figure>

Em seguida, vá para a aba _App & Event_ à sua direita, onde você configurará seu evento para um evento _Catch Hook_.

<figure><img src="../.gitbook/assets/image (505).png" alt="" width="404"><figcaption><p>Configuração do Webhook</p></figcaption></figure>

Vá para a aba _Test_ e obtenha sua **URL do Webhook**.

Essa URL será usada na configuração do seu Canal de Eventos [aqui](webhook-tool-zapier.md#criando-um-canal-de-eventos).

<figure><img src="../.gitbook/assets/image (506).png" alt="" width="410"><figcaption><p>URL do Webhook</p></figcaption></figure>

Após configurar a URL do webhook no seu Canal de Eventos, clique em _Test Trigger_ para coletar uma amostra de dados e usá-la para configurar sua Google Sheet.

{% hint style="warning" %}
_Atenção! Certifique-se de ter uma **Campanha Ativa** e seu Canal de Eventos **ativado** para que os dados estejam disponíveis para esse teste. Note que o teste é **necessário** para garantir que haja dados disponíveis para a configuração posterior na etapa de_ [_Ação_](webhook-tool-zapier.md#acao)_._
{% endhint %}

Os dados podem demorar um pouco para ficarem disponíveis. Assim que seu Canal de Eventos enviar informações para sua ferramenta, estes serão os dados que você receberá desse evento.

<figure><img src="../.gitbook/assets/image (639).png" alt="" width="402"><figcaption><p>Dados Coletados pelo Zapier</p></figcaption></figure>

Clique em <img src="../.gitbook/assets/image (935).png" alt="" data-size="line"> e então passaremos a configurar a Ação que será executada após a coleta dos dados.

Se todos os passos foram seguidos corretamente, seu Gatilho exibirá um <img src="../.gitbook/assets/image (937).png" alt="Check" data-size="line"> indicando que está funcionando conforme esperado.

### Ação <a href="#action" id="action"></a>

Usaremos o **Google Sheets** para gerenciar os dados coletados.

<figure><img src="../.gitbook/assets/image (936).png" alt="" width="377"><figcaption><p>Gatilho e Ação</p></figcaption></figure>

Crie um Google Sheet na sua conta preferida e deixe as colunas prontas para serem configuradas.

Neste exemplo, coletaremos os seguintes dados: **Timestamp**, **Domínio**, **ID da Campanha** e **ID do Anúncio**.

Observe que você pode nomear suas colunas conforme suas necessidades; fique à vontade para definir qualquer identificação que achar melhor para você.

<figure><img src="../.gitbook/assets/image (938).png" alt="" width="333"><figcaption><p>Google Sheet Configurado</p></figcaption></figure>

Usaremos o evento _Create Spreadsheet Row_ na configuração da ação do nosso Google Sheet.

<figure><img src="../.gitbook/assets/image (939).png" alt="" width="410"><figcaption><p>Configuração de Evento de Ação</p></figcaption></figure>

Após configurar sua conta na aba _Account_, vá para a aba _Action_.

Lá configuraremos nossa planilha, a aba da planilha (worksheet) e quais dados serão enviados para cada coluna.

<figure><img src="../.gitbook/assets/image (940).png" alt="" width="408"><figcaption><p>Planilha e Colunas Configuradas</p></figcaption></figure>

Para facilitar a busca de cada valor, digite na aba de pesquisa o valor que deseja coletar.

<figure><img src="../.gitbook/assets/image (941).png" alt=""><figcaption><p>Coleta de Dados</p></figcaption></figure>

Após configurar todos os campos de dados com a amostra coletada no teste do **Gatilho**, você estará pronto para começar os testes.

<figure><img src="../.gitbook/assets/image (942).png" alt="" width="400"><figcaption><p>Teste de Ação</p></figcaption></figure>

Clique em <img src="../.gitbook/assets/image (943).png" alt="" data-size="line"> e confirme se os dados foram enviados para sua planilha.

<figure><img src="../.gitbook/assets/image (490).png" alt="" width="563"><figcaption><p>Dados enviados para a Planilha</p></figcaption></figure>

Se todos os passos tiverem sido seguidos com sucesso, seus eventos terão um <img src="../.gitbook/assets/image (945).png" alt="Check" data-size="line">.

<figure><img src="../.gitbook/assets/image (946).png" alt="" width="251"><figcaption><p>Eventos Checados</p></figcaption></figure>

Clique em <img src="../.gitbook/assets/image (947).png" alt="" data-size="line"> para ativar seu webhook e todos os dados enviados pelo nosso recurso Canal de Eventos estarão disponíveis no seu Google Sheets!

## Comece a Receber Dados! <a href="#start-collecting-data" id="start-collecting-data"></a>

Assim que você tiver uma Campanha Ativa, Canal de Eventos e Webhook, é assim que seu Google Sheet será atualizado.

<figure><img src="../.gitbook/assets/Spreadsheetdata Animated.gif" alt="" width="563"><figcaption><p>Atualizações em Tempo Real no Google Sheets</p></figcaption></figure>

{% hint style="info" %}
_Se você tiver interesse em mais informações sobre Webhooks através do Zapier, aqui você pode encontrar informações mais detalhadas:_ [_Guia de Webhook do Zapier_](https://zapier.com/blog/what-are-webhooks/)_._
{% endhint %}

{% hint style="info" %}
_Existem muitas ferramentas que podem ser usadas para configurar um Webhook, portanto, encontre a que melhor atenda às suas necessidades. O Zapier é apenas uma entre várias opções._
{% endhint %}
