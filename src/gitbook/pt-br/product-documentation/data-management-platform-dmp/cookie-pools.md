---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Cookie Pools

Um cookie pool é uma coleção ou banco de dados de _cookies_ de usuários. _Cookies_ são pequenos pedaços de dados armazenados no navegador de um usuário quando ele visita um site. Esses _cookies_ registram o comportamento online dos usuários, suas preferências e interações com sites e serviços.

No contexto de publicidade e marketing digital, um _pool_ de cookies pode servir a vários propósitos:

* **Segmentação de Público**: Segmentar usuários em diferentes grupos com base em seus interesses, comportamentos, demografia ou outros critérios. Essa segmentação permite campanhas publicitárias mais direcionadas e personalizadas.
* **Retargeting**: Coletar dados de usuários com base em eventos e ações para fins de rastreamento. Esses dados podem ser usados posteriormente para criar modelos de recomendação para suas campanhas de _retargeting_, melhorando suas conversões. [Saiba mais sobre campanhas de Retargeting](../../solutions/retargeting.md).
* **Personalização de Anúncios**: Usar os dados coletados para exibir anúncios mais relevantes para cada usuário em sua segmentação, com base em sua atividade online recente, interesses e comportamento. Anúncios personalizados são mais envolventes e levam o anunciante a obter melhores resultados.
* **Análise e Medição**: Rastrear o desempenho de suas campanhas, medindo taxas de cliques, taxas de conversão, engajamento do usuário, entre outras métricas.
* **Limite de Frequência**: Definir limites de frequência para controlar a frequência com que um anúncio específico é mostrado a um usuário dentro de um determinado período. Isso evita a exibição repetida do mesmo anúncio para o mesmo usuário.

## Gerenciando Cookie Pools <a href="#managing-cookie-pools" id="managing-cookie-pools"></a>

<figure><img src="../../.gitbook/assets/Captura de tela 2024-08-15 091558.png" alt=""><figcaption><p>Lista de Cookie Pools</p></figcaption></figure>

### Criando um Cookie Pool <a href="#creating-a-cookie-pool" id="creating-a-cookie-pool"></a>

Um cookie pool deve ser criado pouco antes de ser usado para uma campanha, para que possa ser populado. Configure por quanto tempo seus cookies devem ficar disponíveis antes de expirarem, defina quantos cookies você deseja armazenar em seu pool e selecione as Ad Exchanges que você usará para sincronizar seus cookies com ele.

1. Clique em ![Create Cookie Pool](<../../.gitbook/assets/image (1135).png>) para criar um cookie pool.
2.  Preencha as informações:\


    <figure><img src="../../.gitbook/assets/Captura de tela 2024-08-15 090606.png" alt=""><figcaption><p>Editor de Cookie Pool</p></figcaption></figure>

    * Nome: Insira um nome para o seu cookie pool.
    * Tags: Insira tags para sua organização.
    * Exchanges: Selecione as _ad exchanges_ para sincronizar com seus cookies. Recomendamos selecionar apenas as _exchanges_ que você usará para veicular suas campanhas de anúncios, a fim de evitar cobranças desnecessárias.
    * TTL (Tempo de Vida): Defina o número de dias que um cookie será mantido no _pool_ após a sincronização.
    * Tamanho Máximo (_Max Size_): Defina a quantidade máxima de cookies que serão armazenados. Após atingir o limite, nenhum cookie a mais será adicionado ao _pool_ até que os antigos expirem, mas os cookies coletados ainda estarão disponíveis para uso. Também é possível aumentar o Tamanho Máximo para permitir que mais cookies sejam coletados.
3. Clique em ![Save](<../../.gitbook/assets/image (1132).png>) para salvar seu Cookie Pool.

### Editando um Cookie Pool <a href="#editing-a-cookie-pool" id="editing-a-cookie-pool"></a>

Após criar um _pool_ de cookies, você pode editá-lo clicando no botão de edição <img src="../../.gitbook/assets/image (175).png" alt="editing button" data-size="line">. Todos os parâmetros são editáveis; para o TTL, as alterações se aplicarão apenas aos cookies recém-adicionados. Após fazer suas alterações, clique em ![Save](<../../.gitbook/assets/image (1132).png>) para salvá-las.

É possível arquivar _pools_ de cookies para sua melhor organização. Clique em ![](<../../.gitbook/assets/image (359).png>) para arquivar o _pool_ de cookies selecionado. Visualize seus _pools_ de cookies arquivados ativando a chave seletora "Arquivados" acima da lista de _pools_ de cookies. Também é possível desarquivar um _pool_ de cookies clicando em ![](<../../.gitbook/assets/image (360).png>).

### Excluindo um Cookie Pool <a href="#deleting-a-cookie-pool" id="deleting-a-cookie-pool"></a>

{% hint style="danger" %}
Atenção! Tenha cuidado ao excluir _pools_ de cookies. Esta ação não pode ser desfeita e todos os dados relacionados, incluindo métricas coletadas anteriormente, também serão excluídos.
{% endhint %}

Você pode excluir um pool de cookies clicando no botão de exclusão <img src="../../.gitbook/assets/image (176).png" alt="delete button" data-size="original">. Um aviso de que esta ação não pode ser desfeita será exibido. Para prosseguir com o processo, clique em ![Delete](<../../.gitbook/assets/image (1134).png>) para confirmar que está excluindo, e pronto. Esteja ciente de que as segmentações baseadas nesses _pools_ de cookies deixarão de funcionar.

## Instalando um Cookie Pool <a href="#installing-a-cookie-pool" id="installing-a-cookie-pool"></a>

Após criar um cookie pool, você precisará instalá-lo em seu site para começar a usá-lo. Isso pode ser feito seguindo as instruções na aba Instruções de Instalação da página de cookie pools.

<figure><img src="../../.gitbook/assets/image (178).png" alt=""><figcaption><p>Aba de Instruções de Instalação</p></figcaption></figure>

1. Selecione o _pool_ de cookies que você irá instalar marcando a caixa de seleção ao lado de seu nome.
2. Na aba Instruções de Instalação, clique em <img src="../../.gitbook/assets/image (179).png" alt="" data-size="line"> para copiar o código.
3. Cole o código o mais alto possível dentro da tag `<head>` da página.
4. Se desejar, é possível usar um ID de usuário único. Isso é útil se seus usuários fazem login em múltiplos dispositivos. Para fazer isso, remova a parte indicada do código e insira o ID de usuário único.

Você também pode usar um gerenciador de tags, como o Google Tag Manager (GTM), para adicionar este código ao seu site.

## Aba de Métricas <a href="#metrics-tab" id="metrics-tab"></a>

Após instalar seus cookie pools, você deve começar a receber dados deles. É possível acompanhar este processo na aba de métricas. Estas são as métricas disponíveis para cookie pools:

* [Contagem de Expirações](dmp-metrics.md#contagem-de-expiracoes)
* [Tamanho Máximo](dmp-metrics.md#tamanho-maximo-de-cookie-pool)
* [Tamanho](dmp-metrics.md#tamanho-de-cookie-pool)
* [Contagem de Sincronizações](dmp-metrics.md#contagem-de-sincronizacoes)
* [Tempo até a Expiração](dmp-metrics.md#tempo-ate-a-expiracao)
