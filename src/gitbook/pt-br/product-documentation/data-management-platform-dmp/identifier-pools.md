# Identifier Pools

Identifier Pools funcionam de maneira muito semelhante aos _cookie pools_, mas são projetados especificamente para dispositivos móveis, incluindo smartphones Android, tablets e produtos iOS. Cada sistema operacional emprega seus próprios métodos exclusivos para identificar os usuários de forma eficaz.

O Android do Google utiliza o GAID (_Google Advertising ID_), um identificador único fornecido pelo Google Play Services para fins publicitários. O GAID permite que desenvolvedores e anunciantes rastreiem a atividade do usuário e entreguem anúncios personalizados, ao mesmo tempo que dá aos usuários controle sobre suas configurações de privacidade.

O iOS da Apple atribui um identificador único e aleatório a cada usuário, conhecido como IDFA (_Identifier for Advertisers_). Semelhante ao GAID, o IDFA permite que desenvolvedores e anunciantes monitorem a atividade do usuário e sirvam anúncios personalizados, tudo isso enquanto oferece aos usuários controle sobre suas preferências de privacidade.

## Gerenciando Identifier Pools <a href="#managing-identifier-pools" id="managing-identifier-pools"></a>

<figure><img src="../../.gitbook/assets/image (1144).png" alt=""><figcaption><p> Lista de Identifier Pools</p></figcaption></figure>

### Criando um Identifier Pool <a href="#creating-an-identifier-pool" id="creating-an-identifier-pool"></a>

Um Identifier Pool deve ser criado antes de ser usado para uma campanha, para que possa ser populado. Configure por quanto tempo os identificadores devem ficar disponíveis antes de expirarem e defina quantos identificadores você deseja armazenar em seu _pool_. Além disso, selecione uma _Ad Exchange_ para sincronizar seus Identificadores com ela.

1. Clique em ![Create Identifier Pool](<../../.gitbook/assets/image (1148).png>) para criar um novo identifier pool.
2.  Preencha as informações:

    <figure><img src="../../.gitbook/assets/image (1146).png" alt=""><figcaption><p>Editor de Identifier Pool</p></figcaption></figure>

    * Nome: Informe como você deseja nomear seu identifier pool.
    * Tags: Defina tags para organizar seus identifier pools.
    * Exchanges: Selecione as _Ad Exchanges_ desejadas.
    * TTL (Tempo de Vida): Defina o número de dias que você deseja manter os identificadores no _pool_ após serem adicionados.
    * Tamanho Máximo (_Max Size_): Defina quantos identificadores podem ser adicionados ao _pool_.
3. Clique em ![Save](<../../.gitbook/assets/image (1149).png>) para salvar seu Identifier Pool.

### Editando um Identifier Pool <a href="#editing-an-identifier-pool" id="editing-an-identifier-pool"></a>

Após criar um identifier pool, você pode editá-lo clicando no botão de edição ![Edit](<../../.gitbook/assets/image (1155).png>). Todos os parâmetros são editáveis; para o TTL, as alterações se aplicarão apenas aos identificadores recém-adicionados. Após fazer suas alterações, clique em ![Save](<../../.gitbook/assets/image (1149).png>) para salvá-las.

É possível arquivar identifier pools para uma melhor organização. Clique em <img src="../../.gitbook/assets/image (6).png" alt="" data-size="line"> para arquivar o identifier pool selecionado e visualize seus identifier pools arquivados ativando a chave seletora "Arquivado" acima da lista. Também é possível desarquivar um identifier pool clicando em <img src="../../.gitbook/assets/image (7).png" alt="" data-size="line">.

### Excluindo um Identifier Pool <a href="#deleting-an-identifier-pool" id="deleting-an-identifier-pool"></a>

Você pode excluir um identifier pool clicando no botão de exclusão <img src="../../.gitbook/assets/image (8).png" alt="" data-size="line">. Para prosseguir com o processo, clique em <img src="../../.gitbook/assets/image (9).png" alt="" data-size="line"> para confirmar. Esteja ciente de que as ações de rastreadores baseadas nesses identifier pools deixarão de funcionar.

