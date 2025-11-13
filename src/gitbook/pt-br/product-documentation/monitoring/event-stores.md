# Armazenamento de Eventos

Na nossa página armazenamento de eventos, você pode criar um repositório que atua como um banco de dados para armazenar eventos. Você poderá criar um armazenamento de eventos para onde seus _pipelines_ de eventos serão enviados. Em seguida, você pode baixar os eventos como um arquivo JSON e importá-lo para seu arquivo de gerenciamento de dados para organizá-lo melhor.

<figure><img src="../../.gitbook/assets/image (296).png" alt="" width="563"><figcaption><p>Armazenamento de Eventos</p></figcaption></figure>

## Criando um Armazenamento de Eventos <a href="#creating-an-event-store" id="creating-an-event-store"></a>

Para criar um armazenamento de eventos, clique em ![Create Event Store](<../../.gitbook/assets/image (1063).png>) e uma tela de criação aparecerá.

<figure><img src="../../.gitbook/assets/image (508).png" alt="" width="361"><figcaption><p>Criação de Armazenamento de Eventos</p></figcaption></figure>

* Nome: Defina um nome para seu armazenamento de eventos.
* Tags: Crie tags para identificar melhor cada armazenamento de eventos.
* Retenção: Decida por quanto tempo você manterá os dados coletados por este armazenamento de eventos. Após a expiração, os dados serão excluídos.

Após configurar seu armazenamento de eventos, clique no botão ![Save](<../../.gitbook/assets/image (1060).png>) para finalizar a criação.

### Habilitando seu Armazenamento de Eventos <a href="#enabling-your-event-store" id="enabling-your-event-store"></a>

Para habilitar um armazenamento de eventos, simplesmente acione a chave seletora <img src="../../.gitbook/assets/image (510).png" alt="Toggle" data-size="line"> e seu armazenamento de eventos será habilitado.

<div align="center"><figure><img src="../../.gitbook/assets/image (511).png" alt="" width="148"><figcaption><p>Armazenamento de Eventos Habilitado</p></figcaption></figure></div>

### Editando seu Armazenamento de Eventos <a href="#editing-your-event-store" id="editing-your-event-store"></a>

Para editar seu armazenamento de eventos, clique em <img src="../../.gitbook/assets/image (512).png" alt="Edit" data-size="line"> e uma tela de edição aparecerá. Faça as alterações necessárias e clique em ![Save](<../../.gitbook/assets/image (1060).png>).

<figure><img src="../../.gitbook/assets/image (513).png" alt="" width="360"><figcaption><p>Tela de Edição de Armazenamento de Eventos</p></figcaption></figure>

### Ações em Lote <a href="#bulk-actions" id="bulk-actions"></a>

Ao selecionar dois ou mais armazenamentos de eventos, as Ações em Lote serão habilitadas, permitindo que você realize ações em lote. Você será capaz de Arquivar, Excluir, Habilitar e Desabilitar armazenamento de eventos em lote.

<figure><img src="../../.gitbook/assets/image (266).png" alt="" width="188"><figcaption><p>Ações em Lote de Armazenamento de Eventos</p></figcaption></figure>

### Arquivando e Desarquivando seu Armazenamento de Eventos <a href="#archiving-and-unarchiving-your-event-store" id="archiving-and-unarchiving-your-event-store"></a>

Para arquivar seu armazenamento de eventos, clique em <img src="../../.gitbook/assets/image (514).png" alt="Archive" data-size="line">e ele será enviado para a lista de arquivados. Para desarquivar, mude sua visualização para a lista de arquivados acionando a chave seletora <img src="../../.gitbook/assets/image (515).png" alt="Archived Toggle" data-size="line">. Você verá a lista de itens arquivados. Clique em <img src="../../.gitbook/assets/image (962).png" alt="Unarchive" data-size="line"> para desarquivar um armazenamento de eventos.

### **Excluindo seu** Armazenamento de Eventos <a href="#deleting-your-event-store" id="deleting-your-event-store"></a>

Para excluir um armazenamento de eventos, clique em <img src="../../.gitbook/assets/image (963).png" alt="Delete" data-size="line"> e uma tela de confirmação aparecerá.

<figure><img src="../../.gitbook/assets/image (964).png" alt="" width="359"><figcaption><p>Tela de Exclusão</p></figcaption></figure>

Para confirmar sua exclusão, clique em ![Delete](<../../.gitbook/assets/image (1062).png>).

{% hint style="danger" %}
_Atenção! Se você excluir um armazenamento de eventos, todos os dados relacionados a ele serão excluídos._
{% endhint %}

## Fluxos de Eventos <a href="#event-streams" id="event-streams"></a>

Depois de criar seus armazenamentos de eventos e _pipelines_ de eventos, todos os eventos acionados serão apresentados na sua aba Fluxos de Eventos, estando disponíveis para download de acordo com suas configurações de retenção de dados.

Esses dados só serão exibidos se houver um _pipeline_ de eventos enviando dados para um armazenamento de eventos.

<figure><img src="../../.gitbook/assets/Captura de tela 2024-11-28 072309.png" alt=""><figcaption><p>Aba Fluxos de Eventos</p></figcaption></figure>

