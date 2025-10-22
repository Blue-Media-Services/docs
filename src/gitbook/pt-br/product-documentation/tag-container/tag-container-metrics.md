# Métricas de Contêiner de Tags

Selecione um Contêiner de Tags na lista para exibir as métricas relacionadas a ele na aba de métricas. Selecionar nenhum mostrará métricas gerais da conta para todos os seus Contêineres de Tags, e selecionar mais de um exibirá uma comparação entre os selecionados. Além disso, ao revisar as métricas, você pode sempre usar o <img src="../../.gitbook/assets/image (1089).png" alt="" data-size="line"> para acessar nossos artigos sobre uma métrica específica.

{% hint style="info" %}
Você pode aprender mais sobre como as métricas são tratadas visitando a [página de Métricas](../metrics.md).
{% endhint %}

<figure><img src="../../.gitbook/assets/Captura de tela 2024-12-10 082108.png" alt=""><figcaption><p>Aba de Métricas - Contêiner de Tags</p></figcaption></figure>

### Taxa de Falhas <a href="#failure-rate" id="failure-rate"></a>

Essa métrica indica, em porcentagem, a frequência com que um contêiner de tags foi solicitado, mas a requisição falhou dentro do período de tempo definido.

<div data-full-width="false"><figure><img src="../../.gitbook/assets/Failure Rate.png" alt=""><figcaption><p>Métrica de Taxa de Falhas</p></figcaption></figure></div>

_**Exemplo:** Nesta imagem, o período definido foi de 1 semana, dividido em períodos diários. Como essa métrica mostra a taxa de falhas, o ideal é que os resultados sejam o mais baixos possível. Você perceberá que, neste caso, a taxa de falhas foi de 0%, o que significa que nenhuma requisição falhou durante esse período._

### Contagem de Requisições <a href="#request-count" id="request-count"></a>

Essa métrica representa o número de vezes que os contêineres de tags selecionados foram solicitados dentro do período de tempo definido.

<div data-full-width="true"><figure><img src="../../.gitbook/assets/request count.png" alt=""><figcaption><p>Métrica de Contagem de Requisições</p></figcaption></figure></div>

_**Exemplo:** Uma requisição é contabilizada cada vez que o contêiner de tags é carregado durante o carregamento do seu site, de acordo com sua instalação. Nesta imagem, você pode observar que o período definido foi de 1 semana, dividido em períodos diários. Cada linha representa um contêiner de tags diferente selecionado da lista. Por exemplo, a linha azul mostra um pouco mais de 1.000 requisições diárias nos primeiros 4 dias, depois caiu para cerca de 400 requisições em 28 de setembro, e variou entre 400 e 700 requisições pelo restante da semana._