{% hint style="danger" %}
Atenção! Tenha cuidado ao excluir identifier pools. Esta ação não pode ser desfeita e todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos.
{% endhint %}

## Configurando Identifier Pools <a href="#configuring-identifier-pools" id="configuring-identifier-pools"></a>

Após criar um identifier pool, é necessário configurá-lo antes de usá-lo como um público-alvo em uma campanha.

Para usar identifier pools, você precisará configurar um rastreador ou usar um já existente. Este artigo é dedicado ao recurso de identifier pools; acesse nossa [documentação de Rastreadores](trackers/) para saber mais sobre a configuração de um rastreador.

### Criando uma Ação Vinculada a um Identifier Pool <a href="#creating-an-action-linked-to-an-identifier-pool" id="creating-an-action-linked-to-an-identifier-pool"></a>

Siga os passos abaixo para criar uma ação para um rastreador que adicionará ou removerá usuários de seus identifier pools.

Após criar e selecionar um rastreador da lista de rastreadores, siga os passos abaixo para vinculá-lo ao seu identifier pool:

1. Na aba Configuração, na seção de eventos rastreados, clique em ![Add Event](<../../.gitbook/assets/image (1158).png>) para adicionar um novo evento.
2.  Preencha as informações:\


    <figure><img src="../../.gitbook/assets/image (1161).png" alt=""><figcaption><p>Editor de Evento</p></figcaption></figure>

    * Nome: Informe como você deseja nomear este evento.
    * ID do Evento: Este campo pode ser personalizado, mas é preenchido automaticamente com o nome do evento.
    * Campos de dados personalizados: Defina campos de dados a serem coletados quando o evento for capturado.
    * Ações: Defina ações a serem executadas quando este evento for solicitado. Neste artigo, definiremos uma ação que adiciona ou remove identificadores do nosso _pool_ de identificadores.
      1. Clique em ![Add Event](<../../.gitbook/assets/image (1158).png>) para adicionar uma nova ação.
      2.  Preencha as informações:\


          <figure><img src="../../.gitbook/assets/Captura de tela 2025-02-27 084528.png" alt=""><figcaption><p>Editor de Ação</p></figcaption></figure>

          * Nome: Defina um nome para sua ação.
          * O que fazer?: Selecione Rastrear no Identifier Pool.
          * Identifier Pool: Selecione o identifier pool que você vinculará a esta ação.
          * Operação: Selecione se deseja adicionar ou remover identificadores do _pool_.
      3. Clique em ![Save](<../../.gitbook/assets/image (1149).png>) para salvar sua ação.
3. Clique em ![Save](<../../.gitbook/assets/image (1149).png>) novamente para salvar seu evento.

O rastreador deve ser instalado em todas as páginas do seu site onde você deseja rastrear a atividade do usuário. Após instalar o rastreador, pode levar um tempo, dependendo do tráfego do seu site, até que o sistema colete identificadores suficientes para usá-lo como um público-alvo em uma campanha.

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Você pode acompanhar o crescimento dos seus Identifier Pools usando a aba de métricas da Página de Identifier Pools. Estas são todas as métricas para este recurso:

* [Contagem de Identificadores Adicionados](dmp-metrics.md#contagem-de-identificadores-adicionados)
* [Contagem de Identificadores Habilitados](dmp-metrics.md#contagem-de-identificadores-habilitados)
* [Contagem de Identificadores Expirados](dmp-metrics.md#contagem-de-identificadores-expirados)
* [Contagem de Identificadores Removidos Manualmente](dmp-metrics.md#contagem-de-identificadores-removidos-manualmente)
* [Tamanho Máximo](dmp-metrics.md#tamanho-maximo-de-identifier-pool)
* [Tamanho](dmp-metrics.md#tamanho-de-identifier-pool)
* [Tempo até a Expiração](dmp-metrics.md#tempo-ate-a-expiracao-de-identifier-pool)