### Baixando seus Fluxos de Eventos <a href="#downloading-your-event-streams" id="downloading-your-event-streams"></a>

Você pode baixar seus fluxos de eventos clicando em ![](<../../.gitbook/assets/image (950).png>) na mesma linha do fluxo de eventos que deseja baixar. Existem dois formatos de arquivo disponíveis:

#### JSON-line

O formato JSON-line oferece uma visão bruta e não filtrada do fluxo de eventos, capturando todas as informações relevantes à medida que os eventos ocorrem. Este formato garante que nenhum dado seja deixado de fora, dando a você visibilidade completa de cada transação para análise detalhada ou integração em fluxos de trabalho personalizados.

<figure><img src="../../.gitbook/assets/image (951).png" alt=""><figcaption><p>JSON-line</p></figcaption></figure>

Selecione este formato e clique em ![Download](<../../.gitbook/assets/image (1064).png>) para baixar seu fluxo de eventos.

#### CSV

O formato CSV fornece uma visão personalizável e organizada do fluxo de eventos, permitindo que você escolha campos de dados específicos para exportação. Este formato torna os dados mais fáceis de analisar em aplicativos de planilha ou ferramentas de relatório, mantendo as informações essenciais necessárias para obter insights sobre o desempenho e a atividade da publicidade.

<figure><img src="../../.gitbook/assets/image (954).png" alt=""><figcaption><p>CSV</p></figcaption></figure>

É possível adicionar ou remover colunas do seu arquivo CSV. Para adicionar uma coluna, clique em <img src="../../.gitbook/assets/image (956).png" alt="" data-size="line">, e preencha os detalhes:

<figure><img src="../../.gitbook/assets/image (955).png" alt=""><figcaption><p>Adicionar Coluna</p></figcaption></figure>



* Rótulo - Informe o rótulo desejado para a coluna.
* Ler Dados De - Informe o parâmetro de onde você deseja ler os dados.
* Valor Padrão - Preencha com um valor padrão para a coluna (campo opcional).

Para remover uma coluna, selecione-a na lista e clique em ![](<../../.gitbook/assets/image (957).png>).

Após finalizar suas configurações, clique em ![Download](<../../.gitbook/assets/image (1064).png>) para baixar seu arquivo CSV.

### Ações em Lote <a href="#bulk-actions" id="bulk-actions"></a>

Você pode selecionar múltiplos fluxos de eventos marcando a <img src="../../.gitbook/assets/image (970).png" alt="Checkbox" data-size="line">. Após selecionar mais de um evento, as opções em lote serão habilitadas. Você pode baixar os fluxos de eventos selecionados clicando em <img src="../../.gitbook/assets/image (959).png" alt="" data-size="line">e selecionando um dos formatos de arquivo disponíveis.

Para baixar fluxos de eventos em lote, você pode selecionar até 100 fluxos individuais ou selecionar todos os fluxos de eventos.

Também é possível excluir seus fluxos de eventos em lote. Clique em <img src="../../.gitbook/assets/image (960).png" alt="" data-size="line">, selecione excluir e confirme a exclusão quando solicitado.

### Excluindo Fluxos de Eventos <a href="#deleting-event-streams" id="deleting-event-streams"></a>

Para excluir um evento, clique em ![](<../../.gitbook/assets/image (975).png>) e uma confirmação será necessária.

<figure><img src="../../.gitbook/assets/image (976).png" alt="" width="359"><figcaption><p>Exclusão de Evento</p></figcaption></figure>

Após clicar em ![Delete](<../../.gitbook/assets/image (1062).png>), seus dados do evento serão permanentemente excluídos.

{% hint style="danger" %}
_Atenção! Tenha cuidado ao excluir fluxos de eventos. Esta ação não pode ser desfeita, o que significa que seus dados são removidos permanentemente._
{% endhint %}

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Selecione um armazenamento de eventos para visualizar as métricas preenchidas pelos _pipelines_ de eventos. Note que você deve selecionar um armazenamento de evento para preencher ao criar um _pipeline_ de eventos. Se você enviar seus eventos apenas para um _webhook_, o armazenamento de eventos não será preenchido. Estas são todas as métricas disponíveis para o armazenamento de eventos:

* [Bytes do Fluxo ](monitoring-metrics.md#bytes-do-fluxo)
* [Contagem de Fluxos](monitoring-metrics.md#contagem-de-fluxos)
* [Bytes de Upload do Fluxo](monitoring-metrics.md#metrica-de-bytes-de-upload-do-fluxo)
* [Contagem de Uploads do Fluxo ](monitoring-metrics.md#contagem-de-uploads-do-fluxo)
* [Bytes de Download do Fluxo](monitoring-metrics.md#bytes-de-download-do-fluxo)
* [Contagem de Downloads do Fluxo ](monitoring-metrics.md#contagem-de-downloads-do-fluxo)
* [Bytes Excluídos do Fluxo ](monitoring-metrics.md#bytes-excluidos-do-fluxo)
* [Contagem de Exclusões do Fluxo](monitoring-metrics.md#contagem-de-exclusoes-de-fluxo)
